# Protocolo de colaboración entre VSlices Development y Research

## Estado

**Estado:** protocolo local de colaboración en evaluación.

Este documento preserva una forma de trabajo utilizada durante la ejecución de VSlices sobre Anamnesis y Concept.

No constituye por sí mismo una regla del protocolo base, una extensión del Docs Standard ni una obligación general de VSlices.

Su propósito es permitir que Development y Research colaboren sin mezclar responsabilidades y sin promover prematuramente una solución local a mecanismo reusable de la suite.

---

## Responsabilidades

### VSlices Development

Development es responsable de:

- detectar fricciones durante uso real de VSlices;
- intentar resolverlas primero con mecanismos existentes;
- proponer mecanismos técnicos o metodológicos locales cuando los existentes no alcanzan;
- ejecutar o co-ejecutar esas propuestas cuando corresponda;
- preservar su relación con el problema concreto que las originó;
- decidir, dentro de su autoridad, cómo diseñar o implementar VSlices.

### Research

Research es responsable de ayudar a:

- clasificar observaciones, tensiones, hipótesis, findings y preguntas;
- distinguir evidencia de interpretación;
- identificar confounders y límites de atribución;
- diseñar comparaciones, controles, benchmarks o replicaciones cuando hagan falta;
- determinar qué evidencia sería proporcional a una afirmación;
- evaluar si un resultado parece local, recurrente, reusable o todavía indeterminado.

Research no decide cómo debe diseñarse o implementarse VSlices.

Development no debe tratar una evaluación de Research como transferencia automática de autoridad técnica.

---

## Cuándo involucrar a Research

Development debería conversar con Research cuando aparezca al menos una de estas condiciones:

- una fricción real parece revelar una limitación de VSlices y no sólo del caso local;
- aparece una construcción nueva que podría ser candidata a mecanismo reusable;
- una preferencia de diseño empieza a presentarse como mejora metodológica;
- existe riesgo de atribuir a VSlices un resultado que puede explicarse por evolución normal del consumidor, documentación general u otra intervención;
- una abstracción podría estar siendo promovida desde evidencia de un solo caso;
- se necesita definir qué evidencia permitiría adoptar, rechazar o mantener provisional una práctica;
- un cambio retrospectivo puede reescribir artificialmente la trayectoria anterior;
- una conclusión parece generalizable pero todavía no existen casos comparativos suficientes;
- una implementación, benchmark o experimento técnico necesita evaluación metodológica independiente;
- una práctica parece útil pero su costo, drift, excepciones o efectos adversos todavía no están caracterizados.

No es necesario involucrar a Research por cada decisión técnica local ni por cada iteración normal de implementación.

---

## Forma preferida de presentar una nueva presión

Cuando Development entregue una observación o candidata a Research, debería preferir esta secuencia:

```text
Friction
→ Existing mechanisms
→ Observed limit
→ Local candidate
→ Evidence to collect
```

### Friction

Describir primero el problema real observado.

Preguntas útiles:

- ¿Qué intentábamos hacer?
- ¿Qué necesidad estaba activa?
- ¿Qué costo, ambigüedad, pérdida de continuidad o bloqueo apareció?
- ¿Qué falla si no introducimos ninguna solución nueva?

La fricción debe poder entenderse sin aceptar todavía la solución propuesta.

### Existing mechanisms

Indicar qué mecanismos existentes de VSlices se intentaron o podrían razonablemente utilizarse.

Esto evita crear construcciones nuevas sólo porque todavía no se examinó adecuadamente el vocabulario actual.

### Observed limit

Preservar dónde los mecanismos existentes:

- alcanzan;
- obligan a reconstrucción costosa;
- generan duplicación;
- pierden información relevante;
- mezclan responsabilidades;
- producen ambigüedad;
- o fuerzan una semántica que el caso no sostiene.

No basta con que una alternativa nueva parezca más elegante.

### Local candidate

Sólo después de preservar la fricción y el límite observado, describir la mínima estructura local que Development propone probar.

La candidata debe permanecer local mientras no exista evidencia suficiente para promoción.

### Evidence to collect

Definir qué observar durante uso real.

Según el caso puede incluir:

- costo de reanudación;
- costo de reconstrucción;
- drift entre fuentes;
- carga de mantenimiento;
- frecuencia de replanning;
- trabajo invalidado;
- facilidad para identificar el siguiente movimiento;
- errores evitados o introducidos;
- excepciones;
- contraejemplos;
- respuesta de otros consumidores;
- reconstrucción desde contexto fresco.

---

## Escalera epistemológica

Development y Research deben evitar saltar directamente desde una solución útil a una regla general.

La trayectoria preferida es:

```text
solución útil aquí
≠
patrón recurrente
≠
mecanismo reusable de VSlices
≠
invariante del método
```

Una construcción puede permanecer indefinidamente en cualquiera de esos niveles.

No existe obligación de promoción.

---

## Regla de mínima promoción

Ante una fricción nueva:

```text
encuentra una fricción real
→ intenta resolverla con mecanismos existentes
→ documenta dónde esos mecanismos alcanzan y dónde fuerzan
→ introduce la mínima estructura local necesaria
→ úsala durante ejecución real
→ conserva costo, utilidad, drift y excepciones
→ recién después considera promoción
```

Si el mecanismo existente resulta suficiente, la nueva construcción debe abandonarse o permanecer como conveniencia local.

Si la construcción local funciona pero no aparece presión independiente, debe evitarse inferir reusabilidad sólo por éxito en un caso.

---

## Autoridad y participación

La participación no implica autoridad.

```text
recommendation
≠
authority

co-execution
≠
ownership

implementation
≠
methodological validation
```

Development puede recomendar o co-ejecutar trabajo con un consumidor sin apropiarse de:

- sus necesidades;
- sus decisiones de producto;
- sus prioridades externas;
- sus criterios de aceptación;
- sus restricciones organizacionales;
- sus artefactos cuya autoridad pertenezca a otra superficie.

Research puede evaluar una propuesta sin convertirse en autoridad de diseño sobre VSlices.

---

## No reinterpretación retrospectiva

Cuando una construcción nueva describa adecuadamente trabajo previo, preservar la trayectoria real:

```text
trabajo original
→ evidencia o fricción
→ interpretación posterior
→ nueva construcción
```

No reescribirla como:

```text
la nueva construcción guió siempre el trabajo
```

Esto aplica especialmente a:

- modalidades reconocidas retrospectivamente;
- reclasificación de milestones o checkpoints;
- nuevas categorías documentales;
- nuevas relaciones entre artefactos;
- nuevas reglas de interacción o navegación.

---

## Cambios promovidos a VSlices

Una recomendación de Research favorable a continuar una prueba no implica promoción automática.

Antes de promover una práctica local a VSlices, Development debería poder responder suficientemente:

1. ¿Qué fricción concreta resolvió?
2. ¿Por qué los mecanismos existentes eran insuficientes?
3. ¿Qué evidencia tenemos de utilidad real?
4. ¿Qué costo o complejidad introduce?
5. ¿Qué excepciones o contraejemplos conocemos?
6. ¿La necesidad reapareció independientemente?
7. ¿Qué afirmación exacta estamos autorizados a hacer con la evidencia disponible?
8. ¿Quién tiene autoridad para realizar el cambio correspondiente?

Si alguna respuesta requiere inventar conocimiento, la promoción debe permanecer abierta.

---

## Aplicación actual en Anamnesis / Concept

Las siguientes construcciones permanecen actualmente como presión operacional local o hipótesis en evaluación:

- proyección de `Execution State`;
- `Checkpoint Plan`;
- relación entre `Deliverable` y `Milestone`;
- modos de interacción o asesoría con consumidores;
- promotion lineage;
- posible coexistencia de varios Continuity Paths primarios.

Su presencia en esta ejecución no las convierte automáticamente en mecanismos del protocolo base ni del Docs Standard.

La estrategia actual es:

```text
usar
→ observar
→ comparar con mecanismos existentes
→ medir costo y utilidad
→ buscar contraejemplos
→ repetir
→ evaluar promoción / rechazo / disolución
```

---

## Resultado esperado de la colaboración

La colaboración entre Development y Research debería permitir que una propuesta termine, de forma explícita, en alguno de estos estados:

```text
local-useful
provisional
needs-more-evidence
candidate-for-replication
candidate-for-promotion
rejected
dissolved-into-existing-mechanism
```

Estos estados son descriptores operativos de esta colaboración y no una taxonomía formal del protocolo base.

El objetivo no es maximizar la cantidad de ideas promovidas.

El objetivo es que, cuando VSlices cambie, pueda reconstruirse qué problema real motivó el cambio, qué evidencia lo respaldó, qué alternativas fueron consideradas y qué grado de generalidad está realmente justificado.
