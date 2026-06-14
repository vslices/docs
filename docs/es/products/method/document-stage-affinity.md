# Afinidad documento-etapa

La afinidad documento-etapa (_Document-Stage Affinity_ en inglés) explica cómo los documentos de _VSlices Docs Standard_ pueden apoyar cada etapa de una iteración de _VSlices Design_.

No hace que los documentos sean obligatorios. Ayuda a los equipos a elegir documentación útil sin convertir _VSlices Method_ en una _checklist_. El flujo compartido de iteración es:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

## Idea central

Cada etapa crea o cambia un tipo distinto de conocimiento. Algunos documentos apoyan naturalmente mejor algunas etapas que otras.

Esta afinidad es solo una guía. Un equipo puede crear, actualizar, omitir, fusionar o volver a visitar documentos cuando la iteración lo requiera.

La pregunta no es _¿Qué documentos requiere esta etapa?_, si no: **¿Qué conocimiento necesitamos preservar para tomar la siguiente decisión responsable?**.

## Afinidad por etapa

| Etapa                               | Conocimiento a manejar                                                                                                                                | Documentos útiles                                                                                                                                                                  | Riesgo evitado                                                              |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| **Understanding**                   | <ul><li>Señales tempranas<br/>del dominio</li><li>Lenguaje</li><li>Supuestos</li><li>Riesgos</li><li>Preguntas abiertas</li></ul>                         | <ul><li>**Domain Vocabulary**</li><li>**Support Note**</li><li>**Context Document**<br/>temprano</li></ul>                                                                             | Diseñar artefactos<br/>de *software* antes<br/>de entender el mundo<br/>al que pertenecen.        |
| **Contextualizing**                 | <ul><li>Escenario</li><li>Actores</li><li>Límites</li><li>Líneas de trabajo</li><li>*workflows*</li><li>Contexto circundante</li></ul>                | <ul><li>**Context Document**</li><li>**Process Document**</li><li>**Domain Vocabulary**</li><li>**Support Note**</li></ul>                                                         | Tratar un problema,<br/>caso de uso o *feature*<br/>como si estuviera<br/>aisladode su contexto. |
| **Planning**                        | <ul><li>Mejora esperada</li><li>Comportamiento</li><li>Capacidades</li><li>Alcance</li><li>Decisiones</li><li>*tradeoffs*</li></ul>                   | <ul><li>**Use Case Document**</li><li>**Capability Document**</li><li>**Decision Record**</li><li>**Support Note**</li></ul>                                                       | Resolver un problema<br/>técnico atractivo en<br/>vez del problema de<br/>negocio relevante.      |
| **Building**                        | <ul><li>Comportamiento de<br/>implementación</li><li>Validaciones</li><li>Errores esperados</li><li>Restricciones</li><li>*feedback* de entrega</li></ul> | <ul><li>**Use Case Document**</li><li>**Capability Document**</li><li>**Decision Record**</li><li>**Validation Note**</li><li>**Support Note**</li></ul>                           | Tratar la <br/>implementación como<br/>el final del<br/>aprendizaje.                               |
| **Returning to<br/> Understanding** | <ul><li>Evidencia</li><li>Aprendizaje</li><li>Supuestos cambiados</li><li>Contexto actualizado</li><li>Nueva incertidumbre</li></ul>                  | <ul><li>**Validation Note**</li><li>**Context Document**</li><li>**Process Document**</li><li>**Use Case Document**</li><li>**Decision Record**</li><li>**Support Note**</li></ul> | Ignorar lo que el<br/>sistema enseñó<br/>después de ser<br/>construido.                           |


## Afinidad por documento

El mismo documento puede apoyar más de una etapa.

| Documento | Afinidad más fuerte | Útil cuando |
| --- | --- | --- |
| [**Vocabulario de Dominio**](../docs-standard/taxonomy/domain-vocabulary.md) | **Understanding** y<br/>**Contextualizing**. | El lenguaje aparece, cambia, entra en<br/>conflicto o se vuelve importante para las<br/>decisiones. |
| [**Documento de Contexto**](../docs-standard/taxonomy/context-document.md) | **Contextualizing**. | El equipo necesita preservar el escenario,<br/>los actores, los límites o la situación actual. |
| [**Documento de Proceso**](../docs-standard/taxonomy/process-document.md) | **Contextualizing**. | El trabajo depende de responsabilidades,<br/>_workflows_, _handoffs_ u operaciones repetidas. |
| [**Documento de Caso de Uso**](../docs-standard/taxonomy/use-case-document.md) | **Planning** y **Building**. | Comportamiento, consecuencias, validaciones<br/>o errores esperados necesitan guiar la<br/>implementación. |
| [**Documento de Capacidad**](../docs-standard/taxonomy/capability-document.md) | **Planning** y **Building**. | Una capacidad estable de negocio o sistema<br/>necesita ser nombrada y preservada. |
| [**Registro de decisión**](../docs-standard/taxonomy/decision-record.md) | **Planning** y **Building**. | Una dirección, _tradeoff_, riesgo aceptado u<br/>opción rechazada puede afectar trabajo<br/>futuro. |
| [**Nota de Validación**](../docs-standard/taxonomy/validation-note.md) | **Building** y **Returning<br/>to Understanding**. | Evidencia desde implementación, revisión,<br/>uso u operación cambia lo que el equipo sabe. |
| [**Nota de soporte**](../docs-standard/taxonomy/support-note.md) | Todas las etapas. | El conocimiento es útil, pero todavía<br/>temprano, local, incierto o temporal. |

## Uso de la afinidad

La afinidad documental debería ayudar al equipo a decidir qué preservar. No debería decidir por el equipo. Usa un documento cuando ayude al equipo a:

* clarificar lenguaje
* preservar contexto
* explicar comportamiento
* hacer visible una decisión
* llevar intención hacia la implementación
* registrar evidencia
* evitar redescubrir el mismo conocimiento más adelante

Omite un documento cuando solo existe porque una etapa parece esperarlo.

## Regla de Method

Usa el documento que preserve el conocimiento necesario para la siguiente decisión responsable.

* Si un documento ayuda al equipo a avanzar con más claridad, úsalo.
* Si un documento crea ceremonia sin preservar conocimiento útil, omítelo.
