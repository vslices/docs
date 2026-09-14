---
type: study
state: candidate
code: STU-008
visibility: public
evidence_policy: direct
study_scope: bounded

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
* FND-0004

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Design
* VSlices Framework
* VSlices Tooling
* Domus Orbis

---

# STU-008 — Construcción de producto desde cero con VSlices en un dominio doméstico

## Estado

candidate

## Visibilidad

public

## Política de evidencia

Este estudio trabaja con un caso real, propio y publicable.

A diferencia de estudios privados o redactados, este caso puede usar evidencia directa cuando sea conveniente:

* artifacts reales
* documentos de investigación
* decisiones de diseño
* fragments de YAML
* diagramas
* commits
* conversaciones sintetizadas
* iteraciones documentales
* cambios de modelo
* observaciones de uso
* hallazgos sobre dominio
* ejemplos del producto

Aun así, la evidencia debe manejarse con prudencia cuando incluya información doméstica sensible, hábitos personales, datos económicos, URLs privadas, compras reales o información que pueda exponer detalles innecesarios de la vida cotidiana.

La regla candidata es:

> Publicable no significa publicar todo. Significa que el caso puede mostrar artifacts reales o simplificados sin depender de confidencialidad empresarial.

## Contexto

Este estudio ocurre en Domus Orbis, un producto construido desde cero con VSlices.

Domus Orbis explora cómo transformar conocimiento doméstico cotidiano en artifacts, software y aprendizaje progresivo.

El caso nace desde una necesidad real: reducir carga ejecutiva y mejorar la planificación doméstica, especialmente alrededor de compras mensuales, productos esenciales, clasificación, reemplazos, disponibilidad, precios y continuidad entre decisiones prácticas y automatización futura.

Este caso es especialmente importante porque permite observar VSlices desde el inicio del trabajo, no como reconstrucción posterior.

> Domus Orbis permite observar cómo VSlices Design, Docs Standard, Method, Framework y Tooling pueden retroalimentarse mientras un producto real emerge desde un dominio cotidiano.

## Situación observada

Antes de existir software completo, ya existía conocimiento doméstico relevante.

Ese conocimiento estaba presente en:

* hábitos de compra
* decisiones sobre productos esenciales
* prioridades domésticas
* restricciones de presupuesto
* reemplazos aceptables
* preferencias de almacenamiento
* clasificaciones prácticas
* conocimiento de marcas, formatos y cantidades
* uso real de productos
* problemas de planificación mensual
* tensión entre gasto disponible y cobertura de despensa
* acuerdos domésticos implícitos

Parte de ese conocimiento no estaba formalizado.

Otra parte podía expresarse mediante listas, YAML, conversaciones, decisiones de clasificación o criterios de reemplazo.

El riesgo era digitalizar demasiado rápido una versión parcial del dominio.

## Problema de continuidad

El problema central es preservar continuidad entre:

* necesidad doméstica real
* descubrimiento de dominio
* clasificación de productos
* artifacts iniciales
* documentación viva
* decisiones de diseño
* comportamiento esperado
* estructura futura del software
* automatización progresiva
* evolución del producto

En este contexto, la continuidad puede romperse antes de existir software si el conocimiento doméstico tácito no se explora suficientemente.

También puede romperse si el artifact inicial se trata como simple dato y no como evidencia de dominio.

## Pregunta local del estudio

¿Cómo ayudan los mecanismos de VSlices Docs Standard a preservar continuidad desde conocimiento doméstico tácito hacia artifacts, decisiones y software en construcción progresiva?

## RQs relacionadas

Este estudio puede alimentar varias preguntas de investigación de Docs Standard.

| RQ                                   | Relación con el estudio                                                                                     |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| [RQ-002 — Caminos de Continuidad](../questions/rq-002-continuity-paths.md)      | Observa si paths ayudan a conectar escenario doméstico, dominio, producto, software y evolución             |
| [RQ-003 — Nexos Documentales](../questions/rq-003-document-nexus.md)          | Puede observar si capabilities o comportamientos compuestos requieren composición documental                |
| [RQ-004 — Documentos](../questions/rq-004-documents.md)                  | Observa si Documents por pregunta principal ayudan a preservar conocimiento emergente                       |
| [RQ-005 — Organizaciones Documentales](../questions/rq-005-documental-organization.md) | Observa cómo ordenar artifacts de producto, dominio, investigación y software                               |
| [RQ-006 — Notas de Soporte](../questions/rq-006-support-notes.md)            | Observa si notas auxiliares ayudan a preservar hipótesis, riesgos, resultados y validaciones domésticas     |
| [RQ-007 — Diagramas Documentales](../questions/rq-007-diagrams.md)      | Observa si diagramas ayudan a representar clasificación, continuidad, ramificación de preguntas o evolución |

Aunque el caso puede alimentar todas estas RQs, no debe intentar validarlas todas al mismo tiempo.

Su foco principal debería ser `RQ-004`, `RQ-006`, `RQ-002` y `RQ-007`.

## Mecanismos de Docs Standard observados

### Document artifacts

El estudio puede observar Documents como:

* Context Document
* Domain Vocabulary
* Behavior Document
* Structure Document
* Scope Document
* Consistency Document
* Viability Document
* Decision Record
* Feedback Document
* Update Document
* Navigation Document

Estos documents pueden ayudar a preservar continuidad entre observaciones domésticas y diseño de producto.

Por ejemplo:

* un Context Document puede explicar dónde aparece el problema doméstico
* un Domain Vocabulary puede preservar conceptos como producto, reemplazo, clasificación, almacenamiento o necesidad mensual
* un Behavior Document puede explicar qué debe ocurrir al preparar una lista
* un Consistency Document puede preservar reglas sobre clasificación o reemplazos
* un Decision Record puede registrar por qué se separó clasificación de metadata
* un Scope Document puede limitar qué parte del problema se aborda ahora

### Support Notes

Las Support Notes pueden ser especialmente útiles en Domus Orbis porque gran parte del conocimiento aparece de forma incompleta o exploratoria.

Pueden preservar:

* hipótesis de dominio
* dudas sobre clasificación
* riesgos de modelado
* resultados de uso de artifacts YAML
* validaciones domésticas iniciales
* referencias externas
* observaciones de compra
* problemas detectados al editar listas
* criterios todavía no estables

Las Support Notes pueden evitar que cada intuición doméstica se convierta prematuramente en Document artifact.

### Continuity Paths

Este estudio puede usar Continuity Paths para conectar perspectivas.

Paths especialmente relevantes:

* Business Scenario
* Domain Context
* Viability
* Evolution
* Software Initiative
* Client Product
* Software Project
* Impact
* Traceability
* Ownership

En Domus Orbis, el Business Scenario puede partir desde el trabajo doméstico real.

El Domain Context puede preservar lenguaje y reglas emergentes.

Evolution puede seguir cómo cambian artifacts, clasificaciones y decisiones.

Traceability puede conectar observación doméstica, decisión documental, modelo de dominio y comportamiento de software.

### Nexus artifacts

El estudio puede observar si ciertos elementos requieren Nexus.

Posibles candidatos:

* lista mensual de compra
* planificación de despensa
* clasificación de producto
* reemplazo de producto
* inventario doméstico
* capability de preparación de compra
* capability de recomendación o automatización futura

Un Nexus solo debería aparecer si ayuda a componer artifacts dispersos sin crear un documento monolítico.

### Organizaciones documentales

Domus Orbis puede observar organizaciones documentales alrededor de:

* dominio doméstico
* producto
* iteración
* capability
* artifact YAML
* decisiones
* investigación
* implementación
* evolución
* validación

Este caso puede ayudar a observar cómo un producto pequeño necesita varias formas de organización sin duplicar fuente de verdad.

### Diagramas documentales

El estudio puede usar diagramas para representar:

* ramificación de preguntas de un Document artifact
* continuidad desde escenario doméstico hacia software
* clasificación de productos
* relaciones entre producto, hogar, almacenamiento y proveedor
* evolución de artifacts
* paths entre observación, decisión y modelo
* capabilities candidatas
* necesidades documentales pendientes

Los diagramas deben mantenerse al servicio de la comprensión, no de la estética.

## Evidencia disponible

La evidencia inicial puede incluir:

* artifacts YAML de lista mensual
* cambios en estructura de productos
* separación entre metadata y classification
* decisiones sobre clasificación doméstica, de producto y almacenamiento
* aparición del concepto `replacement-kind`
* ejemplos de reemplazos same-kind y functional
* conversaciones de diseño sintetizadas
* documentos de Domus Orbis
* notas de investigación
* decisiones de alcance
* modelos de dominio candidatos
* iteraciones Slice-First
* observaciones de uso real
* feedback doméstico
* commits o cambios documentales cuando existan

Esta evidencia puede ser directa, pero debe redactarse cuando exponga información privada innecesaria.

## Observaciones esperadas

Este estudio podría permitir observar:

* si Docs Standard ayuda a preservar conocimiento antes de existir software completo
* si los Document artifacts ayudan a ordenar descubrimiento de dominio
* si las Support Notes evitan formalización prematura
* si los Continuity Paths conectan práctica doméstica, dominio, producto y software
* si los diagramas ayudan a representar clasificación o ramificación de preguntas
* si una organización documental permite separar investigación, producto e implementación
* si el modelo de dominio evoluciona mejor cuando las decisiones quedan trazadas
* si un artifact YAML puede actuar como evidencia de dominio y no solo como archivo de datos
* si VSlices evita congelar prematuramente una interpretación parcial del hogar

## Evidencia faltante

Todavía falta observar:

* qué Documents serán realmente necesarios
* qué Support Notes serán útiles y cuáles serán exceso
* qué paths ayudan a recorrer el caso sin checklist
* qué diagramas realmente reducen ambigüedad
* qué Nexus, si alguno, reduce fragmentación
* cómo evolucionará el artifact YAML hacia software
* qué parte del conocimiento doméstico se mantiene tácita
* qué decisiones serán estables después de uso real
* qué validaciones domésticas se podrán repetir
* qué efectos tendrá Tooling cuando empiece a apoyar artifacts
* qué límites tendrá Domus Orbis como caso publicable y personal

## Criterios iniciales de observación

El estudio puede considerar señales positivas si:

* los artifacts permiten recordar por qué se tomó una decisión
* el vocabulario doméstico se vuelve más claro
* los cambios de estructura se explican mejor
* las Support Notes preservan ideas sin forzar documentos grandes
* los Continuity Paths ayudan a conectar dominio, producto y software
* los diagramas ayudan a ver relaciones o clasificación
* el YAML se entiende como artifact de aprendizaje, no solo como datos
* se reduce la pérdida de conocimiento entre conversaciones, archivos y código
* las decisiones pueden revisarse sin depender solo de memoria

El estudio puede considerar señales problemáticas si:

* la documentación crece más rápido que el producto
* los diagramas se vuelven más complejos que el problema
* las Support Notes acumulan intuiciones sin cierre
* los paths se convierten en checklist
* los Documents se escriben antes de tener evidencia suficiente
* el artifact YAML se sobreinterpreta como modelo final
* el caso personal introduce sesgos difíciles de separar
* la comodidad de publicar el caso lleva a generalizar demasiado

## Riesgos metodológicos

### Riesgo de sobreformalizar un dominio doméstico

Domus Orbis puede parecer pequeño, pero su dominio puede volverse muy rico.

El estudio debe evitar convertir cada observación doméstica en artifact formal.

### Riesgo de confundir evidencia personal con generalidad

Que algo funcione en este hogar no implica que funcione para todos los hogares.

El caso puede sugerir patrones, no validarlos universalmente.

### Riesgo de congelar una interpretación temprana

Un artifact YAML inicial puede capturar una versión parcial del dominio.

Debe tratarse como evidencia evolutiva, no como modelo definitivo.

### Riesgo de entusiasmo por ser caso propio

Al ser un producto propio y publicable, existe riesgo de interpretar cada hallazgo como validación de VSlices.

El estudio debe registrar también fricciones, excesos, ambigüedades y mecanismos que no aporten.

### Riesgo de mezclar producto e investigación

Domus Orbis es simultáneamente producto, experimento y caso de investigación.

El estudio debe distinguir cuándo se está tomando una decisión de producto y cuándo se está produciendo evidencia para VSlices Research.

### Riesgo de privacidad doméstica

Aunque el caso sea publicable, algunas evidencias pueden exponer información personal, financiera, doméstica o relacional.

La publicación debe ser selectiva.

## Límites del estudio

Este estudio no puede demostrar que Docs Standard funciona en general.

No puede demostrar que Domus Orbis representa todos los dominios domésticos.

No puede validar universalmente VSlices como método de construcción de productos.

No debe concluir que toda automatización doméstica necesita la misma documentación.

No puede separar completamente diseño de producto, aprendizaje personal e investigación aplicada.

Su valor está en observar un producto real construido desde cero con VSlices, donde conocimiento tácito, artifacts, documentación, decisiones y software evolucionan juntos.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre descubrimiento de dominio doméstico
* Observations sobre artifacts YAML como evidencia de dominio
* Tensions entre automatización, descubrimiento y sobreformalización
* Findings locales sobre utilidad o límites de Documents, Support Notes, Paths, Organizations, Nexus y Diagrams
* ajustes candidatos a Docs Standard
* criterios para usar Domus Orbis como caso publicable
* aprendizajes para VSlices Method, Design, Framework y Tooling

## Relación con estudios fundacionales

Este estudio se relaciona especialmente con `STU-004`, donde se observa el riesgo de escape de conocimiento en contextos no digitalizados.

Domus Orbis permite observar cómo el conocimiento puede existir en práctica cotidiana antes de existir software.

También puede alimentar `SYN-0001` al mostrar un caso donde la continuidad puede romperse por escape inicial si el conocimiento tácito no se explora antes de digitalizar.

## Relación con Alive Lab

Domus Orbis es uno de los casos principales de Alive Lab.

Su valor no está en ser un ejemplo perfecto.

Su valor está en ser un laboratorio vivo donde VSlices puede observar:

* descubrimiento progresivo
* documentación mínima
* artifacts vivos
* decisiones revisables
* evolución del modelo
* continuidad entre uso real y software
* límites de aplicar VSlices en un producto pequeño
* retroalimentación entre producto e investigación

## Límite actual

Este estudio debe mantenerse en estado `candidate` mientras no se haya revisado evidencia suficiente.

El caso es metodológicamente valioso porque nace desde cero, es real y puede publicarse con bastante transparencia.

Sin embargo, sus conclusiones deben formularse con prudencia porque el dominio es personal, el producto está en construcción y la investigación forma parte activa del proceso de diseño.


## Alcance del estudio

Este estudio cubre una versión inicial acotada de Domus Orbis.

El alcance actual corresponde a una v0.N del producto, no al producto completo.

Hasta ahora, Domus Orbis tiene definidas funcionalidades suficientes para aproximadamente tres o cuatro iteraciones iniciales.

El estudio observa principalmente:

* descubrimiento de dominio doméstico
* artifacts iniciales de planificación y compra
* automatización y simplificación de procesos
* decisiones documentales y de dominio
* continuidad entre observación doméstica, artifact, documentación y software inicial
* evolución de una primera base de producto

El estudio no busca validar Domus Orbis como SaaS completo ni como producto terminado.

Su foco está en observar cómo VSlices ayuda o no ayuda durante la construcción progresiva de una versión temprana del producto.

## Fuera de alcance

Queda fuera de alcance:

* validar el producto completo
* cubrir todas las funcionalidades futuras de Domus Orbis
* generalizar el dominio doméstico a todos los hogares
* asumir que las primeras iteraciones representan la arquitectura final
* convertir artifacts YAML iniciales en modelo definitivo
* evaluar escalamiento comercial o adopción masiva
* validar todo VSlices Framework, Method o Tooling mediante este caso

El valor del estudio está en observar una v0.N real, acotada y publicable, donde conocimiento doméstico, documentación, decisiones y software evolucionan juntos.
