# Afinidad documento-etapa

La afinidad documento-etapa explica cómo los documentos de VSlices Docs Standard pueden apoyar cada etapa de una iteración de VSlices Design.

!!! principle "Principio de Documentación"

    La afinidad documento-etapa ayuda a elegir documentación útil según la etapa de trabajo.

    No convierte los documentos en requisitos obligatorios ni transforma VSlices Method en una checklist.

Esta página usa el siguiente flujo base de iteración:

<p class="vslices-diagram-caption">Flujo base de iteración usado para organizar la afinidad documental.</p>

{% include-markdown "shared/simple-design-iteration-flow.md" %}

## Idea central

Cada etapa crea o cambia un tipo distinto de conocimiento.

Algunos documentos apoyan naturalmente mejor unas etapas que otras, pero esta afinidad es solo una guía. Un equipo puede crear, actualizar, omitir, fusionar o revisitar documentos cuando la iteración lo requiera.

!!! principle "Principio de Documentación"

    La pregunta no es _¿qué documentos requiere esta etapa?_, sino _¿qué conocimiento necesitamos preservar para tomar la siguiente decisión responsable?_


## Afinidad por etapa

| Etapa | Conocimiento que se está manejando | Documentos útiles | Riesgo principal que evita |
| --- | --- | --- | --- |
| **Understanding** | Señales tempranas del dominio, lenguaje, supuestos, riesgos y preguntas abiertas. | **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**, **[Context Document](../docs-standard/taxonomy/context-document.md)** temprano. | Diseñar artefactos de software antes de entender el mundo al que pertenecen. |
| **Contextualizing** | Escenario, actores, límites, work lines, workflows y contexto circundante. | **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Domain Vocabulary](../docs-standard/taxonomy/domain-vocabulary.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Tratar un problema, caso de uso o feature como si estuviera aislado de su contexto. |
| **Planning** | Mejora esperada, comportamiento, capacidades, alcance, decisiones y tradeoffs. | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Resolver un problema técnico atractivo en vez del problema de negocio relevante. |
| **Building** | Comportamiento de implementación, validaciones, errores esperados, restricciones y feedback de entrega. | **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Capability Document](../docs-standard/taxonomy/capability-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Tratar la implementación como el final del aprendizaje. |
| **Returning to Understanding** | Evidencia, aprendizaje, supuestos modificados, contexto actualizado y nueva incertidumbre. | **[Validation Note](../docs-standard/taxonomy/validation-note.md)**, **[Context Document](../docs-standard/taxonomy/context-document.md)**, **[Process Document](../docs-standard/taxonomy/process-document.md)**, **[Use Case Document](../docs-standard/taxonomy/use-case-document.md)**, **[Decision Record](../docs-standard/taxonomy/decision-record.md)**, **[Support Note](../docs-standard/taxonomy/support-note.md)**. | Ignorar lo que el sistema enseñó después de ser construido. |

## Afinidad por documento

Un mismo documento puede apoyar más de una etapa.

| Documento | Afinidad más fuerte | Útil cuando |
| --- | --- | --- |
| [**Domain Vocabulary**](../docs-standard/taxonomy/domain-vocabulary.md) | Understanding y Contextualizing. | Aparece lenguaje, cambia, entra en conflicto o se vuelve importante para tomar decisiones. |
| [**Context Document**](../docs-standard/taxonomy/context-document.md) | Contextualizing. | El equipo necesita preservar el escenario, los actores, los límites o la situación actual. |
| [**Process Document**](../docs-standard/taxonomy/process-document.md) | Contextualizing. | El trabajo depende de responsabilidades, workflows, handoffs u operaciones repetidas. |
| [**Use Case Document**](../docs-standard/taxonomy/use-case-document.md) | Planning y Building. | El comportamiento, las consecuencias, las validaciones o los errores esperados deben guiar la implementación. |
| [**Capability Document**](../docs-standard/taxonomy/capability-document.md) | Planning y Building. | Una habilidad estable del negocio o del sistema necesita ser nombrada y preservada. |
| [**Decision Record**](../docs-standard/taxonomy/decision-record.md) | Planning y Building. | Una dirección, tradeoff, riesgo aceptado u opción rechazada puede afectar trabajo futuro. |
| [**Validation Note**](../docs-standard/taxonomy/validation-note.md) | Building y Returning to Understanding. | La evidencia desde implementación, revisión, uso u operación cambia lo que el equipo sabe. |
| [**Support Note**](../docs-standard/taxonomy/support-note.md) | Todas las etapas. | El conocimiento es útil, pero todavía es temprano, local, incierto o temporal. |

## Uso de la afinidad

La afinidad documental debería ayudar al equipo a decidir qué conocimiento preservar. No debería decidir por el equipo.

Usa un documento cuando ayude al equipo a:

* aclarar lenguaje
* preservar contexto
* explicar comportamiento
* hacer visible una decisión
* llevar intención hacia la implementación
* registrar evidencia
* evitar redescubrir el mismo conocimiento más adelante

!!! risk "Riesgo a evitar"

    Omite un documento cuando existe solo porque una etapa parece esperarlo.


## Regla de Method

!!! principle "Usa documentación solo cuando preserve continuidad"

    Usa el documento que preserve el conocimiento necesario para la siguiente decisión responsable.


Si un documento ayuda al equipo a avanzar con más claridad, úsalo.

Si un documento crea ceremonia sin preservar conocimiento útil, omítelo.
