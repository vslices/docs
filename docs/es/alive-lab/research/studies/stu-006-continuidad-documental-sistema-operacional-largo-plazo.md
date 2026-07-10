---
type: study
state: candidate
code: STU-006
visibility: private-redacted
evidence_policy: summarized

related_questions:
* RQ-001
* RQ-002
* RQ-003
* RQ-004
* RQ-005
* RQ-006
* RQ-007

related_notes:
* RN-0001
* RN-0002
* RN-0003

related_synthesis:
* SYN-0001

related_findings:
* FND-0001
* FND-0002

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
---

# STU-006 — Continuidad documental en un sistema operacional de largo plazo

## Estado

candidate

## Visibilidad

private-redacted

## Política de evidencia

Este estudio trabaja con un caso real de un sistema operacional mantenido durante un período prolongado.

Por restricciones de privacidad, confidencialidad y responsabilidad profesional, el estudio no debe publicar documentos internos completos, nombres sensibles, detalles operacionales específicos, datos de negocio, información de clientes, diagramas completos ni material que permita reconstruir información privada del contexto.

La evidencia podrá utilizarse en forma de:

* descripciones generales
* artifacts redactados
* diagramas simplificados
* ejemplos sintéticos derivados
* observaciones metodológicas
* resultados agregados
* comparación entre estados documentales
* evolución de prácticas documentales
* feedback general de personas involucradas

Los artifacts reales podrán resumirse, anonimizarse o transformarse en ejemplos equivalentes cuando sea necesario.

## Contexto

Este estudio ocurre en Hual, un contexto donde el equipo de desarrollo cumple en la práctica una función cercana a un área de TI para la organización.

El sistema ha sido desarrollado, mantenido y extendido durante un período prolongado.

Al inicio del proyecto, parte de la documentación fue producida con una versión muy prototipo de VSlices Method.

Esto hace que el caso sea especialmente útil para observar continuidad en el tiempo:

> ¿Qué ocurre cuando un sistema real, vivo y operacional evoluciona durante años mientras las prácticas documentales también maduran?

A diferencia de un caso centrado en transferencia puntual de conocimiento, este estudio observa continuidad sostenida, evolución de artifacts, cambios de necesidades, mantenimiento operativo y aprendizaje acumulado.

## Situación observada

En sistemas operacionales de largo plazo, el conocimiento no se pierde necesariamente de una vez.

Puede degradarse lentamente.

Puede quedar repartido entre:

* código
* conversaciones
* decisiones pasadas
* documentos antiguos
* convenciones de uso
* ajustes operacionales
* conocimiento de usuarios
* conocimiento del equipo técnico
* incidencias resueltas
* integraciones
* reportes
* procesos manuales o semi-manuales

Además, el sistema puede seguir cambiando mientras la documentación queda congelada en una forma anterior del proyecto.

En este caso existe una tensión particular:

> El sistema siguió evolucionando, pero la documentación inicial nació desde una versión prototipo de VSlices y puede no representar completamente las necesidades actuales de continuidad.

## Problema de continuidad

El problema central es preservar continuidad documental en un sistema vivo.

La pregunta no es solo cómo documentar una funcionalidad, sino cómo mantener trazabilidad suficiente entre:

* operación real
* necesidades de negocio
* usuarios
* procesos
* flujos
* decisiones
* comportamiento esperado
* estructura técnica
* incidentes
* ajustes
* evolución del sistema
* conocimiento histórico
* conocimiento vigente

La continuidad puede romperse por varias razones:

* documentación inicial insuficiente
* documentación desactualizada
* cambios acumulados sin registro claro
* decisiones implícitas
* conocimiento concentrado en pocas personas
* integración entre módulos o procesos no explícita
* diferencias entre uso real y documentación existente
* crecimiento del sistema sin reorganización documental

## Pregunta local del estudio

¿Cómo evoluciona la continuidad documental en un sistema operacional mantenido durante largo plazo cuando se pasa desde una documentación prototipo hacia mecanismos más formales de VSlices Docs Standard?

## RQs relacionadas

Este estudio puede alimentar varias preguntas de investigación de Docs Standard.

| RQ                                   | Relación con el estudio                                                                                 |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------- |
| [RQ-002 — Caminos de Continuidad](../questions/rq-002-continuity-paths.md)      | Observa si paths ayudan a recorrer conocimiento acumulado y evolución del sistema                       |
| [RQ-003 — Nexos Documentales](../questions/rq-003-document-nexus.md)          | Puede observar si capabilities, integraciones o procesos compuestos requieren composición documental    |
| [RQ-004 — Documentos](../questions/rq-004-documents.md)                  | Observa si Documents por pregunta principal ayudan a ordenar conocimiento operacional                   |
| [RQ-005 — Organizaciones Documentales](../questions/rq-005-documental-organization.md) | Observa cómo organizar artifacts de un sistema vivo sin duplicar fuentes de verdad                      |
| [RQ-006 — Notas de Soporte](../questions/rq-006-support-notes.md)            | Observa si notas auxiliares ayudan a capturar riesgos, resultados, validaciones o conocimiento temporal |
| [RQ-007 — Diagramas Documentales](../questions/rq-007-diagrams.md)      | Observa si diagramas ayudan a representar evolución, recorridos, composición o estado documental        |

Aunque el caso puede alimentar varias RQs, no debe intentar validarlas todas con el mismo peso.

Su foco principal debería ser `RQ-002`, `RQ-004`, `RQ-005` y `RQ-007`.

## Mecanismos de Docs Standard observados

### Document artifacts

El estudio puede observar Documents orientados a preguntas principales como:

* Context Document
* Domain Vocabulary
* Behavior Document
* Structure Document
* Scope Document
* Consistency Document
* Update Document
* Feedback Document
* Decision Record
* Navigation Document

Estos documents pueden ayudar a distinguir conocimiento vigente, histórico, operacional y técnico.

La observación principal no es si todos los documentos existen, sino si los documents necesarios permiten preservar continuidad sin sobrecargar el mantenimiento.

### Continuity Paths

Este estudio puede usar Continuity Paths para recorrer conocimiento acumulado.

Paths especialmente relevantes:

* Business Scenario
* Domain Context
* Software Initiative
* Software Project
* Client Product
* Consumable Service
* Evolution
* Impact
* Ownership
* Traceability

El path de Evolution puede ser especialmente importante porque el caso implica cambios sostenidos en el tiempo.

El path de Impact también puede aportar cuando modificaciones en una zona del sistema afectan procesos, reportes, integraciones o flujos operacionales.

### Organizaciones documentales

El estudio puede observar cómo organizar documentación alrededor de diferentes criterios.

Posibles organizaciones:

* por proceso operacional
* por módulo
* por flujo
* por capability
* por sistema
* por integración
* por tipo documental
* por evolución histórica
* por estado vigente o deprecated
* por prioridad de mantenimiento

La organización documental debe ayudar a recorrer conocimiento sin duplicar artifacts ni convertir carpetas en única fuente de verdad conceptual.

### Support Notes

El estudio puede usar Support Notes para preservar:

* resultados de revisión
* riesgos operacionales
* dudas sobre comportamiento vigente
* validaciones parciales
* referencias externas
* notas de testing
* hallazgos durante mantenimiento
* conocimiento temporal mientras se decide si requiere Document artifact

### Nexus artifacts

El estudio puede observar si ciertos elementos compuestos requieren Nexus.

Por ejemplo:

* una capability operacional relevante
* una integración crítica
* un flujo que involucra varias áreas del sistema
* un reporte o proceso que depende de varias fuentes
* una zona que combina decisiones, comportamiento, estructura y reglas

El Nexus solo debería aparecer si ayuda a reducir fragmentación real.

### Diagramas documentales

El estudio puede usar diagramas para representar:

* continuidad entre procesos y software
* evolución de una capacidad
* relaciones entre módulos
* impactos de cambios
* recorridos documentales
* artifacts existentes y faltantes
* composición de capabilities o integraciones
* estado documental de zonas del sistema

Los diagramas deben mantenerse simplificados y redactados si existe riesgo de exponer información sensible.

## Evidencia disponible

La evidencia inicial esperada puede incluir:

* documentación prototipo creada en etapas anteriores
* documentación actual o parcialmente actualizada
* artifacts nuevos creados bajo Docs Standard
* decisions records
* diagrams simplificados
* notas de soporte
* incidentes o cambios relevantes
* feedback de usuarios o stakeholders
* feedback del equipo técnico
* comparación entre documentación previa y mecanismos actuales
* observaciones sobre mantenimiento real
* ejemplos redactados de evolución documental
* señales de conocimiento vigente, perdido, disperso o implícito

La evidencia publicada deberá ser resumida, redactada o transformada en ejemplos sintéticos cuando corresponda.

## Observaciones esperadas

Este estudio podría permitir observar:

* si una documentación prototipo conserva valor después de años
* qué partes de la documentación inicial quedaron obsoletas
* qué tipo de artifacts ayudan más a recuperar continuidad
* si los Continuity Paths ayudan a recorrer conocimiento histórico y vigente
* si los Documents por pregunta principal reducen ambigüedad
* si las organizaciones documentales ayudan a navegar un sistema vivo
* si las Support Notes ayudan a capturar hallazgos de mantenimiento
* si los diagramas ayudan a explicar evolución o impacto
* si Nexus reduce fragmentación en procesos o capacidades compuestas
* si Docs Standard ayuda a transformar documentación antigua sin rehacer todo

## Evidencia faltante

Todavía falta observar:

* qué artifacts existentes siguen siendo útiles
* qué artifacts están obsoletos
* qué conocimiento crítico no está documentado
* qué paths ayudan realmente a recorrer el sistema
* qué organización documental reduce fricción
* qué diagramas son útiles para explicar evolución
* qué documentos nuevos son necesarios
* qué documentos no vale la pena crear
* qué feedback entregan lectores reales
* qué costo introduce actualizar documentación histórica
* qué cambios requiere Docs Standard para sistemas de largo plazo

## Criterios iniciales de observación

El estudio puede considerar señales positivas si:

* la documentación existente puede evolucionar sin descartarse por completo
* los Documents ayudan a separar responsabilidades
* los paths permiten reconstruir recorridos de conocimiento
* las organizaciones reducen duplicación
* los diagramas aclaran relaciones o impacto
* las Support Notes preservan hallazgos sin crear burocracia
* los Nexus reducen fragmentación en elementos compuestos
* el equipo identifica mejor qué conocimiento está vigente
* el equipo identifica mejor qué conocimiento quedó histórico, obsoleto o incierto

El estudio puede considerar señales problemáticas si:

* actualizar documentación antigua cuesta más que reescribirla
* los paths se vuelven mapas demasiado grandes
* las organizaciones documentales confunden más de lo que orientan
* los diagramas se vuelven ilegibles
* las Support Notes se acumulan sin cierre
* los Nexus agregan capas sin reducir fragmentación
* los Documents duplican documentación operacional existente
* el equipo no distingue conocimiento vigente de histórico
* Docs Standard exige más precisión de la que el contexto puede sostener

## Riesgos metodológicos

### Riesgo de supervivencia documental

Que un artifact antiguo todavía exista no significa que siga siendo útil.

El estudio debe distinguir existencia documental de continuidad efectiva.

### Riesgo de atribuir madurez al paso del tiempo

Un sistema antiguo no necesariamente tiene mejor conocimiento preservado.

Puede tener más historia, pero también más pérdida, deuda o contradicción.

### Riesgo de juzgar documentación prototipo con criterios actuales

La documentación inicial fue creada con una versión temprana de VSlices.

No debe evaluarse como si hubiera aplicado el modelo actual completo.

### Riesgo de redacción excesiva

Por privacidad, parte de la evidencia debe simplificarse o redactarse.

Eso puede limitar la verificabilidad externa.

### Riesgo de validar por familiaridad

Como el equipo conoce profundamente el sistema, puede parecer que la documentación es más clara de lo que sería para una persona nueva.

### Riesgo de convertir continuidad larga en teoría general

Este caso puede sugerir patrones para sistemas de largo plazo, pero no valida universalmente Docs Standard en todos los contextos operacionales.

## Límites del estudio

Este estudio no puede demostrar que Docs Standard funciona en general.

No puede publicar toda la evidencia directa.

No puede asegurar que las prácticas documentales observadas sean transferibles a cualquier organización.

No puede evaluar de forma completamente aislada el impacto de Docs Standard frente a experiencia acumulada, relación con usuarios, conocimiento del equipo o evolución natural del sistema.

No debe concluir que todos los sistemas de largo plazo requieren la misma organización documental.

Su valor está en observar cómo mecanismos candidatos de Docs Standard pueden ayudar o no ayudar a preservar continuidad en un sistema operacional vivo que ha evolucionado durante años.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre documentación de largo plazo
* Tensions entre evolución, mantenimiento y costo documental
* Findings locales sobre utilidad o límites de Documents, Paths, Organizations, Notes, Nexus y Diagrams
* criterios para actualizar documentación prototipo
* ajustes candidatos a Docs Standard para sistemas vivos
* límites explícitos sobre evidencia privada redactada

## Relación con estudios fundacionales

Este estudio se relaciona especialmente con escenarios donde la continuidad puede romperse por pérdida histórica o dispersión activa.

Puede alimentar `SYN-0001` al observar cómo un sistema vivo acumula conocimiento que puede mantenerse, degradarse, dispersarse o volverse difícil de recorrer.

También puede complementar `STU-005`, porque mientras `STU-005` observa una transición concentrada en handoff, este estudio observa continuidad sostenida en el tiempo.

## Límite actual

Este estudio debe mantenerse en estado `candidate` mientras no se haya revisado evidencia suficiente.

El caso es metodológicamente valioso porque permite observar documentación y continuidad en un sistema real, operacional y de largo plazo.

Sin embargo, por su carácter privado y por la existencia de documentación prototipo previa, sus conclusiones deben formularse con prudencia y distinguir claramente entre evidencia observada, interpretación local y posible ajuste a Docs Standard.
