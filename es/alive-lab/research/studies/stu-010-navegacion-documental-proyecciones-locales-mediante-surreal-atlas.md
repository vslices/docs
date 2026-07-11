---
type: study
state: candidate
code: STU-010
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

related_findings: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
* Surreal Atlas
---

# STU-010 — Navegación documental y proyecciones locales mediante Surreal Atlas

## Estado

candidate

## Visibilidad

public

## Política de evidencia

Este estudio trabaja con un caso real, propio y publicable.

Surreal Atlas puede usar evidencia directa cuando sea conveniente:

* artifacts documentales
* metadata
* relaciones entre documents
* proyecciones navegables
* diagramas
* capturas o representaciones de atlas locales
* decisiones de diseño
* ejemplos de navegación
* commits
* estructuras de archivos
* outputs de Tooling
* observaciones de uso
* cambios derivados del uso real

Aun así, si Surreal Atlas visualiza documentación privada de otros casos, esa evidencia debe redactarse, simplificarse o reemplazarse por ejemplos sintéticos.

La regla candidata es:

> Surreal Atlas puede ser publicable como producto y como caso de investigación, pero no toda documentación visualizada por Surreal Atlas es automáticamente publicable.

## Contexto

Este estudio ocurre en Surreal Atlas, un producto orientado a navegar, visualizar y explorar documentación local o estructurada.

Surreal Atlas aparece como una respuesta a un problema práctico: incluso cuando existen documentos, su valor disminuye si las relaciones entre ellos no son visibles, navegables o explorables.

Docs Standard define artifacts, relaciones, continuidad, composiciones, organizaciones y proyecciones.

Tooling puede generar o preparar metadata, templates y estructuras.

Surreal Atlas puede observar si esas piezas permiten construir experiencias de navegación documental útiles.

> Surreal Atlas permite estudiar cómo hacer visible la continuidad documental sin convertir la visualización en fuente de verdad.

## Situación observada

En muchos proyectos, la documentación existe, pero queda atrapada en archivos, carpetas, índices o convenciones difíciles de recorrer.

El problema no siempre es ausencia de documentos.

A veces el problema es que no se puede ver fácilmente:

* qué documents existen
* cómo se relacionan
* qué artifact explica qué pregunta
* qué paths conectan conceptos
* qué nexus componen artifacts
* qué notas apoyan una explicación
* qué documentos pertenecen a una organización
* qué proyección conviene usar para un lector específico
* qué conocimiento está vigente, candidate, deprecated o superseded
* qué relaciones son estructurales y cuáles son auxiliares
* qué parte del mapa documental está incompleta

Surreal Atlas permite observar si una herramienta visual puede mejorar la exploración de ese conocimiento sin duplicarlo.

## Problema de continuidad

El problema central es preservar continuidad navegable entre artifacts.

Docs Standard puede definir relaciones, pero esas relaciones pueden perder valor si no se pueden recorrer.

La continuidad puede romperse si:

* los artifacts existen, pero no son visibles como red
* los paths no se pueden seguir
* los nexus no se pueden explorar
* las organizaciones solo viven como intención
* las proyecciones duplican contenido
* los diagramas quedan estáticos o desactualizados
* las relaciones no distinguen composición, apoyo, navegación, continuidad o referencia
* los lectores no saben qué artifact revisar primero

Surreal Atlas observa la capa de navegación y representación de esa continuidad.

## Pregunta local del estudio

¿Cómo ayudan las proyecciones navegables y visualizaciones documentales a recorrer artifacts relacionados sin duplicar contenido ni reemplazar la fuente de verdad?

## RQs relacionadas

Este estudio puede alimentar varias preguntas de investigación de Docs Standard.

| RQ                                   | Relación con el estudio                                                                       |
| ------------------------------------ | --------------------------------------------------------------------------------------------- |
| [RQ-002 — Caminos de Continuidad](../questions/rq-002-continuity-paths.md)      | Observa si los paths pueden recorrerse visualmente o mediante navegación local                |
| [RQ-003 — Nexos Documentales](../questions/rq-003-document-nexus.md)          | Observa si la composición entre artifacts puede visualizarse sin duplicar contenido           |
| [RQ-004 — Documentos](../questions/rq-004-documents.md)                  | Observa si los Documents son navegables como unidades de explicación                          |
| [RQ-005 — Organizaciones Documentales](../questions/rq-005-documental-organization.md) | Observa directamente fuente de verdad, organización, proyección y navegación                  |
| [RQ-006 — Notas de Soporte](../questions/rq-006-support-notes.md)            | Observa si Support Notes pueden aparecer como apoyo sin competir con Documents                |
| [RQ-007 — Diagramas Documentales](../questions/rq-007-diagrams.md)      | Observa si diagramas y visualizaciones representan necesidades documentales de forma efectiva |

Aunque el caso puede alimentar varias RQs, no debe intentar validarlas todas con el mismo peso.

Su foco principal debería ser `RQ-005`, `RQ-007`, `RQ-003` y `RQ-002`.

## Mecanismos de Docs Standard observados

### Organizaciones documentales

Surreal Atlas puede observar de forma directa la separación entre:

* fuente de verdad documental
* organización documental
* proyección navegable
* navegación
* visualización

Este es probablemente el mecanismo más importante para este estudio.

La fuente de verdad puede vivir en archivos Markdown, repositorios, metadata o artifacts canónicos.

La organización puede definirse por criterios como:

* producto
* proyecto
* capability
* continuity path
* nexus
* study
* research question
* dominio
* etapa
* estado
* tipo documental

La proyección navegable puede mostrarse como:

* árbol
* grafo
* mapa local
* lista agrupada
* recorrido
* vista por relaciones
* vista por estado
* vista por target

Surreal Atlas permite observar si esa separación reduce duplicación o si introduce una capa extra difícil de mantener.

### Continuity Paths

Surreal Atlas puede observar si los Continuity Paths son navegables.

Un path puede aparecer como:

* recorrido visual
* secuencia de artifacts
* grafo de conceptos
* mapa de perspectivas
* vista de nodos documentados y candidatos
* ruta recomendada de lectura
* cambio entre paths relacionados

La pregunta no es solo si se puede mostrar un path.

La pregunta es si verlo ayuda a preservar continuidad.

### Nexus artifacts

Surreal Atlas puede observar si un Nexus puede visualizarse como composición.

Por ejemplo:

* Capability Nexus
* Service Consumption Nexus
* composición de artifacts alrededor de un target
* artifacts faltantes
* artifacts existentes
* roles de composición
* relaciones estructurales y auxiliares

La visualización debe apoyar la lectura del Nexus, no reemplazarlo.

### Document artifacts

Surreal Atlas puede observar si los Documents funcionan como unidades navegables de explicación.

Puede mostrar:

* tipo documental
* pregunta principal
* target
* estado
* relaciones
* artifacts relacionados
* paths asociados
* notes de soporte
* nexus donde participa
* organizaciones donde aparece

Esto puede ayudar a validar si la metadata mínima de Documents es suficiente para navegación.

### Support Notes

Surreal Atlas puede observar si las Support Notes pueden aparecer como apoyo sin ocupar el lugar de Documents.

Puede mostrar:

* qué artifact soportan
* qué tipo de nota son
* qué estado tienen
* si están abiertas, cerradas o candidatas
* si podrían requerir promoción
* si acumulan demasiada información auxiliar

La visualización puede ayudar a detectar notas huérfanas o exceso de notas.

### Diagramas documentales

Surreal Atlas puede observar si los diagramas documentales tienen una versión visual más interactiva o navegable.

Puede explorar:

* diagramas Mermaid embebidos
* diagramas generados desde metadata
* grafos locales
* relaciones expandibles
* nodos con estados documentales
* mapas de continuity paths
* mapas de nexus
* proyecciones visuales de organizaciones

La pregunta clave es si esas visualizaciones reducen incertidumbre o solo agregan estética.

## Relación con Tooling

Surreal Atlas construye sobre necesidades que Tooling puede preparar.

Tooling puede generar o validar:

* front-matter
* metadata
* relaciones
* índices
* diagramas Mermaid
* projections
* archivos intermedios
* mapas de artifacts
* outputs consumibles por Surreal Atlas

Surreal Atlas puede consumir esa información para generar navegación local o experiencias visuales.

La relación candidata es:

```text id="3t03uk"
Docs Standard define artifacts y relaciones
Tooling prepara, valida o genera metadata
Surreal Atlas visualiza y permite navegar proyecciones
```

Esta relación es candidata y debe observarse en uso real.

Tooling no debería producir datos solo porque Surreal Atlas puede mostrarlos.

Surreal Atlas no debería obligar a Docs Standard a capturar metadata innecesaria.

## Evidencia disponible

La evidencia inicial esperada puede incluir:

* modelo conceptual de Surreal Atlas
* documents de VSlices Docs Standard
* outputs de Tooling
* metadata de artifacts
* relaciones entre documents
* ejemplos de organizations
* examples de projections
* views de atlas local
* diagrams generados o visualizados
* decisiones de diseño del producto
* navegación sobre Domus Orbis
* navegación sobre Docs Standard
* navegación sobre estudios de VSlices Research
* observaciones de uso
* feedback propio o de lectores
* comparación entre navegación Markdown e interfaz visual

La evidencia puede publicarse directamente cuando no exponga contenido privado de otros casos.

## Observaciones esperadas

Este estudio podría permitir observar:

* si las proyecciones navegables ayudan a explorar artifacts
* si Surreal Atlas reduce fricción para encontrar conocimiento relacionado
* si las relaciones de Docs Standard son suficientemente explícitas
* si la metadata actual permite navegación útil
* si los Continuity Paths se entienden mejor como recorrido visual
* si los Nexus se entienden mejor como composición visual
* si las Support Notes aparecen como apoyo y no como ruido
* si los diagrams ayudan o se vuelven redundantes frente a vistas interactivas
* si una visualización permite detectar gaps documentales
* si la separación entre fuente de verdad y proyección se mantiene clara
* si Tooling produce suficiente información para construir atlas locales

## Evidencia faltante

Todavía falta observar:

* qué estructura mínima necesita Surreal Atlas para navegar artifacts
* qué metadata es realmente necesaria
* qué relaciones son útiles para lectores
* qué relaciones generan ruido
* qué vistas aportan más valor
* qué vistas son innecesarias
* si los usuarios entienden la diferencia entre Document, Note, Nexus, Path y Organization
* si la visualización ayuda sin reemplazar lectura
* si el atlas puede mantenerse localmente
* si Surreal Atlas debe consumir Markdown directo, output de Tooling o ambos
* si la navegación visual ayuda en casos privados redactados
* si la visualización escala sin convertirse en mapa ilegible

## Criterios iniciales de observación

El estudio puede considerar señales positivas si:

* los usuarios encuentran artifacts relacionados más rápido
* las relaciones entre documents son más claras
* las proyecciones no duplican contenido
* los paths se pueden recorrer sin checklist
* los Nexus se entienden como composición
* las Support Notes no saturan la navegación
* los diagramas o vistas visuales reducen ambigüedad
* se detectan gaps documentales
* se mantiene clara la fuente de verdad
* Tooling y Surreal Atlas se complementan sin acoplarse demasiado
* las vistas pueden generarse desde información ya justificada por Docs Standard

El estudio puede considerar señales problemáticas si:

* Surreal Atlas exige metadata que Docs Standard no necesita
* la visualización se vuelve más importante que el artifact
* las proyecciones duplican contenido canónico
* los grafos se vuelven ilegibles
* las relaciones generan ruido
* los usuarios exploran mucho pero entienden poco
* los paths se convierten en navegación decorativa
* los Nexus se perciben como carpetas visuales sin intención
* las Support Notes aparecen como desorden
* Tooling produce estructura solo para alimentar visualización
* el atlas oculta límites, estados o incertidumbre documental

## Riesgos metodológicos

### Riesgo de confundir navegación con continuidad

Que un usuario pueda navegar más cosas no significa que la continuidad de conocimiento haya mejorado.

La investigación debe observar si la navegación preserva intención, relación, contexto o trazabilidad útil.

### Riesgo de visualización como falsa madurez

Una interfaz visual puede hacer que artifacts inmaduros parezcan más estables de lo que son.

Los estados `candidate`, `draft`, `deprecated` o `superseded` deben mantenerse visibles.

### Riesgo de duplicar fuente de verdad

Surreal Atlas debe visualizar o proyectar información.

No debe convertirse en una fuente paralela de contenido canónico salvo que esa responsabilidad se defina explícitamente.

### Riesgo de agregar metadata por la herramienta

Docs Standard no debería capturar campos solo porque Surreal Atlas podría mostrarlos.

La metadata debe existir porque preserva continuidad, no porque mejora una interfaz.

### Riesgo de acoplar investigación y producto demasiado pronto

Surreal Atlas es producto y caso de investigación.

El estudio debe distinguir decisiones de producto de evidencia sobre Docs Standard.

### Riesgo de grafos ilegibles

Las relaciones documentales pueden crecer rápidamente.

Un grafo completo puede ser menos útil que una vista local, filtrada o contextual.

### Riesgo de extrapolar desde casos propios

Surreal Atlas puede funcionar bien con VSlices porque fue diseñado junto a VSlices.

Eso no demuestra automáticamente utilidad en otros ecosistemas documentales.

## Límites del estudio

Este estudio no puede demostrar que toda documentación necesita visualización avanzada.

No puede demostrar que Surreal Atlas sea necesario para aplicar Docs Standard.

No puede validar universalmente un modelo de navegación documental.

No puede asumir que más relaciones visibles equivalen a mayor comprensión.

No debe concluir que Docs Standard debe adaptarse a todas las necesidades de Surreal Atlas.

Su valor está en observar cómo proyecciones navegables y visualizaciones pueden apoyar continuidad documental sin reemplazar artifacts ni duplicar fuentes de verdad.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre navegación documental
* Observations sobre proyecciones locales
* Tensions entre visualización, fuente de verdad y metadata
* Tensions entre exploración visual y comprensión real
* Findings locales sobre utilidad o límites de Surreal Atlas
* ajustes candidatos a Docs Standard
* requisitos candidatos para Tooling
* criterios para decidir qué visualizar
* criterios para evitar grafos o vistas excesivas
* límites explícitos sobre visualización como mecanismo de continuidad

## Relación con estudios fundacionales

Este estudio se relaciona con `RQ-001` porque observa una forma concreta de preservar continuidad de conocimiento mediante navegación y visualización.

También se relaciona con `RN-0002`, porque explora cómo los mecanismos de Docs Standard pueden proyectarse y recorrerse.

Y se relaciona con `RN-0003`, porque Surreal Atlas puede observar una versión más rica de la representación visual que los diagramas Markdown iniciales.

## Relación con Alive Lab

Surreal Atlas es uno de los casos principales de Alive Lab.

Su valor no está en ser una vitrina visual de VSlices.

Su valor está en observar si la continuidad documental mejora cuando los artifacts, relaciones, paths, nexus y organizaciones pueden explorarse visualmente.

Surreal Atlas también permite validar una frontera importante:

> Una visualización puede ayudar a recorrer conocimiento, pero no debería reemplazar el artifact que lo preserva.

## Relación con Domus Orbis y Tooling

Surreal Atlas puede apoyarse en los aprendizajes de Domus Orbis y Tooling.

Domus Orbis puede proveer un caso real de producto, dominio y documentación viva.

Tooling puede proveer metadata, validaciones y outputs.

Surreal Atlas puede mostrar cómo esos artifacts se navegan, se conectan y se proyectan.

La relación candidata es:

```text id="zcwaj9"
Domus Orbis produce evidencia viva de producto y dominio
Tooling prepara artifacts, metadata y relaciones
Surreal Atlas permite navegar y visualizar esas relaciones
```

Esta relación debe observarse progresivamente, no asumirse como arquitectura definitiva.

## Límite actual

Este estudio debe mantenerse en estado `candidate` mientras no se haya revisado evidencia suficiente.

El caso es metodológicamente valioso porque permite observar Docs Standard desde navegación, proyección, visualización y producto.

Sin embargo, sus conclusiones deben formularse con prudencia porque Surreal Atlas está construido junto a VSlices, puede reforzar sus supuestos y puede hacer que relaciones candidatas parezcan más maduras de lo que realmente son.


## Alcance del estudio

Este estudio cubre Surreal Atlas como producto de navegación documental y proyecciones locales, pero su avance depende de una base previa de VSlices Tooling.

Surreal Atlas puede avanzar conceptualmente en paralelo, pero su validación práctica requiere que Tooling tenga definida una base suficiente para generar, mantener o exponer artifacts, metadata, relaciones y proyecciones.

El alcance inicial de este estudio incluye:

* exploración de navegación documental
* proyecciones locales
* visualización de relaciones entre artifacts
* consumo de outputs generados o preparados por Tooling
* navegación de Documents, Support Notes, Nexus y Continuity Paths
* representación visual de organizaciones documentales
* exploración de atlas locales
* relación entre fuente de verdad y visualización
* validación progresiva de Surreal Atlas como capa SaaS sobre capacidades habilitadas por Tooling

Surreal Atlas se entiende como una capa de producto más cercana al SaaS, mientras Tooling actúa como base operativa para preparar la información que el atlas puede navegar o visualizar.

## Fuera de alcance

Queda fuera de alcance:

* validar Surreal Atlas antes de contar con una base suficiente de Tooling
* asumir que toda visualización documental requiere Surreal Atlas
* convertir Surreal Atlas en fuente de verdad documental
* forzar metadata en Docs Standard solo para alimentar visualizaciones
* validar un SaaS empresarial completo en la primera etapa
* cubrir todos los posibles sabores o flavors de atlas
* evaluar adopción empresarial amplia antes de validar navegación local básica

El valor del estudio está en observar cómo Surreal Atlas puede construir sobre Tooling para navegar, proyectar y visualizar continuidad documental sin reemplazar los artifacts que preservan el conocimiento.
