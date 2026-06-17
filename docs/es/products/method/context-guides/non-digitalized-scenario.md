# Escenario "No digitalizado"

Un escenario "No digitalizado" es un contexto de trabajo donde el trabajo importante todavía no está representado por software.

El trabajo puede ocurrir mediante conversaciones, hojas de cálculo, documentos en papel, mensajes, reuniones, coordinación manual o rutinas informales.

Esto no significa que el trabajo sea simple. Significa que el conocimiento necesario para apoyarlo puede seguir siendo implícito, distribuido o inestable.

## Idea central

En un escenario no digitalizado, VSlices Method ayuda al equipo a entender cómo ocurre actualmente el trabajo antes de decidir qué debería convertirse en software.

El objetivo no es documentarlo todo. Es descubrir suficiente contexto de dominio, proceso y decisión para evitar automatizar una realidad mal entendida.

## Cuándo aplica esta guía

Usa esta guía cuando:

* ningún software apoya actualmente el trabajo
* el software existente no está relacionado con el trabajo que se está estudiando
* el trabajo se coordina manualmente
* el conocimiento vive principalmente en personas, documentos o hábitos
* los workflows son informales o inconsistentes
* distintas personas explican el mismo trabajo de forma diferente
* se le pide al equipo crear un nuevo sistema, módulo o capability desde cero

Esta guía puede aplicarse a un proyecto completo, una work line o una sola área de comportamiento de negocio.

## Riesgo principal

El riesgo principal es automatizar un proceso que el equipo no entiende. Un escenario no digitalizado puede contener:

* reglas implícitas
* responsabilidades informales
* excepciones manejadas por memoria
* lenguaje que cambia entre personas
* decisiones ocultas en hábitos
* validaciones manuales
* workarounds que revelan restricciones reales
* pasos de proceso que existen solo porque no hay mejor soporte

Si el equipo comienza diseñando software demasiado temprano, puede convertir hábitos temporales en comportamiento permanente del sistema.

## Modalidad inicial útil

Un escenario no digitalizado normalmente comienza con **Context-First**.

| Situación | Modalidad | Razón |
| --- | --- | --- |
| El equipo no entiende cómo ocurre actualmente el trabajo. | [**Context-First**](../../design/modalities/context-first/index.md) | La siguiente decisión necesita una comprensión más amplia del dominio y del proceso. |
| Existe un dolor claro dentro del trabajo manual. | [**Problem-First**](../../design/modalities/problem-first/index.md) | El equipo puede enfocarse en entender el problema sin asumir la solución. |
| Un experimento pequeño puede revelar de forma segura cómo las personas reaccionan al soporte. | [**Slice-First**](../../design/modalities/slice-first/index.md) | El equipo puede aprender mediante un prototipo acotado o una vertical slice. |

Slice-First debería usarse con cuidado. Una slice pequeña es útil solo cuando ayuda a aprender sin fingir que todo el contexto ya se entiende.

## Qué observar primero

Antes de diseñar software, observa cómo las personas realizan actualmente el trabajo. Algunas preguntas útiles son:

* ¿Quién participa en el trabajo?
* ¿Qué activa el trabajo?
* ¿Qué resultado se espera?
* ¿Qué pasos se repiten?
* ¿Qué cambia de un caso a otro?
* ¿Qué términos usan las personas?
* ¿Dónde ocurren retrasos, errores o malentendidos?
* ¿Qué decisiones se toman durante el trabajo?
* ¿Qué validaciones se realizan manualmente?
* ¿Qué excepciones son comunes?
* ¿Qué información se crea, transforma o comparte?
* ¿Qué partes del trabajo existen solo porque no hay soporte de software?

El objetivo no es modelar perfectamente el proceso. Es encontrar suficiente estructura para tomar la siguiente decisión con más seguridad.

## Conocimiento a preservar

Preserva conocimiento cuando afecte lo que debería construirse, evitarse o investigarse después. El conocimiento útil puede incluir:

* términos del dominio y significados en conflicto
* actores y responsabilidades
* workflows actuales
* problemas repetidos
* decisiones manuales
* validaciones y errores esperados
* excepciones importantes
* reglas de negocio ocultas en la rutina
* documentos, hojas de cálculo o mensajes usados como herramientas de coordinación
* preguntas abiertas e incertidumbre

No preserves cada observación. Preserva lo que el trabajo futuro no debería tener que redescubrir.

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

> La afinidad documental por etapa de iteración se describe en la página [Afinidad documento-etapa](../document-stage-affinity.md).

## Enfoque sugerido

Comienza eligiendo un área de trabajo para entender.

No intentes modelar toda la organización primero. Un enfoque útil es:

1. Identificar el escenario o work line que se está explorando.
2. Observar cómo ocurre el trabajo hoy.
3. Capturar lenguaje, actores, workflows, decisiones e incertidumbre.
4. Identificar dolor, riesgo u oportunidad repetida.
5. Preservar solo el conocimiento necesario para la siguiente decisión responsable.
6. Elegir si continuar entendiendo, aclarar un problema o construir una slice pequeña.
7. Usar feedback para actualizar el contexto compartido.

El equipo debería avanzar gradualmente desde la observación hacia la decisión.

## Errores comunes

Los escenarios no digitalizados suelen fallar cuando los equipos saltan desde la conversación hacia la solución. Algunos errores comunes incluyen:

* diseñar pantallas antes de entender el trabajo
* tratar la explicación de una sola persona como si fuera todo el proceso
* ignorar excepciones porque parecen raras
* automatizar hábitos manuales que deberían mejorarse en vez de copiarse
* asumir que el trabajo informal no tiene estructura
* documentarlo todo antes de decidir algo
* construir un sistema completo antes de validar una parte pequeña
* usar conceptos de software antes de que el lenguaje del dominio esté claro

El trabajo manual debería respetarse como evidencia. No debería copiarse ciegamente en software.

## Principio guía

Entiende el trabajo antes de representarlo.

Preserva suficiente contexto, lenguaje, proceso y conocimiento de decisión para evitar convertir hábitos temporales en software permanente.

Construye solo cuando el equipo pueda explicar qué realidad el software debería apoyar o mejorar.
