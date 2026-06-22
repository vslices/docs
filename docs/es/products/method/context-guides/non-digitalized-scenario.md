# Escenario "No digitalizado"

Un escenario "No digitalizado" es un contexto de trabajo donde el trabajo importante todavía no está representado por software.

El trabajo puede ocurrir mediante conversaciones, hojas de cálculo, documentos en papel, mensajes, reuniones, coordinación manual o rutinas informales.

Esto no significa que el trabajo sea simple. Significa que el conocimiento necesario para apoyarlo puede seguir siendo implícito, distribuido o inestable.

## Idea central

!!! principle "Principio de continuidad"

    En un escenario no digitalizado, VSlices Method ayuda al equipo a entender cómo ocurre actualmente el trabajo antes de decidir qué debería convertirse en software.

El objetivo no es documentarlo todo. Es descubrir suficiente contexto de dominio, proceso y decisión para evitar automatizar una realidad mal entendida.

## Cuándo aplica esta guía

Usa esta guía cuando:

* ningún software soporta actualmente el trabajo
* el software existente no está relacionado con el trabajo que se está estudiando
* el trabajo se coordina manualmente
* el conocimiento vive principalmente en personas, documentos o hábitos
* los flujos de trabajo son informales o inconsistentes
* distintas personas explican el mismo trabajo de forma diferente
* se le pide al equipo crear un nuevo sistema, módulo o capacidad desde cero

Esta guía puede aplicarse a un proyecto completo, una línea de trabajo o una sola área de comportamiento de negocio.

## Riesgo principal

El riesgo principal es automatizar un proceso que el equipo todavía no entiende.

Un escenario no digitalizado puede contener:

* reglas implícitas
* responsabilidades informales
* excepciones manejadas por memoria
* lenguaje que cambia entre personas
* decisiones ocultas en hábitos
* validaciones manuales
* workarounds que revelan restricciones reales
* pasos de proceso que existen solo porque no hay mejor soporte


!!! risk "Riesgo a evitar"

    Si el equipo comienza a diseñar software demasiado temprano, puede convertir hábitos temporales en comportamiento permanente del sistema.

## Modalidad inicial útil

Un escenario no digitalizado normalmente comienza con [**Context-First**](../../design/modalities/context-first/index.md), porque el equipo todavía necesita entender cómo ocurre el trabajo antes de decidir qué debería convertirse en software.

| Situación                                                                     | Modalidad útil    | Razón                                                                                |
| ----------------------------------------------------------------------------- | ----------------- | ------------------------------------------------------------------------------------ |
| El equipo no entiende cómo ocurre actualmente el trabajo.                     | **Context-First** | La siguiente decisión necesita una comprensión más amplia del dominio y del proceso. |
| Existe un dolor claro dentro del trabajo manual.                              | [**Problem-First**](../../design/modalities/problem-first/index.md) | El equipo puede enfocarse en entender el problema sin asumir la solución.            |
| Un experimento pequeño puede revelar cómo las personas reaccionan al soporte. | [**Slice-First**](../../design/modalities/slice-first/index.md)   | El equipo puede aprender mediante un prototipo acotado o una vertical slice.         |

!!! risk "Riesgo a evitar"

    Slice-First debe usarse con cuidado en este escenario.

    Una slice pequeña es útil solo cuando ayuda a aprender sin fingir que todo el contexto ya se entiende.


## Qué observar primero

Antes de diseñar software, observa cómo las personas realizan actualmente el trabajo.

| Observa                                                   | Para entender                                                                |
| --------------------------------------------------------- | ---------------------------------------------------------------------------- |
| Quién participa en el trabajo                             | Qué roles, personas o áreas sostienen el proceso.                            |
| Qué activa el trabajo                                     | Qué evento, necesidad o decisión inicia el proceso.                          |
| Qué resultado se espera                                   | Qué significa que el trabajo haya terminado correctamente.                   |
| Qué pasos se repiten                                      | Qué comportamiento podría necesitar estructura estable.                      |
| Qué cambia de un caso a otro                              | Qué variaciones no deberían perderse al digitalizar.                         |
| Qué términos usan las personas                            | Qué lenguaje de dominio debería preservarse.                                 |
| Dónde ocurren retrasos, errores o malentendidos           | Qué fricciones revelan riesgos reales.                                       |
| Qué decisiones se toman durante el trabajo                | Qué conocimiento no debería quedar implícito.                                |
| Qué validaciones se realizan manualmente                  | Qué reglas podrían necesitar hacerse explícitas.                             |
| Qué excepciones son comunes                               | Qué casos especiales deberían entenderse temprano.                           |
| Qué información se crea, transforma o comparte            | Qué datos sostienen el trabajo.                                              |
| Qué partes existen solo porque no hay soporte de software | Qué hábitos podrían ser temporales y no deberían automatizarse sin revisión. |

El objetivo no es modelar perfectamente el proceso. Es encontrar suficiente estructura para tomar la siguiente decisión con más seguridad.

## Conocimiento a preservar

Preserva conocimiento cuando afecte lo que debería construirse, evitarse o investigarse después.

El conocimiento útil puede incluir:

* términos del dominio y significados en conflicto
* actores y responsabilidades
* flujos de trabajo actuales
* problemas recurrentes
* decisiones manuales
* validaciones y errores esperados
* excepciones importantes
* reglas de negocio ocultas en la rutina
* documentos, hojas de cálculo o mensajes usados como herramientas de coordinación
* preguntas abiertas e incertidumbre

!!! principle "Principio de continuidad"

    No guardes cada observación.
  
    Preserva lo que el trabajo futuro no debería tener que redescubrir.


## Apoyo documental

Los documentos pueden ayudar a hacer visible el trabajo implícito.

| Necesidad de conocimiento | Documento útil |
| --- | --- |
| Las personas usan términos de forma inconsistente. | Domain Vocabulary — [Taxonomy](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md) |
| El escenario circundante necesita entenderse. | Context Document — [Taxonomy](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md) |
| El trabajo depende de pasos, handoffs o responsabilidades. | Process Document — [Taxonomy](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md) |
| Un comportamiento debería ser soportado por software. | Use Case Document — [Taxonomy](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md) |
| Está emergiendo una habilidad estable del negocio. | Capability Document — [Taxonomy](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Debe elegirse una dirección bajo tradeoffs. | Decision Record — [Taxonomy](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md) |
| Evidencia temprana cambia lo que el equipo cree. | Validation Note — [Taxonomy](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md) |
| Las observaciones todavía son inciertas, locales o temporales. | Support Note — [Taxonomy](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md) |

Usa documentos para preservar entendimiento, no para formalizar todo demasiado temprano.

{% include-markdown "shared/readings/document-stage-affinity-admonition.md" %}

## Enfoque sugerido

Comienza eligiendo un área de trabajo para entender.

No intentes modelar toda la organización primero. Un enfoque útil es:

1. Identificar el escenario o línea de trabajo que se está explorando.
2. Observar cómo ocurre el trabajo hoy.
3. Capturar lenguaje, actores, flujos de trabajo, decisiones e incertidumbre.
4. Identificar dolores, riesgos u oportunidades que se repiten.
5. Guardar solo el conocimiento necesario para la siguiente decisión responsable.
6. Decidir la siguiente modalidad útil: seguir entendiendo el contexto, aclarar un problema o construir una slice pequeña.
7. Usar feedback para actualizar el contexto compartido.

El equipo debería avanzar gradualmente desde la observación hacia la decisión.

## Errores comunes

Los escenarios no digitalizados suelen fallar cuando los equipos saltan desde la conversación hacia la solución.

Algunos errores comunes incluyen:

* diseñar pantallas antes de entender el trabajo
* tratar la explicación de una sola persona como si fuera todo el proceso
* ignorar excepciones porque parecen raras
* automatizar hábitos manuales que deberían mejorarse en vez de copiarse
* asumir que el trabajo informal no tiene estructura
* documentarlo todo antes de decidir algo
* construir un sistema completo antes de validar una parte pequeña
* usar conceptos de software antes de que el lenguaje del dominio esté claro


!!! risk "No confundas evidencia con diseño"

    El trabajo manual muestra cómo opera la realidad actual.
    No significa que esa realidad deba copiarse tal cual en software.

## Principio guía

!!! principle "Principio de continuidad"

    Entiende el trabajo antes de representarlo.

    Preserva suficiente contexto, lenguaje, proceso y conocimiento de decisión para evitar convertir hábitos temporales en software permanente.

Construye solo cuando el equipo pueda explicar qué realidad el software debería apoyar o mejorar.

