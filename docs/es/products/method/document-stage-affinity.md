# Afinidad documento-etapa

La afinidad documento-etapa (_Document-Stage Affinity_ en inglés) explica cómo los documentos de _VSlices Docs Standard_ pueden apoyar cada etapa de una iteración de _VSlices Design_.

No hace que los documentos sean obligatorios. Ayuda a los equipos a elegir documentación útil sin convertir _VSlices Method_ en una _checklist_. El flujo compartido de iteración es:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

## Idea central

Cada etapa crea o cambia un tipo distinto de conocimiento. Algunos documentos apoyan naturalmente mejor algunas etapas que otras.

Esta afinidad es solo una guía. Un equipo puede crear, actualizar, omitir, fusionar o volver a visitar documentos cuando la iteración lo requiera.

La pregunta no es _¿Qué documentos requiere esta etapa?_, es: **¿Qué conocimiento necesitamos preservar para tomar la siguiente decisión responsable?**.

## Afinidad por etapa

| Etapa | Conocimiento que se está manejando | Documentos útiles | Riesgo principal evitado |
| --- | --- | --- | --- |
| **Understanding** | Señales tempranas del dominio, lenguaje, supuestos, riesgos y preguntas abiertas. | **Domain Vocabulary**, **Support Note**, **Context Document** temprano. | Diseñar artefactos de _software_ antes de entender el mundo al que pertenecen. |
| **Contextualizing** | Escenario, actores, límites, líneas de trabajo, _workflows_ y contexto circundante. | **Context Document**, **Process Document**, **Domain Vocabulary**, **Support Note**. | Tratar un problema, caso de uso o _feature_ como si estuviera aislado de su contexto. |
| **Planning** | Mejora esperada, comportamiento, capacidades, alcance, decisiones y _tradeoffs_. | **Use Case Document**, **Capability Document**, **Decision Record**, **Support Note**. | Resolver un problema técnico atractivo en vez del problema de negocio relevante. |
| **Building** | Comportamiento de implementación, validaciones, errores esperados, restricciones y _feedback_ de entrega. | **Use Case Document**, **Capability Document**, **Decision Record**, **Validation Note**, **Support Note**. | Tratar la implementación como el final del aprendizaje. |
| **Returning to Understanding** | Evidencia, aprendizaje, supuestos cambiados, contexto actualizado y nueva incertidumbre. | **Validation Note**, **Context Document**, **Process Document**, **Use Case Document**, **Decision Record**, **Support Note**. | Ignorar lo que el sistema enseñó después de ser construido. |

## Afinidad por documento

El mismo documento puede apoyar más de una etapa.

| Documento | Afinidad más fuerte | Útil cuando |
| --- | --- | --- |
| [**Vocabulario de Dominio**](../docs-standard/taxonomy/domain-vocabulary.md) | **Understanding** y **Contextualizing**. | El lenguaje aparece, cambia, entra en conflicto o se vuelve importante para las decisiones. |
| [**Documento de Contexto**](../docs-standard/taxonomy/context-document.md) | **Contextualizing**. | El equipo necesita preservar el escenario, los actores, los límites o la situación actual. |
| [**Documento de Proceso**](../docs-standard/taxonomy/process-document.md) | **Contextualizing**. | El trabajo depende de responsabilidades, _workflows_, _handoffs_ u operaciones repetidas. |
| [**Documento de Caso de Uso**](../docs-standard/taxonomy/use-case-document.md) | **Planning** y **Building**. | Comportamiento, consecuencias, validaciones o errores esperados necesitan guiar la implementación. |
| [**Documento de Capacidad**](../docs-standard/taxonomy/capability-document.md) | **Planning** y **Building**. | Una capacidad estable de negocio o sistema necesita ser nombrada y preservada. |
| [**Registro de decisión**](../docs-standard/taxonomy/decision-record.md) | **Planning** y **Building**. | Una dirección, _tradeoff_, riesgo aceptado u opción rechazada puede afectar trabajo futuro. |
| [**Nota de Validación**](../docs-standard/taxonomy/validation-note.md) | **Building** y **Returning to Understanding**. | Evidencia desde implementación, revisión, uso u operación cambia lo que el equipo sabe. |
| [**Nota de soporte**](../docs-standard/taxonomy/support-note.md) | Todas las etapas. | El conocimiento es útil, pero todavía temprano, local, incierto o temporal. |

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
