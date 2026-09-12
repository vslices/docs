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

| Preserva                   | Documento                    | Pregunta principal                      | Ejemplos                                                                                                |
| -------------------------- | ---------------------------- | --------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Lenguaje                   | Vocabulario<br/>de dominio   | ¿Qué significa esto?                    | <ul><li>Términos</li><li>alias</li><li>significados en<br/>conflicto</li><li>ejemplos</li></ul>         |
| Scenario                   | Documento de<br/>contexto    | ¿Dónde estamos<br/>trabajando?          | <ul><li>Organización</li><li>área</li><li>actores</li><li>límites</li><li>puntos de dolor</li></ul>     |
| Work line                  | Documento de<br/>contexto    | ¿Qué ofrecemos u<br/>operamos?          | <ul><li>Departamentos</li><li>servicios</li><li>líneas de negocio</li><li>_value streams_</li></ul>     |
| Work process               | Documento de<br/>proceso     | ¿Cómo lo hacemos?                       | <ul><li>Responsabilidades</li><li>roles</li><li>coordinación</li><li>estructura<br/>operativa</li></ul> |
| Workflow                   | Documento de<br/>proceso     | ¿Qué se hace?                           | <ul><li>Pasos</li><li>_handoffs_</li><li>decisiones</li><li>participantes responsables</li></ul>        |
| Comportamiento             | Documento de<br/>caso de uso | ¿Qué significa este<br/>comportamiento? | <ul><li>Consecuencias</li><li>validaciones</li><li>errores esperados</li><li>reglas</li></ul>           |
| Capacidad                  | Documento de<br/>capacidad   | ¿Qué debe ser<br/>posible?              | Capacidades estables del negocio<br/>o del sistema                                                      |
| Decisión                   | Registro de<br/>decisión     | ¿Por qué elegimos<br/>esto?             | <ul><li>Opciones</li><li>razonamiento</li><li>_tradeoffs_</li><li>consecuencias</li></ul>               |
| Aprendizaje                | Nota de<br/>validación       | ¿Qué aprendimos?                        | <ul><li>Evidencia</li><li>resultados</li><li>_feedback_</li><li>preguntas siguientes</li></ul>          |
| Conocimiento<br/>emergente | Nota de soporte              | ¿Qué no deberíamos<br/>perder todavía?  | <ul><li>Conceptos</li><li>supuestos</li><li>riesgos</li><li>preguntas</li><li>_feedback_</li></ul>      |

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
