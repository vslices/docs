# Soporte para cumplimiento

VSlices Docs Standard prioriza la continuidad del conocimiento por encima del cumplimiento formal. No es una implementación certificada de ningún estándar externo.

Sin embargo, puede ayudar a los equipos a preparar documentación que sea más fácil de mapear hacia estándares establecidos, prácticas de documentación de arquitectura y revisiones orientadas a cumplimiento.

Los equipos que necesiten cumplimiento formal deberían usar VSlices Docs Standard como una capa de continuidad, y luego añadir los artefactos, controles, revisiones, evidencias y mecanismos de aprobación específicos que requiera su estándar objetivo.

## Posición

VSlices Docs Standard está influido por prácticas existentes de documentación y arquitectura.

No las implementa directamente. Se trata de ser honesto sobre:

* **qué soporta VSlices**: áreas en las que los documentos de VSlices ya proporcionan una estructura útil.
* **qué soporta parcialmente VSlices**: áreas en las que VSlices proporciona conocimiento relacionado, pero no la forma completa requerida.
* **qué no proporciona VSlices**: áreas que requieren artefactos o controles adicionales específicos de cumplimiento.

## Resumen de soporte por estándar/práctica

| Standard | Supports | Partially supports | Does not provide |
| --- | --- | --- | --- |
| ISO/IEC/IEEE<br/>42010 | <ul><li>Context</li><li>Concerns</li><li>Rationale</li><li>Decisions</li><li>Relationships</li></ul> | <ul><li>Viewpoints</li><li>Views</li><li>Correspondences</li><li>Architecture<br/>descriptions</li></ul> | Full conforming architecture<br/>description framework |
| ISO/IEC/IEEE<br/>29148 | <ul><li>Behavior</li><li>Validation</li><li>Assumptions</li><li>Expected errors</li><li>Traceability</li></ul> | <ul><li>Requirement quality<br/>attributes</li><li>Verification links</li></ul> | Full requirements specification<br/>and management process |

| Practice | Supports | Partially supports | Does not provide |
| --- | --- | --- | --- |
| arc42 | <ul><li>Context</li><li>Decisions</li><li>Risks</li><li>Glossary</li><li>Continuity</li></ul> | <ul><li>Runtime</li><li>Deployment</li><li>Building block views</li></ul> | Complete arc42 structure<br/>by default |
| C4 Model | <ul><li>Context-level thinking</li><li>Boundary awareness</li></ul> | <ul><li>Container</li><li>Component</li><li>Code views</li></ul> | Diagram notation and visual<br/>model hierarchy |
| ADR | <ul><li>Decision reasoning</li><li>Tradeoffs</li><li>Consequences</li></ul> | <ul><li>Architecture-specific<br/>decision lifecycle</li></ul> | A strict ADR template or<br/>governance process |
| 4+1 View<br/>Model | <ul><li>Scenarios</li><li>Use-case<br/>oriented thinking</li></ul> | <ul><li>Logical</li><li>Process</li><li>Development</li><li>Physical views</li></ul> | Complete 4+1 architecture<br/>view model |

## Cómo usar esto

Usa este documento para entender cómo VSlices Docs Standard puede apoyar la alineación con estándares externos, plantillas de arquitectura, políticas de clientes, expectativas de auditoría o requisitos regulatorios.

Los documentos de VSlices pueden contener conocimiento que esos requisitos externos también necesitan. Sin embargo, VSlices Docs Standard no vuelve ese conocimiento conforme por sí mismo.

Cuando un equipo necesita alinearse con un requisito externo:

- __empieza con VSlices Docs Standard__: preserva primero el conocimiento real de ingeniería, incluyendo contexto, procesos, comportamiento, capacidades, decisiones, validación y evolución.
- __identifica el requisito objetivo__: aclara qué estándar, marco, política de cliente, expectativa de auditoría o requisito regulatorio debe cumplirse.
- __mapea los documentos existentes__: conecta los documentos de VSlices con los artefactos solicitados por el requisito objetivo.
- __identifica evidencias o controles faltantes__: encuentra lo que el requisito objetivo necesita y que VSlices no proporciona por defecto, como aprobaciones, ciclos de revisión, trazabilidad formal, diagramas requeridos, evidencias de auditoría o formatos específicos.
- __extiende sin desconectar__: añade el material de cumplimiento requerido manteniéndolo vinculado al conocimiento de ingeniería original.

El propósito es reutilizar la documentación de VSlices como una base de continuidad. No es afirmar cumplimiento automáticamente.

## Principio

VSlices Docs Standard debería ayudar a los equipos a estar más preparados para el cumplimiento. No debería pretender reemplazar el cumplimiento.

> Preserva primero el conocimiento. Añade controles de cumplimiento cuando el contexto lo requiera.
