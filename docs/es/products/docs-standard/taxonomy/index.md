# Taxonomía

VSlices Docs Standard organiza los documentos según el tipo de conocimiento que preservan.

El objetivo de esta taxonomía es ayudar a los equipos a elegir el documento correcto según lo que necesitan proteger de perderse.

Esta taxonomía no define un flujo de trabajo. No dice qué documento debe crearse primero. Solo explica para qué tipo de conocimiento es más adecuado cada documento.

## Idea central

Los distintos documentos preservan distintos tipos de conocimiento.

Cualquier equipo debería hacer un cambio de enfoque al usar VSlices Docs Standard:

> ¿Qué documento requiere el proceso? -> ¿Qué tipo de conocimiento estamos intentando preservar?

Porque, si el equipo necesita preservar

- lenguaje, puede necesitar un Vocabulario de dominio (_Domain Vocabulary_ en inglés).
- dónde ocurre el trabajo, puede necesitar un Documento de contexto (_Context Document_ en inglés).
- cómo se realiza el trabajo, puede necesitar un Documento de proceso (_Process Document_ en inglés).
- qué significa el comportamiento, puede necesitar un Documento de caso de uso (_Use Case Document_ en inglés).
- qué debe ser posible, puede necesitar un Documento de capacidad (_Capability Document_ en inglés).
- por qué se eligió una dirección, puede necesitar un Registro de decisión (_Decision Record_ en inglés).
- qué se aprendió, puede necesitar una Nota de validación (_Validation Note_ en inglés).

Pero también, si el conocimiento sigue siendo temprano, incierto, local o temporal, puede que solo necesite una Nota de soporte (_Support Note_ en inglés).

## Taxonomía de documentos

| Conocimiento preservado | Documento | Pregunta principal | Ejemplos |
| --- | --- | --- | --- |
| Lenguaje | Vocabulario de dominio (_Domain Vocabulary_ en inglés) | ¿Qué significa esto? | Términos, alias, significados en conflicto, ejemplos |
| Scenario | Documento de contexto (_Context Document_ en inglés) | ¿Dónde estamos trabajando? | Organización, área, actores, límites, puntos de dolor |
| Work line | Documento de contexto (_Context Document_ en inglés) | ¿Qué ofrecemos u operamos? | Departamentos, servicios, líneas de negocio, _value streams_ |
| Work process | Documento de proceso (_Process Document_ en inglés) | ¿Cómo lo hacemos? | Responsabilidades, roles, coordinación, estructura operativa |
| Workflow | Documento de proceso (_Process Document_ en inglés) | ¿Qué se hace? | Pasos, _handoffs_, decisiones, participantes responsables |
| Comportamiento | Documento de caso de uso (_Use Case Document_ en inglés) | ¿Qué significa este comportamiento? | Consecuencias, validaciones, errores esperados, reglas |
| Capacidad | Documento de capacidad (_Capability Document_ en inglés) | ¿Qué debe ser posible? | Capacidades estables del negocio o del sistema |
| Decisión | Registro de decisión (_Decision Record_ en inglés) | ¿Por qué elegimos esto? | Opciones, razonamiento, _tradeoffs_, consecuencias |
| Aprendizaje | Nota de validación (_Validation Note_ en inglés) | ¿Qué aprendimos? | Evidencia, resultados, _feedback_, preguntas siguientes |
| Conocimiento emergente | Nota de soporte (_Support Note_ en inglés) | ¿Qué no deberíamos perder todavía? | Conceptos, supuestos, riesgos, preguntas, _feedback_ |

## Grupos de taxonomía

Los documentos también pueden entenderse como grupos.

* **Documentos orientados al lenguaje**: preservan términos y significados que apoyan el entendimiento compartido.
* **Documentos orientados al contexto**: preservan scenarios y work lines para que las decisiones posteriores no queden aisladas.
* **Documentos orientados a la operación**: preservan work processes y _workflows_ para que la implementación refleje cómo se realiza el trabajo.
* **Documentos orientados al comportamiento**: preservan casos de uso para que acciones, consecuencias, validaciones y errores sigan siendo explícitos.
* **Documentos orientados a la capacidad**: preservan capacidades estables antes de que se conviertan en estructura de implementación.
* **Documentos orientados a la decisión**: preservan razonamiento, _tradeoffs_ y consecuencias aceptadas.
* **Documentos orientados al aprendizaje**: preservan validación, _feedback_ y evidencia recopilada después de revisiones o implementación.
* **Documentos de soporte**: preservan conocimiento temprano o incierto antes de que gane más estructura.

## Cómo elegir un documento

Usa el documento más pequeño que preserve el conocimiento del que depende el trabajo futuro.

* **Usa Vocabulario de dominio** cuando el lenguaje pueda afectar el entendimiento, el comportamiento, el nombrado o los límites.
* **Usa Documento de contexto** cuando el equipo necesite preservar el scenario, los work lines, los actores o la situación circundante.
* **Usa Documento de proceso** cuando importen las responsabilidades, la coordinación, los _workflows_, los _handoffs_ o las reglas operativas.
* **Usa Documento de caso de uso** cuando el comportamiento necesite significado explícito, consecuencias, validaciones o errores esperados.
* **Usa Documento de capacidad** cuando varios comportamientos o procesos dependan de una capacidad estable.
* **Usa Registro de decisión** cuando una elección tenga _tradeoffs_, consecuencias o impacto futuro significativos.
* **Usa Nota de validación** cuando la evidencia cambie o confirme conocimiento del que dependerá el trabajo futuro.
* **Usa Nota de soporte** cuando el conocimiento sea útil pero todavía temprano, incierto, local o temporal.

## Principio de la taxonomía

La taxonomía sigue un principio:

> Elige los documentos por el conocimiento que preservan, no por la ceremonia que sugieren.

Un documento es útil cuando protege la continuidad. Si el conocimiento puede preservarse con un artefacto más pequeño, usa el artefacto más pequeño.
