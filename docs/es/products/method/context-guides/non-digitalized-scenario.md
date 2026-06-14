# Escenario "No digitalizado"

Los escenarios "No digitalizados" (*Non-Digitalized Scenarios* en inglés) son contextos de trabajo donde trabajo importante todavía no está representado por *software*.

El trabajo puede ocurrir mediante conversaciones, planillas, documentos en papel, mensajes, reuniones, coordinación manual o rutinas informales.

Esto no significa que el trabajo sea simple. Significa que el conocimiento necesario para apoyarlo todavía puede ser implícito, distribuido o inestable.

## Idea central

En un escenario no digitalizado, *VSlices Method* ayuda al equipo a entender cómo ocurre actualmente el trabajo antes de decidir qué debería convertirse en *software*.

El objetivo no es documentarlo todo. Es descubrir suficiente contexto de dominio, proceso y decisión para evitar automatizar una realidad mal entendida.

## Cuándo aplica esta guía

Usa esta guía cuando:

* actualmente no hay *software* que apoye el trabajo
* el *software* existente no está relacionado con el trabajo que se está estudiando
* el trabajo se coordina manualmente
* el conocimiento vive principalmente en personas, documentos o hábitos
* los *workflows* son informales o inconsistentes
* distintas personas explican el mismo trabajo de formas distintas
* se le pide al equipo crear un nuevo sistema, módulo o capacidad desde cero

Esta guía puede aplicar a un proyecto completo, una línea de trabajo o un área específica de comportamiento de negocio.

## Riesgo principal

El riesgo principal es automatizar un proceso que el equipo no entiende. Un escenario no digitalizado puede contener:

* reglas implícitas
* responsabilidades informales
* excepciones manejadas de memoria
* lenguaje que cambia entre personas
* decisiones ocultas en hábitos
* validaciones manuales
* *workarounds* que revelan restricciones reales
* pasos de proceso que existen solo porque no hay mejor soporte

Si el equipo comienza diseñando *software* demasiado pronto, puede convertir hábitos temporales en comportamiento permanente del sistema.

## Modalidad inicial útil

Un escenario no digitalizado normalmente comienza con *Context-First*.

| Situación                                                                                     | Modalidad                                                             | Razón                                                                                 |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| El equipo no entiende cómo<br/>ocurre actualmente el trabajo.                                     | [***Context-First***](../../design/modalities/context-first/index.md) | La siguiente decisión necesita un entendimiento<br/>más amplio del dominio y del proceso. |
| Existe un dolor claro dentro<br/>del trabajo manual.                                              | [***Problem-First***](../../design/modalities/problem-first/index.md) | El equipo puede enfocarse en entender el<br/>problema sin asumir la solución.             |
| Un experimento pequeño<br/>puede revelar de forma<br/>segura cómo reaccionan las<br/>personas al soporte. | [***Slice-First***](../../design/modalities/slice-first/index.md)     | El equipo puede aprender mediante un<br/>prototipo o vertical slice acotada.              |

*Slice-First* debería usarse con cuidado. Una slice pequeña es útil solo cuando ayuda a aprender sin fingir que todo el contexto está entendido.

## Qué observar primero

Antes de diseñar *software*, observa cómo las personas realizan actualmente el trabajo. Algunas preguntas útiles incluyen:

* ¿Quién participa en el trabajo?
* ¿Qué dispara el trabajo?
* ¿Qué resultado se espera?
* ¿Qué pasos se repiten?
* ¿Qué cambia de caso a caso?
* ¿Qué términos usan las personas?
* ¿Dónde ocurren retrasos, errores o malentendidos?
* ¿Qué decisiones se toman durante el trabajo?
* ¿Qué validaciones se realizan manualmente?
* ¿Qué excepciones son comunes?
* ¿Qué información se crea, transforma o comparte?
* ¿Qué partes del trabajo existen solo porque no hay soporte de *software*?

El objetivo no es modelar perfectamente el proceso. Es encontrar suficiente estructura para hacer más segura la siguiente decisión.

## Conocimiento a preservar

Preserva conocimiento cuando afecta qué debería construirse, evitarse o investigarse después. El conocimiento útil puede incluir:

* términos de dominio y significados en conflicto
* actores y responsabilidades
* *workflows* actuales
* problemas repetidos
* decisiones manuales
* validaciones y errores esperados
* excepciones importantes
* reglas de negocio ocultas en la rutina
* documentos, planillas o mensajes usados como herramientas de coordinación
* preguntas abiertas e incertidumbre

No preserves cada observación. Preserva lo que el trabajo futuro no debería tener que redescubrir.

## Soporte documental

Los documentos pueden ayudar a hacer visible el trabajo implícito.

| Necesidad de conocimiento                                      | Documento útil                                                                                                                                                                                                      |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Las personas usan términos de<br/>forma inconsistente.             | Vocabulario de dominio — [Taxonomía](../../docs-standard/taxonomy/domain-vocabulary.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)       |
| El escenario circundante<br/>necesita entenderse.                  | Documento de contexto — [Taxonomía](../../docs-standard/taxonomy/context-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)           |
| El trabajo depende de pasos,<br/>*handoffs* o responsabilidades.   | Documento de proceso — [Taxonomía](../../docs-standard/taxonomy/process-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)            |
| Un comportamiento debería ser<br/>apoyado por *software*.          | Documento de caso de uso — [Taxonomía](../../docs-standard/taxonomy/use-case-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/use-case-document.md)     |
| Está emergiendo una capacidad<br/>estable de negocio.              | Documento de capacidad — [Taxonomía](../../docs-standard/taxonomy/capability-document.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md) |
| Debe elegirse una dirección bajo<br/>*tradeoffs*.                  | Registro de decisión — [Taxonomía](../../docs-standard/taxonomy/decision-record.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/decision-record.md)               |
| Evidencia temprana cambia lo<br/>que el equipo cree.               | Nota de validación — [Taxonomía](../../docs-standard/taxonomy/validation-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/validation-note.md)                 |
| Las observaciones todavía son<br/>inciertas, locales o temporales. | Nota de soporte — [Taxonomía](../../docs-standard/taxonomy/support-note.md) · [Template](https://github.com/vslices/docs-standard/blob/main/templates/support-note.md)                             |

Usa documentos para preservar entendimiento, no para formalizarlo todo demasiado pronto.

> La afinidad documento-etapa (*Document-Stage affinity*) se describe en la página [afinidad documento-etapa](../document-stage-affinity.md).

## Enfoque sugerido

Comienza eligiendo un área de trabajo a entender.

No intentes modelar toda la organización primero. Un enfoque útil es:

1. Identificar el escenario o línea de trabajo que se está explorando.
2. Observar cómo ocurre el trabajo hoy.
3. Capturar lenguaje, actores, *workflows*, decisiones e incertidumbre.
4. Identificar dolor, riesgo u oportunidad repetida.
5. Preservar solo el conocimiento necesario para la siguiente decisión responsable.
6. Elegir si continuar entendiendo, clarificar un problema o construir una slice pequeña.
7. Usar *feedback* para actualizar el contexto compartido.

El equipo debería moverse gradualmente desde la observación hacia la decisión.

## Errores comunes

Los escenarios no digitalizados suelen fallar cuando los equipos se apresuran desde la conversación hacia la solución. Algunos errores comunes incluyen:

* diseñar pantallas antes de entender el trabajo
* tratar la explicación de una persona como el proceso completo
* ignorar excepciones porque parecen raras
* automatizar hábitos manuales que deberían mejorarse en vez de copiarse
* asumir que el trabajo informal no tiene estructura
* documentarlo todo antes de decidir cualquier cosa
* construir un sistema completo antes de validar una parte pequeña
* usar conceptos de *software* antes de que el lenguaje de dominio esté claro

El trabajo manual debería respetarse como evidencia. No debería copiarse ciegamente al *software*.

## Principio guía

Entiende el trabajo antes de representarlo.

Preserva suficiente contexto, lenguaje, proceso y conocimiento de decisión para evitar convertir hábitos temporales en *software* permanente.

Construye solo cuando el equipo pueda explicar qué realidad debería apoyar o mejorar el *software*.
