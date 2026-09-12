# Soporte para compliance

VSlices Docs Standard prioriza la continuidad del conocimiento por encima del cumplimiento formal.

No es una implementación certificada de ningún estándar externo ni declara conformidad con marcos, normas, auditorías o regulaciones específicas.

Puede ayudar a preparar documentación más fácil de mapear hacia estándares establecidos, políticas internas, auditorías o revisiones orientadas a cumplimiento.

!!! principle "Principio de Compliance"

    Preserva primero el conocimiento de ingeniería. Añade controles de cumplimiento cuando el contexto lo requiera.


Los equipos que necesiten cumplimiento formal deberían usar VSlices Docs Standard como una capa de continuidad y luego añadir los artefactos, controles, revisiones, evidencias y mecanismos de aprobación que requiera su estándar objetivo.

## Posición

VSlices Docs Standard está influido por prácticas existentes de documentación, arquitectura y trazabilidad.

No las implementa directamente.

Esta página ayuda a distinguir:

* qué puede apoyar VSlices: áreas donde la documentación de VSlices ya proporciona una estructura útil
* qué puede apoyar parcialmente VSlices: áreas donde VSlices preserva conocimiento relacionado, pero no toda la forma requerida
* qué requiere agregar: áreas que necesitan artefactos, controles, aprobaciones o evidencias específicas

## Qué agregan los caminos de continuidad

Los caminos de continuidad agregan una capa de lectura entre los documentos individuales de VSlices y los estándares externos.

Un estándar externo normalmente no solo necesita documentos aislados. También necesita entender cómo se relacionan contexto, decisiones, comportamiento, arquitectura, evidencias y evolución.

VSlices Docs Standard puede apoyar ese trabajo al organizar documentos alrededor de caminos de continuidad.

Esto no convierte a VSlices en una implementación formal de esos estándares.

Solo ayuda a mapear el conocimiento preservado hacia artefactos, vistas, controles o evidencias que otros estándares puedan requerir.

!!! principle "Principio de Mapeo"

    Mapea primero la continuidad preservada. Después agrega los artefactos, controles o evidencias formales que el estándar externo requiera.


## Resumen de apoyo

La siguiente tabla no declara conformidad.

Solo muestra áreas donde los caminos y documentos de VSlices pueden servir como base para preparar, mapear o complementar documentación requerida por referencias externas.

!!! risk "Riesgo a evitar"

    No uses esta tabla como evidencia automática de cumplimiento formal.


| Referencia externa | Caminos que pueden apoyar                                       | Puede apoyar                                                                | Puede apoyar parcialmente                                                 | Requiere agregar                                                   |
| ------------------ | --------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| ISO/IEC/IEEE 42010 | Proyecto de software, Contexto de dominio, Servicio consumible  | Contexto, intereses, justificación, decisiones y relaciones documentales    | Puntos de vista, vistas, correspondencias y descripciones de arquitectura | Framework conforme de descripción de arquitectura                  |
| ISO/IEC/IEEE 29148 | Producto al cliente, Servicio consumible, Contexto de dominio   | Comportamiento esperado, supuestos, errores esperados y trazabilidad ligera | Atributos de calidad, verificación y gestión formal de requisitos         | Proceso formal de especificación, revisión, verificación y gestión |
| arc42              | Proyecto de software, Escenario de negocio, Contexto de dominio | Contexto, decisiones, riesgos, glosario y continuidad documental            | Vistas de ejecución, despliegue y bloques de construcción                 | Estructura completa de arc42                                       |
| C4 Model           | Proyecto de software, Servicio consumible                       | Contexto del sistema y conciencia de límites                                | Vistas de contenedor, componente y código                                 | Notación, jerarquía visual y convenciones completas de C4          |
| ADR                | Proyecto de software, Contexto de dominio                       | Razonamiento de decisión, tradeoffs y consecuencias                         | Ciclo de vida formal de decisiones de arquitectura                        | Template ADR estricto, gobernanza o aprobación                     |
| 4+1 Model          | Producto al cliente, Proyecto de software, Servicio consumible  | Escenarios y razonamiento orientado a casos de uso                          | Vistas lógica, de proceso, de desarrollo y física                         | Modelo completo de vistas arquitectónicas 4+1                      |

## Cómo usar esto

Usa este documento para entender cómo VSlices Docs Standard puede apoyar la alineación con estándares externos, plantillas de arquitectura, políticas de clientes, expectativas de auditoría o requisitos regulatorios.

VSlices puede preservar conocimiento que esos requisitos externos también necesitan, pero no vuelve ese conocimiento conforme por sí mismo.

Cuando un equipo necesita alinearse con un requisito externo:

1. Empieza con VSlices Docs Standard

    Preserva primero el conocimiento real de ingeniería: contexto, procesos, comportamiento, capacidades, decisiones, validación y evolución.

2. Identifica el camino de continuidad afectado

    Determina si el requisito se relaciona principalmente con escenario de negocio, contexto de dominio, proyecto de software, producto al cliente o servicio consumible.

3. Identifica el requisito objetivo

    Aclara qué estándar, marco, política de cliente, expectativa de auditoría o requisito regulatorio debe cumplirse.

4. Mapea los documentos existentes

    Conecta los documentos de VSlices y su camino de continuidad con los artefactos solicitados por el requisito objetivo.

5. Identifica evidencias o controles faltantes

    Encuentra lo que el requisito objetivo necesita y que VSlices no proporciona por defecto, como aprobaciones, ciclos de revisión, trazabilidad formal, diagramas requeridos, evidencias de auditoría o formatos específicos.

6. Extiende sin desconectar

    Añade el material de cumplimiento requerido manteniéndolo vinculado al conocimiento de ingeniería original.

## Qué no debería hacer esta página

Esta página no debería usarse para afirmar que VSlices Docs Standard cumple un estándar externo.

Tampoco reemplaza:

* revisión legal
* revisión de compliance
* auditoría formal
* aprobación de arquitectura
* controles organizacionales
* evidencias regulatorias específicas
* plantillas obligatorias de un cliente o industria

Su propósito es mostrar cómo la documentación de VSlices puede servir como base de continuidad para preparar esos trabajos.

## Regla de uso

!!! principle "Principio de Compliance"

    No uses VSlices Docs Standard como sustituto de revisión, evidencia, aprobación o conformidad formal.


Usa VSlices Docs Standard para preservar conocimiento de ingeniería que pueda apoyar trabajos de cumplimiento.
