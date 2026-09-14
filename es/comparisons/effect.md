# VSlices y Effect

## Propósito

Este documento compara VSlices con [Effect](https://effect.website/), una biblioteca y ecosistema para construir aplicaciones robustas, mantenibles y tipadas en TypeScript.

Effect es un precedente especialmente relevante para VSlices porque concentra, dentro de una semántica coherente de ejecución, varias preocupaciones que VSlices también reconoce en su superficie ejecutable: efectos, errores tipados, requisitos de runtime, composición de servicios, concurrencia estructurada, scheduling, resource management, schemas, tracing y resolución declarativa de requests.

La comparación no implica genealogía.

VSlices no deriva de Effect, ni pretende reproducir su API. Muchas de las similitudes aparecieron de forma independiente al perseguir problemas parecidos desde puntos de partida distintos.

!!! note "Una forma deliberadamente provocadora de decirlo"

    **Effect is a parent architecture — only if all you do is code.**

    La frase no afirma que Effect sea históricamente la arquitectura madre de VSlices. Señala una diferencia de alcance: si se observa únicamente la superficie ejecutable de VSlices, Effect puede parecer un precedente arquitectónico muy cercano. VSlices, sin embargo, comienza antes del código y continúa después de él.

## Estado de la comparación

Esta página describe una comparación conceptual, no una garantía de equivalencia funcional.

A fecha de 12 de septiembre de 2026:

- Effect v4 se encuentra en Release Candidate;
- la versión estable publicada sin tag continúa siendo Effect v3;
- el repositorio de Effect describe como preocupaciones centrales los errores tipados, dependency injection, structured concurrency, scheduling, tracing y schema validation.

Por tratarse de un ecosistema activo, los detalles de API pueden cambiar. Esta comparación se concentra principalmente en las responsabilidades y las ideas arquitectónicas, no en firmas concretas.

## La similitud principal

Effect puede entenderse como un _application foundation_ orientado a representar y ejecutar programas con semántica explícita.

VSlices puede llegar a ofrecer una superficie equivalente o más amplia dentro de VSlices Framework y sus realizaciones, pero el proyecto completo tiene un alcance mayor.

Effect trabaja principalmente sobre problemas de software ejecutable.

VSlices intenta preservar continuidad entre:

- realidad de negocio;
- contexto operativo;
- conocimiento de dominio;
- documentación;
- decisiones;
- diseño;
- representación semántica;
- implementación;
- verificación;
- operación;
- y evolución.

Por ello, la relación más útil no es:

```text
Effect API ⊂ VSlices API
```

ni tampoco:

```text
Everything Effect can do
is already implemented by VSlices
```

La afirmación relevante es de alcance:

```text
Effect's problem space
        ⊂
a portion of VSlices' intended problem space
```

VSlices puede considerarse un _scope superset_ de varias preocupaciones que Effect materializa, sin afirmar todavía paridad de features ni equivalencia de madurez.

## Diferencia de dirección

Una diferencia fundamental aparece al observar de dónde proviene la semántica.

Effect puede partir de una definición programática y derivar representaciones e intérpretes ejecutables desde ella.

Por ejemplo, su sistema de Schema permite definir estructura y transformaciones y luego derivar validación, codecs, formatters u otras interpretaciones.

VSlices sigue una trayectoria distinta:

```text
Reality / Problem
       ↓
Understanding
       ↓
Documentation
       ↓
Continuity
       ↓
Semantic Representation
       ↓
Implementation
       ↓
Verification / Operation
       ↓
Updated Understanding
```

En VSlices, `.vsir` no pretende reemplazar la documentación que le da origen.

Es una representación computable de conocimiento que ya fue preservado mediante continuidad.

Esto importa porque una representación semántica puede contener invariantes, traits, transformaciones y relaciones ejecutables sin necesariamente conservar por sí sola:

- por qué una decisión existe;
- qué tensión de negocio la originó;
- qué alternativas fueron descartadas;
- qué evidencia sostuvo una interpretación;
- qué incertidumbres permanecían abiertas;
- o qué historia produjo el estado actual.

Por eso, generar una referencia desde VSIR puede ser útil, pero regenerar toda la documentación de continuidad desde VSIR no sería equivalente a recuperar el conocimiento original.

## Mapa comparativo

| Effect | VSlices | Relación aproximada |
| --- | --- | --- |
| `Effect<A, E, R>` | `Flow<RT, REQ, A>` y modelo de Feature | Ambos hacen explícitos requisitos de ejecución y resultados effectful; VSlices separa request y runtime. |
| `Context` / services | Runtime capabilities | Ambos modelan capacidades requeridas por una ejecución. |
| `Layer` | Responsabilidad de Deploy / runtime assembly | `Layer` es un precedente para composición de runtime; Deploy cubre un espacio mayor. |
| `Schema` / Schema AST | Documentación semántica + VSIR | Existe un paralelo en la interpretabilidad, pero la procedencia es distinta. |
| Schema transformations | `Trait Transform` | VSlices trata transform como transporte validable entre espacios semánticos, no sólo como codec. |
| Typed errors / `Cause` | LanguageExt `Error` + `IO` en la realización .NET | La realización .NET ya distingue errores esperados, excepcionales y múltiples. |
| `Schedule` | Execution policies | Effect es un precedente útil para políticas de retry, repeat y scheduling como datos. |
| `ExecutionPlan` | Feature orchestration | Área compatible con prototipos y direcciones ya exploradas en VSlices. |
| Fibers / structured concurrency | Ejecución concurrente de Features | Área de investigación especialmente relevante. |
| `Request` / `RequestResolver` | Ports y estrategias físicas de ejecución | Precedente para separar intención semántica de resolución física, incluyendo batching. |
| Test services | Runtime capabilities reemplazables | Compatible con runtimes deterministas para tiempo, random y otras dependencias. |

La tabla muestra afinidades, no equivalencias exactas.

## Schema AST y VSIR

Effect ofrece una demostración práctica de una idea importante: cuando suficiente semántica se reifica en una representación inspeccionable, múltiples comportamientos pueden derivarse de ella.

Eso es valioso para VSIR.

Sin embargo, la dirección causal debe preservarse.

Una simplificación de Effect puede representarse como:

```text
Schema
  ↓
Schema AST
  ├── validation
  ├── codec
  ├── arbitrary generation
  ├── formatting
  └── other interpretations
```

En VSlices, la trayectoria esperada es más cercana a:

```text
Documentation / Continuity
  ↓
VSIR
  ├── invariants
  ├── lowering
  ├── tests
  ├── compatibility analysis
  ├── derived references
  └── other interpretations
```

Por ello, el precedente no es que VSIR deba convertirse en la fuente original de toda la semántica.

El precedente es que una representación semántica downstream puede soportar múltiples intérpretes sin perder su relación con el conocimiento que la originó.

## Transformaciones

Effect distingue varios tipos de transformaciones en su sistema de Schema.

VSlices no necesita necesariamente copiar esa taxonomía.

`Trait Transform` ya puede representar de forma más general un transporte validable entre espacios semánticos.

La inspiración útil es investigar propiedades del transporte, por ejemplo:

- totalidad o parcialidad;
- reversibilidad;
- determinismo;
- conservación de información;
- colisiones;
- representabilidad;
- round-trip;
- y conservación semántica.

Estas propiedades pueden justificar leyes y pruebas sin multiplicar innecesariamente las primitivas del lenguaje.

## Error handling

Effect conserva una distinción fuerte entre fallos esperados y defectos inesperados y mantiene información adicional sobre causas e interrupciones de ejecución.

La realización .NET de VSlices ya se apoya en LanguageExt, cuyo `Error` distingue errores `Expected`, `Exceptional` y `ManyErrors`, además de errores predefinidos como cancelación y timeout.

Por ello, Effect no revela actualmente una necesidad de introducir un segundo sistema de errores en VSlices.

La pregunta abierta más interesante aparece en concurrencia: si varias ramas fallan al mismo tiempo, puede ser útil investigar si necesitamos conservar no sólo una colección de errores, sino también la topología causal de esos fallos.

Esa necesidad debe demostrarse antes de agregar una abstracción nueva.

## Layer y Deploy

`Layer` es un precedente sólido para construir, componer y compartir servicios necesarios por un programa.

VSlices ubica esa responsabilidad dentro de un concepto más amplio: Deploy.

Una Feature declara qué capacidades necesita.

Un Deploy decide cómo materializarlas.

```text
Feature
    requires capability

Deploy
    chooses provider
    chooses construction
    chooses lifetime
    chooses sharing
    chooses disposal
    chooses hosting/runtime topology
```

Esto evita que una Feature tenga que declarar detalles como `Scoped`, `Singleton` o `Transient` cuando esos detalles pertenecen al ensamblaje de runtime.

Si una Feature requiere una garantía semántica, por ejemplo que varias operaciones participen en una misma transacción, esa garantía debería expresarse como capacidad o contrato semántico. El Deploy puede decidir cómo materializarla.

## Policies como datos

Effect modela scheduling, retry y otros comportamientos de ejecución mediante valores componibles.

VSlices ya reconoce como dirección futura políticas de ejecución para Features, incluyendo ejecución en background, ejecución temporal y orquestaciones durables.

Effect resulta útil como precedente para estudiar preguntas como:

- qué políticas componen;
- qué política domina ante conflicto;
- qué errores activan retry o fallback;
- cómo se propaga cancellation;
- cómo interactúan timeout y retry;
- qué se observa y registra;
- y si una política puede cambiar los requisitos de runtime.

La existencia de una solución madura en Effect no obliga a copiar su API. Permite utilizarla como corpus de decisiones arquitectónicas contra el cual contrastar diseños de VSlices.

## Structured concurrency

La concurrencia estructurada es una de las áreas donde Effect ofrece un precedente especialmente útil.

Para VSlices conviene distinguir al menos dos ejes:

```text
Execution topology
    structured ←→ detached

Durability
    ephemeral  ←→ durable
```

Esto evita usar palabras como "background" para promesas muy diferentes.

Por ejemplo:

- un child task puede ser `structured + ephemeral`;
- un fire-and-forget puede ser `detached + ephemeral`;
- un job persistido puede ser `detached + durable`;
- una orchestration durable puede conservar ownership lógico aunque sobreviva al proceso que la inició.

Las leyes relevantes incluyen ownership, cancellation, completion, failure propagation, resource lifetime y durability.

## Requests declarativas y Ports

Effect incluye un modelo de `Request` y `RequestResolver` que permite separar qué dato se necesita de cómo se obtiene físicamente, habilitando estrategias como batching.

La idea relevante para VSlices es más amplia que el batching:

> separar la intención semántica de una interacción de su estrategia física de ejecución cuando esa separación produce valor.

Una futura investigación sobre Ports podría evaluar si ciertas operaciones deben poder representarse como requests declarativas que un runtime pueda:

- agrupar;
- cachear;
- deduplicar;
- paralelizar;
- resolver local o remotamente;
- o materializar mediante distintas infraestructuras.

Esto permanece como investigación, no como requisito actual del Framework.

## Continuidad y lineage

La diferencia más importante vuelve a aparecer en provenance.

Effect intenta preservar semántica durante la composición y ejecución de programas.

VSlices intenta preservar significado durante la vida y evolución del software.

Una trayectoria futura de lineage puede verse así:

```text
Business / Domain Knowledge
        ↓
Documentation
        ↓
Semantic assertion
        ↓
VSIR
        ↓
Lowered artifact
        ↓
Runtime behavior
        ↓
Validation evidence
        ↓
Updated understanding
```

Esta trayectoria no debe asumir que una representación posterior puede reconstruir perfectamente todas las anteriores.

Debe conservar suficiente provenance para navegar de una consecuencia ejecutable hacia el conocimiento que la justificó.

## Qué aprender de Effect

Effect es valioso para VSlices como precedente porque muestra que varias preocupaciones tradicionalmente dispersas pueden convivir bajo una semántica coherente.

Entre las áreas más útiles para estudiar se encuentran:

- composición de efectos;
- requisitos de runtime;
- construcción de servicios;
- resource management;
- policies como datos;
- structured concurrency;
- schemas interpretables;
- requests declarativas;
- testing determinista;
- observability integrada.

VSlices puede reutilizar las preguntas que Effect ya tuvo que responder sin asumir que deba reutilizar las mismas respuestas.

## Qué no implica esta comparación

Esta comparación no implica que:

- VSlices deba copiar Effect;
- Effect sea una dependencia requerida;
- Effect sea el origen histórico de VSlices;
- VSIR deba convertirse en un clon de Schema AST;
- VSlices necesite una abstracción `Layer` propia;
- VSlices necesite otro sistema de `Cause` o `Exit`;
- toda Feature deba declarar resource lifetime;
- batching deba implementarse antes de existir un problema real;
- o que VSlices ya tenga la misma madurez ejecutable de Effect.

El valor del precedente está en disponer de una realización madura contra la cual contrastar decisiones presentes y futuras.

## Conclusión

Effect y VSlices convergen en una parte importante del problema de construir software ejecutable con semántica explícita.

Effect ha materializado muchas de esas preocupaciones en un application foundation coherente.

VSlices persigue una continuidad más amplia: intenta conectar el problema, el conocimiento, la documentación, el diseño, la representación semántica, la ejecución, la verificación y la evolución.

Por eso Effect puede parecer una arquitectura madre cuando se observa sólo el código.

Cuando se observa el sistema completo de conocimiento, su papel cambia: deja de ser un molde y se convierte en uno de los precedentes más valiosos para estudiar la superficie ejecutable de VSlices.

## Referencias

- [Effect](https://effect.website/)
- [Effect v4 installation](https://effect.website/docs/v4/getting-started/installation)
- [Effect v4 Schema](https://effect.website/docs/v4/schema/getting-started)
- [Effect v4 Schema annotations](https://effect.website/docs/v4/schema/annotations)
- [Effect v4 batching](https://effect.website/docs/v4/batching)
- [Effect repository](https://github.com/Effect-TS/effect)
- [LanguageExt error handling](https://github.com/louthy/language-ext/wiki/How-to-handle-errors-in-a-functional-way)
- [LanguageExt built-in errors](https://github.com/louthy/language-ext/blob/main/LanguageExt.Core/Common/Errors.cs)
