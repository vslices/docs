---
type: study
state: candidate
code: STU-009
visibility: internal-publicable
evidence_policy: direct-redacted

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

related_findings: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
* Surreal Atlas

---

# STU-009 — Tooling interno para generación y mantenimiento de artifacts documentales

## Estado

candidate

## Visibilidad

internal-publicable

## Política de evidencia

Este estudio trabaja con un caso real de herramienta interna asociada a VSlices.

El caso puede usar evidencia directa cuando sea conveniente, pero no necesariamente debe exponer todos los detalles internos de diseño, implementación, automatización o roadmap.

La evidencia podrá utilizarse en forma de:

* artifacts generados
* templates
* front-matter
* reglas de validación
* ejemplos de entrada y salida
* decisiones de diseño
* commits o fragmentos de código cuando sea adecuado
* diagramas
* observaciones de uso
* errores detectados
* ajustes derivados del uso real
* ejemplos simplificados o redactados

La política candidata es:

> Publicar la evidencia suficiente para evaluar la utilidad del tooling sin obligar a publicar toda su implementación interna o decisiones todavía inestables.

## Contexto

Este estudio ocurre en VSlices Tooling, una herramienta interna orientada a apoyar la generación, mantenimiento, validación o navegación de artifacts documentales definidos por VSlices Docs Standard.

El caso aparece como una necesidad práctica: Docs Standard define mecanismos documentales candidatos, pero esos mecanismos pueden volverse costosos, inconsistentes o difíciles de mantener si dependen solo de autoría manual.

Tooling intenta observar qué partes del estándar pueden apoyarse mediante automatización sin convertir Docs Standard en un sistema rígido, burocrático o prematuramente cerrado.

Este caso es especialmente importante porque conecta investigación, documentación y operación:

> VSlices Tooling permite observar qué conceptos de Docs Standard son suficientemente claros como para ser asistidos por herramientas, y cuáles todavía necesitan exploración humana antes de automatizarse.

## Situación observada

Docs Standard propone artifacts, front-matter, preguntas principales, relaciones, paths, nexus, support notes, organizaciones documentales y diagramas.

En la práctica, mantener esos elementos manualmente puede introducir problemas como:

* errores de consistencia
* front-matter incompleto
* nombres de archivo divergentes
* metadata derivada escrita manualmente
* duplicación de datos
* relaciones rotas
* templates usados de forma inconsistente
* dificultad para navegar artifacts
* dificultad para generar índices
* dificultad para validar estructura mínima
* exceso de esfuerzo para mantener diagramas o proyecciones

Al mismo tiempo, automatizar demasiado temprano puede congelar conceptos que todavía están en estado `candidate`.

## Problema de continuidad

El problema central es preservar continuidad entre el modelo documental y su uso real.

Docs Standard puede perder continuidad si:

* sus reglas viven solo en documentos conceptuales
* los artifacts reales no siguen las convenciones
* la metadata no puede usarse para navegación
* los paths no se conectan con artifacts existentes
* los nexus no pueden resolverse
* las organizaciones no pueden proyectarse
* los diagramas quedan desactualizados
* el costo manual impide mantener artifacts vivos

Pero también puede perder continuidad si Tooling impone reglas demasiado pronto.

La tensión central es:

> Automatizar lo suficiente para sostener continuidad, sin convertir exploración documental en rigidez técnica prematura.

## Pregunta local del estudio

¿Qué aspectos de VSlices Docs Standard pueden ser apoyados por tooling sin convertir el estándar en una estructura rígida o prematuramente automatizada?

## RQs relacionadas

Este estudio puede alimentar varias preguntas de investigación de Docs Standard.

| RQ                                   | Relación con el estudio                                                                      |
| ------------------------------------ | -------------------------------------------------------------------------------------------- |
| [RQ-002 — Caminos de Continuidad](../questions/rq-002-continuity-paths.md)      | Observa si Tooling puede generar, validar o recorrer paths sin convertirlos en checklist     |
| [RQ-003 — Nexos Documentales](../questions/rq-003-document-nexus.md)          | Observa si Tooling puede resolver composición entre artifacts sin duplicar contenido         |
| [RQ-004 — Documentos](../questions/rq-004-documents.md)                  | Observa si Tooling puede generar o validar Documents definidos por preguntas principales     |
| [RQ-005 — Organizaciones Documentales](../questions/rq-005-documental-organization.md) | Observa si Tooling puede proyectar organizaciones sin duplicar fuente de verdad              |
| [RQ-006 — Notas de Soporte](../questions/rq-006-support-notes.md)            | Observa si Tooling puede crear, mantener o cerrar Support Notes sin volverlas burocráticas   |
| [RQ-007 — Diagramas Documentales](../questions/rq-007-diagrams.md)      | Observa si Tooling puede generar o validar diagramas útiles sin imponer simbología prematura |

Aunque el caso puede alimentar varias RQs, no debe intentar validarlas todas con el mismo peso.

Su foco principal debería ser `RQ-004`, `RQ-005`, `RQ-006` y `RQ-007`.

## Mecanismos de Docs Standard observados

### Document artifacts

Tooling puede observar si es posible asistir Documents mediante:

* generación de templates
* front-matter base
* preguntas principales
* segmentos recomendados
* nombres derivados
* slugs derivados
* rutas sugeridas
* validación de campos fuente de verdad
* advertencias de metadata faltante
* detección de campos derivados escritos manualmente
* generación de índices

La observación clave no es si Tooling puede generar muchos archivos.

La observación clave es si genera artifacts útiles, pequeños y coherentes con intención documental.

### Support Notes

Tooling puede observar si es posible apoyar Support Notes mediante:

* creación rápida de notas auxiliares
* vinculación con artifacts soportados
* templates por tipo de nota
* validación de objeto soportado
* detección de notas sin cierre
* sugerencia de promoción a Document artifact
* diferenciación entre draft, result, validation, testing-spec, risk y external

La tensión principal es evitar que Tooling transforme cada duda o resultado en archivo permanente sin ciclo de vida.

### Nexus artifacts

Tooling puede observar si es posible apoyar Nexus mediante:

* declaración de artifacts compuestos
* validación de referencias
* detección de composición incompleta
* generación de vistas de composición
* navegación desde un target compuesto
* prevención de duplicación de contenido
* reporte de artifacts faltantes

La tensión principal es que el Nexus debe reducir fragmentación real, no existir solo porque Tooling puede generarlo.

### Continuity Paths

Tooling puede observar si es posible apoyar Continuity Paths mediante:

* generación de estructura base
* validación de paths relacionados
* detección de artifacts conectados
* identificación de nodos sin artifact
* generación de diagramas
* navegación por rutas principales y auxiliares
* advertencias contra checklist
* soporte para nodos documentados, identificados o candidatos

La tensión principal es preservar la naturaleza orientadora del path.

Tooling no debe convertir cada nodo en tarea obligatoria.

### Organizaciones documentales

Tooling puede observar si es posible apoyar organizaciones mediante:

* generación de índices
* proyecciones navegables
* agrupación por metadata
* validación de fuente de verdad
* detección de duplicación
* navegación por proyecto, producto, capability, path o study
* exportación hacia Surreal Atlas
* construcción de TreeViews o mapas

La tensión principal es diferenciar organización, proyección y fuente canónica.

### Diagramas documentales

Tooling puede observar si es posible apoyar diagramas mediante:

* generación Mermaid
* validación de simbología
* detección de nodos sin leyenda
* generación desde metadata
* actualización parcial de diagramas
* integración con paths, nexus u organizaciones
* detección de diagramas demasiado grandes
* exportación hacia visualizaciones más ricas

La tensión principal es no automatizar una semántica visual todavía exploratoria.

## Evidencia disponible

La evidencia inicial esperada puede incluir:

* templates de artifacts
* front-matter base
* comandos o prototipos de generación
* examples de Documents generados
* examples de Support Notes generadas
* validaciones aplicadas
* errores o warnings detectados
* decisiones sobre metadata fuente de verdad
* decisiones sobre campos derivados
* diagramas generados o mantenidos
* proyecciones documentales
* integración candidata con Surreal Atlas
* observaciones de uso manual
* ajustes derivados de fricción real

La evidencia puede publicarse directamente cuando no exponga detalles internos inestables o innecesarios.

Cuando corresponda, puede publicarse en forma simplificada.

## Observaciones esperadas

Este estudio podría permitir observar:

* si Tooling reduce esfuerzo de crear artifacts
* si Tooling mejora consistencia sin imponer rigidez excesiva
* si los campos derivados deben mantenerse fuera del front-matter manual
* si los templates ayudan o vuelven rígida la escritura
* si la validación detecta problemas reales
* si los warnings ayudan a mejorar artifacts
* si las proyecciones navegables pueden generarse sin duplicar contenido
* si los diagramas generados son comprensibles
* si las Support Notes requieren ciclo de vida
* si Nexus y Continuity Paths pueden resolverse desde metadata
* si Tooling debe limitarse a sugerir en vez de corregir automáticamente

## Evidencia faltante

Todavía falta observar:

* qué comandos serán realmente necesarios
* qué partes de Docs Standard son automatizables
* qué partes deben permanecer manuales
* qué validaciones son útiles
* qué validaciones resultan molestas o prematuras
* qué artifacts se generan correctamente
* qué artifacts requieren intervención humana significativa
* qué diagramas pueden generarse desde metadata
* qué diagramas deben diseñarse manualmente
* qué proyecciones necesita Surreal Atlas
* qué límites aparecen al aplicar Tooling sobre casos reales
* qué reglas de Docs Standard están demasiado inmaduras para automatizar

## Criterios iniciales de observación

El estudio puede considerar señales positivas si:

* Tooling reduce errores repetitivos
* Tooling evita escribir metadata derivada manualmente
* Tooling genera artifacts mínimos útiles
* Tooling ayuda a mantener relaciones entre artifacts
* Tooling produce warnings accionables
* Tooling facilita navegación o proyecciones
* Tooling ayuda a detectar duplicación de fuente de verdad
* Tooling mantiene los artifacts editables por humanos
* Tooling permite trabajar sin exigir completitud
* Tooling ayuda a Surreal Atlas sin reemplazar Docs Standard

El estudio puede considerar señales problemáticas si:

* Tooling fuerza estructura antes de que el concepto esté validado
* Tooling genera demasiados artifacts
* Tooling convierte recomendaciones en reglas rígidas
* Tooling oculta intención documental detrás de comandos
* Tooling hace más difícil escribir manualmente
* Tooling produce diagramas que nadie entiende
* Tooling valida reglas que aún están en exploración
* Tooling incentiva crear Nexus, Paths o Support Notes innecesarios
* Tooling convierte Docs Standard en framework técnico antes de tiempo

## Riesgos metodológicos

### Riesgo de automatización prematura

Un concepto candidate no debería convertirse demasiado pronto en regla técnica estricta.

Tooling debe acompañar la investigación, no cerrarla artificialmente.

### Riesgo de confundir consistencia con continuidad

Un artifact puede estar bien formado y aun así no preservar conocimiento útil.

La validación sintáctica no equivale a continuidad documental.

### Riesgo de generar ceremonia por facilidad técnica

Si Tooling facilita crear artifacts, puede incentivar producir más documentación de la necesaria.

### Riesgo de esconder complejidad conceptual

Un comando puede parecer simple aunque el modelo documental detrás siga siendo inmaduro.

### Riesgo de dependencia de herramienta

Docs Standard debería tener valor conceptual sin depender completamente de Tooling.

### Riesgo de validar por comodidad del autor

Si Tooling lo usa principalmente quien diseña VSlices, puede parecer más útil de lo que sería para otra persona.

### Riesgo de acoplar Tooling a Surreal Atlas demasiado pronto

Tooling puede preparar datos para Surreal Atlas, pero no debe asumir que toda documentación necesita visualización avanzada.

## Límites del estudio

Este estudio no puede demostrar que Docs Standard funciona en general.

No puede demostrar que Tooling sea necesario para aplicar Docs Standard.

No puede validar universalmente una estructura de front-matter, templates o diagramas.

No debe concluir que todo artifact debe generarse mediante herramientas.

No puede aislar completamente el valor del tooling frente a la claridad previa del modelo documental.

Su valor está en observar qué partes de Docs Standard pueden ser asistidas de forma útil por herramientas internas y qué partes deben permanecer exploratorias, manuales o flexibles.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre generación de artifacts
* Observations sobre metadata fuente de verdad y campos derivados
* Tensions entre automatización y exploración
* Tensions entre consistencia formal y continuidad real
* Findings locales sobre utilidad o límites de Tooling
* ajustes candidatos a Docs Standard
* criterios para decidir qué automatizar
* criterios para decidir qué mantener manual
* requisitos candidatos para Surreal Atlas
* límites explícitos sobre automatización prematura

## Relación con estudios fundacionales

Este estudio se relaciona con `RQ-001` porque observa cómo una línea de investigación sobre continuidad puede transformarse en soporte operativo sin perder raíz práctica.

También se relaciona con `RN-0002`, porque prueba la operacionalización de mecanismos documentales candidatos.

Y se relaciona con `RN-0003`, porque puede observar si los diagramas documentales pueden generarse o mantenerse mediante reglas mínimas.

## Relación con Alive Lab

VSlices Tooling es un caso interno de Alive Lab.

Su valor no está en demostrar que la automatización es deseable.

Su valor está en observar cuándo la automatización ayuda a preservar continuidad y cuándo convierte una práctica flexible en estructura rígida.

Tooling también actúa como puente hacia Surreal Atlas, porque puede preparar artifacts, metadata, relaciones o proyecciones necesarias para generar atlas locales.

## Límite actual

Este estudio debe mantenerse en estado `candidate` mientras no se haya revisado evidencia suficiente.

El caso es metodológicamente valioso porque transforma Docs Standard en práctica operativa.

Sin embargo, sus conclusiones deben formularse con prudencia porque Tooling puede reforzar tanto las partes valiosas como las partes inmaduras del estándar.
