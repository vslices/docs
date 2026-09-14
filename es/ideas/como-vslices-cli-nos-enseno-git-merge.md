# ¿Cómo que no sabes qué es `git merge`?

> No importa. Nosotros tampoco… hasta que construimos VSlices CLI.

**Estado:** idea de entrada de blog  
**Origen:** experimento real de `TicketCode` durante la reconstrucción postmigración de Ticket Support.

## La idea

Durante años puedes usar `git merge`, resolver conflictos, escuchar hablar de `base`, `ours` y `theirs`, y aun así sentir que el concepto sigue siendo un poco abstracto.

La gracia de esta entrada sería contar que terminamos entendiendo el three-way merge no estudiando Git, sino construyendo VSlices CLI y necesitando preservar una materialización humana mientras una nueva proyección determinista cambiaba.

El punto pedagógico es contar el problema **antes** de introducir la abstracción.

## El caso real

VSlices tenía una proyección determinista previa de `TicketCode` con:

```csharp
namespace Tickets.Domain;
```

El archivo humano había evolucionado por su cuenta a:

```csharp
namespace Tickets.Domain.Aggregates;
```

Después, un nuevo experimento de target context estableció que el namespace determinista por defecto debía ser:

```text
RootNamespace evaluado del .csproj
+ path relativo completo desde el .csproj hasta el .vsir
```

Como `TicketCode.vsir` vive bajo:

```text
Tickets.Domain/
└── Aggregates/
    └── Tickets/
        └── TicketCode.vsir
```

la nueva proyección determinista pasó a ser:

```csharp
namespace Tickets.Domain.Aggregates.Tickets;
```

Y ahí apareció el conflicto.

## ¿Por qué esto es un conflicto si parece tan obvio?

Mirado sólo como dos strings actuales, parece tentador decir:

> “Pero si el determinista sólo extendió lo que ya tenía el humano. Dale nomás.”

Pero esa no es la pregunta que hace un three-way merge.

La pregunta real es:

> ¿Qué cambió el humano respecto del estado anterior, qué cambió la nueva proyección determinista respecto del mismo estado anterior, y puedo aplicar ambos cambios sin inventar intención?

En nuestro caso:

```text
BASE
Tickets.Domain|

HUMAN
Tickets.Domain|.Aggregates

NEXT DETERMINISTIC
Tickets.Domain|.Aggregates.Tickets
```

Los dos lados modificaron el mismo punto de inserción después de `Tickets.Domain`.

Aunque un humano pueda intuir una relación entre ambos cambios, VSlices no tiene autoridad para asumir que `.Aggregates` era una edición provisional que puede reemplazarse automáticamente.

Ese es un conflicto real.

## Y de repente… `git merge`

Hasta este punto podemos evitar completamente hablar de:

```text
base
ours
theirs
```

Primero usamos nombres concretos:

```text
lo que VSlices generó antes
lo que el humano tiene ahora
lo que VSlices generaría ahora
```

Y recién después revelamos:

> Felicidades. Acabas de entender el corazón de un three-way merge.

En Git, conceptualmente, esos estados corresponden al mismo patrón:

```text
base
ours
theirs
```

La abstracción deja de ser una definición que memorizar y pasa a ser el nombre de un problema que ya entendimos.

## Un caso sin conflicto

También conviene mostrar el caso fácil.

Estado anterior:

```csharp
MaxLength = 30;
ToString() => Value;
```

Cambio humano:

```csharp
MaxLength = 30;
ToString() => $"[{Value}]";
```

Nueva proyección determinista:

```csharp
MaxLength = 31;
ToString() => Value;
```

El humano cambió `ToString()` y el determinista cambió `MaxLength`.

No tocan la misma región, así que el merge puede producir:

```csharp
MaxLength = 31;
ToString() => $"[{Value}]";
```

Ese contraste ayuda a entender que un merge no elige un archivo ganador: intenta combinar cambios independientes respecto de un pasado común.

## La definición que nos terminó sirviendo

Una forma más intuitiva de describir un three-way merge sería:

> Fusionar dos conjuntos de cambios inferidos a partir de su diferencia contra un pasado común, siempre que hacerlo no requiera inventar la intención de ninguno de los dos lados.

En VSlices, la tríada concreta es:

```text
previous deterministic witness
human materialization
next deterministic witness
```

El rebaser intenta preservar las libertades humanas mientras incorpora los nuevos cambios deterministas.

Cuando puede demostrar que los cambios no chocan, los fusiona.

Cuando ambos lados tocaron la misma región, se detiene y pide una decisión explícita.

## El CLI como parte de la explicación

Este caso también sirve para mostrar por qué un buen conflicto no debería limitarse a decir:

```text
merge failed
```

VSlices puede mostrar los tres valores relevantes:

```text
Baseline insertion: <empty>
Human insertion: '.Aggregates'
Next deterministic insertion: '.Aggregates.Tickets'
```

Y después ofrecer una resolución explícita:

```bash
vslices lower TicketCode --resolve deterministic
```

La idea no es que `deterministic` sea siempre correcto. La idea es que la herramienta pueda explicar **qué decisión está pidiendo** y permitir que el usuario la tome conscientemente.

## Tesis de la entrada

La historia no sería solamente “cómo implementamos un merge en VSlices”.

La tesis más interesante es:

> Muchas abstracciones de software parecen más difíciles de lo que son porque solemos enseñarlas desde el vocabulario abstracto hacia el problema real.
>
> A nosotros nos tocó hacer el recorrido al revés: tuvimos un problema real, lo entendimos, construimos una solución y sólo entonces nos dimos cuenta de que habíamos terminado entendiendo mejor `git merge`.

Eso además encaja bastante bien con la intuición problem-first de VSlices.

## Posible estructura de la entrada final

1. **¿Cómo que no sabes qué es `git merge`?**  
   No importa. Nosotros tampoco… hasta que construimos VSlices CLI.
2. El problema real de `TicketCode`.
3. Tres estados, sin mencionar todavía `base/ours/theirs`.
4. ¿Por qué el caso del namespace es realmente un conflicto?
5. Un ejemplo donde los cambios sí se pueden combinar automáticamente.
6. “Felicidades: acabas de entender un three-way merge”.
7. Recién ahora: cómo se corresponde esto con `git merge`.
8. Qué aprendimos al diseñar mensajes de conflicto y resolución explícita en VSlices CLI.
9. Cierre: enseñar desde el problema hacia la abstracción.

## Frases que vale la pena conservar

> “¿Cómo que no sabes qué es `git merge`? No importa. Nosotros tampoco… hasta que construimos VSlices CLI.”

> “Un three-way merge no compara archivo A contra archivo B. Compara dos cambios distintos respecto de un tercer estado pasado.”

> “El merge no elige un archivo ganador; intenta combinar intenciones inferidas desde un pasado común.”

> “La herramienta no debería adivinar intención humana sólo porque a nosotros nos parezca obvia.”

> “Felicidades. Acabas de entender `git merge`.”

## Nota para cuando se escriba

Mantener el tono ligero y ligeramente irreverente. La gracia está en que el aprendizaje fue accidental y real, no en convertirlo en una explicación académica de algoritmos de merge.

El artículo puede profundizar después en detalles técnicos del rebaser de VSlices, pero el núcleo debe seguir siendo el recorrido:

```text
problema concreto
→ intuición
→ conflicto real
→ solución
→ nombre de la abstracción
```

No al revés.
