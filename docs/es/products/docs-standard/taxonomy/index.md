# Taxonomía

VSlices Docs Standard organiza los documentos según el tipo de conocimiento que preservan.

El objetivo de esta taxonomía es ayudar a los equipos a elegir el documento correcto según lo que necesitan proteger de perderse.

Esta taxonomía no define un flujo de trabajo. No dice qué documento debe crearse primero. Solo explica para qué tipo de conocimiento es más adecuado cada documento.

## Idea central

Los distintos documentos preservan distintos tipos de conocimiento.

Cualquier equipo debería hacer un cambio de enfoque al usar VSlices Docs Standard:

> ¿Qué documento requiere el proceso? -> ¿Qué tipo de conocimiento estamos intentando preservar?

Porque, si el equipo necesita preservar

- lenguaje, puede necesitar un Vocabulario de dominio.
- dónde ocurre el trabajo, puede necesitar un Documento de contexto.
- cómo se realiza el trabajo, puede necesitar un Documento de proceso.
- qué significa el comportamiento, puede necesitar un Documento de caso de uso.
- qué debe ser posible, puede necesitar un Documento de capacidad.
- por qué se eligió una dirección, puede necesitar un Registro de decisión.
- qué se aprendió, puede necesitar una Nota de validación.

Pero también, si el conocimiento sigue siendo temprano, incierto, local o temporal, puede que solo necesite una Nota de soporte.

## Taxonomía de documentos

| Knowledge preserved | Document | Main question | Examples |
| --- | --- | --- | --- |
| Language | Domain Vocabulary | What does this mean? | Terms, aliases, conflicting meanings, examples |
| Scenario | Context Document | Where are we working? | Organization, area, actors, boundaries, pain points |
| Work line | Context Document | What do we offer or operate? | Departments, services, business lines, value streams |
| Work process | Process Document | How do we do it? | Responsibilities, roles, coordination, operational structure |
| Workflow | Process Document | What is done? | Steps, _handoffs_, decisions, responsible participants |
| Behavior | Use Case Document | What does this behavior mean? | Consequences, validations, expected errors, rules |
| Ability | Capability Document | What must be possible? | Stable business or system abilities |
| Decision | Decision Record | Why did we choose this? | Options, rationale, tradeoffs, consequences |
| Learning | Validation Note | What did we learn? | Evidence, results, _feedback_, next questions |
| Emerging knowledge | Support Note | What should we not lose yet? | Concepts, assumptions, risks, questions, feedback |

## Taxonomy groups

Los documentos también pueden entenderse como grupos.

* **Documentos orientados al lenguaje**: preservan términos y significados que apoyan el entendimiento compartido.
* **Documentos orientados al contexto**: preservan scenarios y work lines para que las decisiones posteriores no queden aisladas.
* **Documentos orientados a la operación**: preservan work processes y workflows para que la implementación refleje cómo se realiza el trabajo.
* **Documentos orientados al comportamiento**: preservan use cases para que acciones, consecuencias, validaciones y errores sigan siendo explícitos.
* **Documentos orientados a la capacidad**: preservan capacidades estables antes de que se conviertan en estructura de implementación.
* **Documentos orientados a la decisión**: preservan razonamiento, tradeoffs y consecuencias aceptadas.
* **Documentos orientados al aprendizaje**: preservan validación, feedback y evidencia recopilada después de revisiones o implementación.
* **Documentos de soporte**: preservan conocimiento temprano o incierto antes de que gane más estructura.

## Cómo elegir un documento

Usa el documento más pequeño que preserve el conocimiento del que depende el trabajo futuro.

* **Usa Vocabulario de dominio** cuando el lenguaje pueda afectar el entendimiento, el comportamiento, el nombrado o los límites.
* **Usa Documento de contexto** cuando el equipo necesite preservar el scenario, los work lines, los actores o la situación circundante.
* **Usa Documento de proceso** cuando importen las responsabilidades, la coordinación, los workflows, los _handoffs_ o las reglas operativas.
* **Usa Documento de caso de uso** cuando el comportamiento necesite significado explícito, consecuencias, validaciones o errores esperados.
* **Usa Documento de capacidad** cuando varios comportamientos o procesos dependan de una capacidad estable.
* **Usa Registro de decisión** cuando una elección tenga _tradeoffs_, consecuencias o impacto futuro significativos.
* **Usa Nota de validación** cuando la evidencia cambie o confirme conocimiento del que dependerá el trabajo futuro.
* **Usa Nota de soporte** cuando el conocimiento sea útil pero todavía temprano, incierto, local o temporal.

## Principio de la taxonomía

La taxonomía sigue un principio:

> Elige los documentos por el conocimiento que preservan, no por la ceremonia que sugieren.

Un documento es útil cuando protege la continuidad. Si el conocimiento puede preservarse con un artefacto más pequeño, usa el artefacto más pequeño.
