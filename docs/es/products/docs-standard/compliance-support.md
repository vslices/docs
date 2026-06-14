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

| Estándar | Soporta | Soporta parcialmente | No provee |
| --- | --- | --- | --- |
| ISO/IEC/IEEE<br/>42010 | <ul><li>Contexto</li><li>Intereses</li><li>Justificación</li><li>Decisiones</li><li>Relaciones</li></ul> | <ul><li>Puntos de vista</li><li>Vistas</li><li>Correspondencias</li><li>Descripciones de<br/>arquitectura</li></ul> | Un framework completo y<br/>conforme para descripción<br/>de arquitectura |
| ISO/IEC/IEEE<br/>29148 | <ul><li>Comportamiento</li><li>Validación</li><li>Supuestos</li><li>Errores esperados</li><li>Trazabilidad</li></ul> | <ul><li>Atributos de calidad<br/>de requisitos</li><li>Enlaces de verificación</li></ul> | Un proceso completo de<br/>especificación y gestión de<br/>requisitos |


| Práctica | Soporta | Soporta parcialmente | No provee |
| --- | --- | --- | --- |
| arc42 | <ul><li>Contexto</li><li>Decisiones</li><li>Riesgos</li><li>Glosario</li><li>Continuidad</li></ul> | <ul><li>Tiempo de ejecución</li><li>Despliegue</li><li>Vistas de bloques<br/>de construcción</li></ul> | La estructura completa de<br/>arc42 por defecto |
| C4 Model | <ul><li>Razonamiento a<br/>nivel de contexto</li><li>Conciencia de<br/>límites</li></ul> | <ul><li>Contenedor</li><li>Componente</li><li>Vistas de código</li></ul> | Notación de diagramas y<br/>jerarquía visual de modelos |
| ADR | <ul><li>Razonamiento<br/>de decisión</li><li>Tradeoffs</li><li>Consecuencias</li></ul> | <ul><li>Ciclo de vida de<br/>decisiones específicas<br/>de arquitectura</li></ul> | Un template ADR estricto o<br/>proceso de gobernanza |
| 4+1 Model | <ul><li>Escenarios</li><li>Razonamiento<br/>orientado a<br/>casos de uso</li></ul> | <ul><li>Vistas lógicas</li><li>Vistas de proceso</li><li>Vistas de desarrollo</li><li>Vistas físicas</li></ul> | Un modelo completo de vistas<br/>arquitectónicas 4+1 |

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
