# Glosario de VSlices Docs Standard

Este glosario define conceptos usados por VSlices Docs Standard.

VSlices Docs Standard se enfoca en preservar conocimiento útil mediante estructuras de documentación viva.

Este glosario no redefine cada tipo de documento. Los tipos de documento específicos se explican en la taxonomía de Docs Standard y en sus propias páginas.

Estos términos ayudan a describir qué tipo de conocimiento debe documentarse, por qué importa y cómo los documentos pueden seguir conectados con el trabajo real.

## Conceptos de documentación

- __Documentación viva (_Living Documentation_ en inglés)__: documentación que evoluciona junto con el sistema, las decisiones, la comprensión del dominio, la implementación, la validación y el _feedback_.

- __Estructura de documento (_Document Structure_ en inglés)__: la forma esperada de un documento, incluyendo su propósito, secciones, relaciones y uso previsto.

- __Tipo de documento (_Document Type_ en inglés)__: una forma reutilizable de documentación usada para preservar un tipo específico de conocimiento, como contexto, proceso, comportamiento, capacidad, decisión o validación.

- __Artefacto de conocimiento (_Knowledge Artifact_ en inglés)__: una pieza de conocimiento preservada de la que el trabajo futuro puede depender, como un documento, una nota, un diagrama, una decisión, un ejemplo o un resultado de validación.

- __Límite de documentación (_Documentation Boundary_ en inglés)__: el límite que define qué debe explicar un documento y qué debe dejarse a otro documento.

## Conceptos de relación

- __Relación de documento (_Document Relationship_ en inglés)__: una conexión entre documentos que ayuda a preservar trazabilidad entre contexto, decisiones, procesos, comportamientos, capacidades, validación e implementación.

- __Referencia (_Reference_ en inglés)__: un enlace explícito desde un documento hacia otro documento, concepto, decisión, comportamiento o artefacto.

- __Trazabilidad (_Traceability_ en inglés)__: la capacidad de seguir cómo el conocimiento se mueve entre descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución.

- __Etapa de documento (_Document Stage_ en inglés)__: el nivel de madurez, estabilidad o confianza que representa actualmente un documento.

- __Afinidad de documento (_Document Affinity_ en inglés)__: la relación natural entre un tipo de documento y el tipo de trabajo, conocimiento, incertidumbre o etapa del ciclo de vida que mejor apoya.

## Conceptos de calidad del conocimiento

- __Conocimiento útil (_Useful Knowledge_ en inglés)__: conocimiento que ayuda al trabajo futuro a entender, decidir, implementar, validar, mantener o evolucionar algo con más seguridad.

- __Intención preservada (_Preserved Intent_ en inglés)__: el razonamiento, significado, propósito y restricciones que deberían seguir siendo comprensibles después de que la discusión o decisión original haya pasado.

- __Deriva de documentación (_Documentation Drift_ en inglés)__: la distancia que aparece cuando la documentación y el comportamiento real del sistema evolucionan por separado.

- __Conocimiento desactualizado (_Outdated Knowledge_ en inglés)__: conocimiento documentado que ya no refleja la comprensión, el comportamiento, la decisión o la implementación actuales.

- __Deuda de documentación (_Documentation Debt_ en inglés)__: brechas de documentación acumuladas, explicaciones desactualizadas, decisiones faltantes o conocimiento desconectado que hacen más difícil el trabajo futuro.

## Relación entre los términos

VSlices Docs Standard ayuda a los equipos a preservar conocimiento usando la estructura de documento más pequeña útil.

```text
Useful knowledge
-> Document type
-> Document structure
-> Document relationship
-> Traceability
-> Living documentation
```

Esto no es un requisito para documentarlo todo. Un equipo debe documentar el conocimiento del que depende el trabajo futuro, usando la estructura más pequeña que preserve suficiente significado, contexto e intención.

El objetivo no es más documentación. El objetivo es menos pérdida de conocimiento.
