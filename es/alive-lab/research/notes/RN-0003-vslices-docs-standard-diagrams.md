---
type: research-note
state: candidate
code: RN-0003

related_questions:
* RQ-001
* RQ-002
* RQ-003
* RQ-004
* RQ-005
* RQ-006

related_notes:
* RN-0001
* RN-0002

related_synthesis:
* SYN-0001

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Tooling
* Surreal Atlas
---

# RN-0003 — Diagramas como representación visual exploratoria en VSlices Docs Standard

## Tipo

research-note

## Estado

candidate

## Propósito

Esta nota registra una línea exploratoria de VSlices Docs Standard:

> Los diagramas podrían actuar como representaciones visuales de necesidades documentales, relaciones, recorridos, preguntas, estados o estructuras que otros artifacts de Docs Standard deben explicar, apoyar, componer, conectar u organizar.

La nota no propone todavía una familia formal de artifacts.

Tampoco valida una semántica visual definitiva.

Su propósito es separar el problema de representación visual del resto de los mecanismos documentales ya identificados en [RN-0002](../notes/RN-0002-vslices-docs-standard.md).

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

La pregunta fundacional estudia qué problema práctico dio origen a VSlices y cómo ese problema puede transformarse en una línea de investigación aplicada sobre continuidad de conocimiento sin perder su raíz práctica.

Esta nota explora una dimensión específica de ese problema:

> ¿Cómo hacer visibles relaciones, recorridos, ramificaciones o necesidades documentales sin convertir el diagrama en la fuente principal de conocimiento?

## Notas relacionadas

[RN-0001 — Superficies de continuidad en VSlices](../notes/RN-0001-superficies-continuidad-vslices.md)

`RN-0001` propone observar VSlices como una suite compuesta por distintas superficies de continuidad.

[RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0002-vslices-docs-standard.md)

`RN-0002` propone observar Docs Standard como una superficie documental compuesta por mecanismos candidatos como:

* Document artifacts
* Support Notes
* Nexus artifacts
* Continuity Paths
* Organizaciones documentales

Esta nota toma una línea más exploratoria dentro de Docs Standard: la representación visual mediante diagramas.

## Idea central

Hasta ahora, los mecanismos principales de Docs Standard tienen responsabilidades relativamente claras:

| Mecanismo                   | Responsabilidad                         |
| --------------------------- | --------------------------------------- |
| Document artifacts          | Explican                                |
| Support Notes               | Apoyan, registran o referencian         |
| Nexus artifacts             | Componen                                |
| Continuity Paths            | Conectan y orientan continuidad         |
| Organizaciones documentales | Ordenan                                 |
| Proyecciones navegables     | Muestran organizaciones                 |
| Navigation Documents        | Explican cómo recorrer una organización |

Los diagramas tienen una responsabilidad distinta:

> Los diagramas representan visualmente.

Esto significa que un diagrama puede mostrar relaciones, recorridos, estados o preguntas, pero no debería reemplazar el artifact que preserva la explicación principal.

## Nivel de exploración

Esta línea es más exploratoria que las preguntas anteriores sobre Docs Standard.

Los diagramas todavía no deberían tratarse como una familia formal estable dentro del estándar.

Por ahora, deben entenderse como **representaciones asociadas** que ayudan a mostrar necesidades documentales.

La razón es que todavía falta observar:

* qué tipos de diagramas necesita realmente Docs Standard
* qué semántica visual es comprensible
* qué convenciones deberían mantenerse
* qué puede representarse con Mermaid
* qué requiere tooling o visualización externa
* qué parte debe vivir en texto
* qué parte puede vivir en diagrama
* cuándo un diagrama ayuda
* cuándo agrega ceremonia visual

## Diagramas candidatos actuales

Hasta ahora existen dos diagramas candidatos principales.

| Diagrama                              | Necesidad que intenta representar                                                                                                    |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Diagrama de Camino de Continuidad     | Representar recorridos de continuidad, preguntas orientadoras, conceptos conectados, artifacts existentes y necesidades documentales |
| Diagrama de Ramificación de Preguntas | Representar cómo una pregunta documental principal se abre en preguntas derivadas, segmentos posibles o ramas de organización        |

Ambos deben entenderse como candidatos.

No constituyen todavía una taxonomía completa de diagramas para Docs Standard.

## Diagrama de Camino de Continuidad

El Diagrama de Camino de Continuidad representa visualmente un Continuity Path.

Su propósito candidato es mostrar:

* el concepto o target que se está siguiendo
* las preguntas orientadoras del recorrido
* los conceptos relacionados
* los artifacts asociados
* los conceptos ya documentados
* los conceptos identificados sin necesidad documental actual
* los conceptos con posible necesidad documental
* las rutas principales
* las rutas auxiliares

Este diagrama puede ayudar a hacer visible continuidad sin obligar a documentar todos los nodos.

### Posible aporte a continuidad

Puede ayudar a preservar continuidad cuando permite observar:

* qué relaciones son relevantes
* dónde existe documentación
* dónde falta documentación
* qué conceptos solo necesitan visibilidad
* qué recorrido seguir
* dónde cambiar de perspectiva
* cuándo detenerse

### Riesgo

Puede convertirse en checklist visual si cada nodo se interpreta como obligación documental.

También puede volverse ilegible si intenta representar demasiadas perspectivas, artifacts o relaciones al mismo tiempo.

## Diagrama de Ramificación de Preguntas

El Diagrama de Ramificación de Preguntas representa cómo una pregunta documental principal se abre en preguntas derivadas.

Su propósito candidato es ayudar a organizar un Document artifact sin imponer una plantilla rígida.

Puede mostrar:

* la pregunta principal del artifact
* preguntas derivadas
* ramas principales
* ramas auxiliares
* segmentos posibles
* preguntas que pueden quedar pendientes
* costo o esfuerzo candidato de incorporar una rama

Este diagrama no debería definir cómo debe verse el documento final.

Solo debería ayudar a razonar sobre qué preguntas podrían organizarlo.

### Posible aporte a continuidad

Puede ayudar a preservar continuidad cuando permite:

* entender qué pregunta principal organiza un artifact
* separar preguntas centrales de preguntas auxiliares
* evitar que cada rama se convierta automáticamente en sección
* decidir qué segmentos documentar ahora
* dejar visibles preguntas futuras sin tratarlas como deuda
* diferenciar importancia de costo documental

### Riesgo

Puede agregar ceremonia si el diagrama exige más esfuerzo que el documento que intenta orientar.

También puede inducir a transformar cada pregunta derivada en heading obligatorio.

## Mermaid como tecnología inicial

Hasta ahora, los diagramas candidatos se expresan mediante Mermaid.

Mermaid es útil porque:

* vive cerca del Markdown
* puede versionarse junto al documento
* puede revisarse en pull requests
* permite representar recorridos básicos
* no requiere herramientas pesadas
* puede ser renderizado por documentación estática

Sin embargo, Mermaid no debe confundirse con la teoría visual de VSlices.

Mermaid es una tecnología de representación inicial.

No define por sí sola:

* qué debe representarse
* qué semántica visual es correcta
* qué símbolos serán estables
* qué diagramas necesita Docs Standard
* qué debe validar Tooling
* qué debería visualizar Surreal Atlas

La regla candidata es:

> Mermaid es el soporte inicial de representación, no la fuente conceptual del modelo visual.

## Leyenda y simbología

Los diagramas candidatos requieren leyenda y simbología explícita.

Sin una leyenda clara, el diagrama puede parecer informativo sin ser interpretable.

La simbología puede representar cosas como:

* concepto documentado
* pregunta orientadora
* concepto identificado
* concepto con posible necesidad documental
* ruta principal
* ruta auxiliar
* esfuerzo bajo, medio o alto
* elemento externo
* artifact relacionado
* path relacionado

La simbología debe mantenerse pequeña.

Si la leyenda crece demasiado, el diagrama empieza a requerir documentación adicional para entender la documentación.

Eso sería una señal de sobreingeniería.

## Relación con Document artifacts

Los diagramas pueden apoyar a los Document artifacts, pero no deberían reemplazarlos.

Un Document artifact explica conocimiento desde una pregunta documental principal.

Un diagrama puede representar:

* la pregunta principal
* las preguntas derivadas
* los segmentos posibles
* relaciones con otros artifacts
* estructura conceptual del contenido

Pero la explicación debe seguir viviendo en el Document artifact.

### Riesgo

Si el diagrama contiene toda la explicación, deja de representar y empieza a competir con el documento.

## Relación con Support Notes

Los diagramas pueden ayudar a visualizar conocimiento auxiliar registrado en Support Notes.

Por ejemplo:

* un riesgo identificado
* una validación pendiente
* un resultado observado
* una referencia externa
* una hipótesis incompleta
* una necesidad documental candidata

Pero la Support Note debe seguir preservando el detalle.

El diagrama solo debería mostrar que la nota existe, qué rol cumple o dónde afecta la continuidad.

### Riesgo

El diagrama puede ocultar la incertidumbre real si transforma una nota exploratoria en un nodo que parece estable.

## Relación con Nexus artifacts

Los diagramas pueden representar composición documental.

Por ejemplo, un Capability Nexus puede mostrarse como una composición entre:

* Scope Document
* Behavior Document
* Structure Document
* Consistency Document
* Viability Document
* Decision Record
* Support Notes

Un Service Consumption Nexus puede mostrarse como composición entre:

* Support Note external
* Structure Document
* Behavior Document
* Consistency Document
* Scope Document
* Decision Record
* Testing Spec
* Risk

Pero el diagrama no debe reemplazar el Nexus.

El Nexus declara composición.

El diagrama muestra composición.

### Riesgo

Si el diagrama se convierte en la única declaración de composición, el modelo pierde trazabilidad estructurada.

## Relación con Continuity Paths

Los diagramas tienen una relación especialmente fuerte con Continuity Paths.

Un Continuity Path conecta y orienta continuidad.

El Diagrama de Camino de Continuidad muestra visualmente ese recorrido.

La distinción candidata es:

| Elemento                          | Responsabilidad                                                     |
| --------------------------------- | ------------------------------------------------------------------- |
| Continuity Path                   | Declara qué continuidad se sigue y qué artifacts o paths participan |
| Diagrama de Camino de Continuidad | Representa visualmente el recorrido                                 |
| Artifacts conectados              | Preservan el detalle                                                |
| Navigation Document               | Explica cómo recorrer una organización o proyección                 |

### Riesgo

Confundir el diagrama con el path completo puede producir pérdida de contenido, exceso visual o falta de trazabilidad.

## Relación con Organizaciones Documentales

Los diagramas pueden representar organizaciones documentales o proyecciones navegables.

Por ejemplo:

* TreeView documental
* mapa de artifacts por iniciativa
* mapa de artifacts por capability
* proyección por release
* proyección por caso de estudio
* visualización de artifacts relacionados

Sin embargo, una organización documental define un criterio de orden.

La proyección navegable muestra ese orden.

El diagrama puede ser una forma de proyección, pero no debería reemplazar la fuente de verdad ni duplicar contenido.

### Riesgo

Un diagrama de organización puede convertirse en una segunda fuente de verdad si empieza a copiar contenido canónico.

## Relación con Tooling

VSlices Tooling podría ayudar a generar, validar o actualizar diagramas.

Posibles usos futuros:

* generar diagramas desde metadata
* detectar nodos sin artifact asociado
* validar simbología
* detectar diagramas demasiado grandes
* mantener enlaces entre nodos y artifacts
* diferenciar nodos documentados de nodos candidatos
* representar segmentos activos y no activos
* sugerir diagramas mínimos

Pero Tooling no debería definir por sí solo qué diagrama es correcto.

Primero debe existir una intención documental clara.

Luego Tooling puede ayudar a materializarla.

### Riesgo

Automatizar diagramas antes de validar su utilidad puede producir mapas complejos que nadie usa.

## Relación con Surreal Atlas

Surreal Atlas puede ser un espacio natural para explorar representación visual de relaciones documentales.

Puede ayudar a observar:

* relaciones entre artifacts
* grafos locales de conocimiento
* proyecciones navegables
* continuity paths visuales
* composición de Nexus
* navegación espacial de documentos
* relaciones entre fuente de verdad y proyección

Sin embargo, Surreal Atlas no debe convertirse en requisito para que los diagramas tengan valor.

Los diagramas deben tener una versión mínima comprensible en Markdown o documentación estática antes de depender de visualización avanzada.

### Riesgo

Surreal Atlas puede hacer que una representación visual parezca más madura de lo que realmente está.

La visualización puede mejorar exploración sin necesariamente preservar continuidad.

## Hipótesis candidata

Los diagramas podrían ayudar a preservar continuidad documental cuando representan visualmente relaciones, preguntas, recorridos o necesidades documentales que serían difíciles de reconocer solo mediante texto.

Sin embargo, su valor depende de que:

* tengan una responsabilidad visual clara
* usen simbología comprensible
* no reemplacen artifacts
* no dupliquen contenido
* no obliguen a documentar cada nodo
* puedan mantenerse con esfuerzo razonable
* ayuden a tomar decisiones documentales
* reduzcan incertidumbre en vez de agregar complejidad

## Pregunta de investigación candidata

Esta nota abre una pregunta de investigación propia:

`RQ-007 — Diagramas Documentales`

¿En qué condiciones los diagramas representan de manera efectiva necesidades documentales de VSlices Docs Standard sin reemplazar los artifacts responsables de explicar, apoyar, componer, conectar u organizar conocimiento?

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* `RQ-001`
* `RN-0001`
* `RN-0002`
* el modelo candidato de Docs Standard
* el Diagrama de Camino de Continuidad
* el Diagrama de Ramificación de Preguntas
* la semántica inicial propuesta para nodos y líneas
* la decisión inicial de usar Mermaid
* la necesidad de representar continuidad sin convertir todo en texto o metadata

## Evidencia faltante

Todavía falta observar:

* si los diagramas ayudan a entender artifacts más rápido
* si reducen ambigüedad
* si la simbología se entiende sin explicación excesiva
* si Mermaid alcanza para las necesidades iniciales
* si los diagramas se mantienen editables
* si los diagramas se vuelven ilegibles al crecer
* si ayudan a decidir qué documentar y qué no
* si evitan o introducen ceremonia visual
* si las personas distinguen diagrama, artifact y fuente de verdad
* si Surreal Atlas mejora la representación sin reemplazar la documentación
* si Tooling puede generar diagramas útiles sin imponer estructura prematura

## Riesgos metodológicos

### Riesgo de convertir diagramas en fuente de verdad

Un diagrama debe mostrar conocimiento, no reemplazar el artifact que lo preserva.

### Riesgo de burocracia visual

Un diagrama puede agregar más complejidad que claridad si exige demasiada simbología, mantenimiento o interpretación.

### Riesgo de simbología demasiado compleja

Si la leyenda necesita demasiada explicación, el diagrama puede dejar de ser una ayuda.

### Riesgo de Mermaid como falsa estabilidad

Que un diagrama pueda escribirse en Mermaid no significa que el modelo visual esté validado.

### Riesgo de reemplazar explicación textual

Los diagramas pueden mostrar relaciones, pero la explicación principal debe vivir en artifacts adecuados.

### Riesgo de mapas ilegibles

Un diagrama demasiado grande puede perder su función orientadora.

### Riesgo de validar estética en vez de utilidad

Un diagrama puede verse bien y aun así no ayudar a preservar continuidad.

## Lo que esta nota no afirma

Esta nota no afirma que Docs Standard necesita diagramas para funcionar.

No afirma que los diagramas actuales sean suficientes.

No afirma que Mermaid sea la solución definitiva.

No afirma que la simbología actual sea estable.

No convierte diagramas en familia formal de artifacts.

No valida que los diagramas preserven continuidad.

No afirma que toda documentación deba tener representación visual.

Solo propone una línea exploratoria para estudiar cómo representar visualmente necesidades documentales de Docs Standard.

## Límite actual

Esta nota debe mantenerse como exploratoria.

Los diagramas deberían investigarse después de observar con mayor claridad qué necesitan representar los mecanismos principales de Docs Standard.

Su valor actual está en abrir una pregunta específica sin contaminar las RQs más estables sobre Documents, Support Notes, Nexus, Continuity Paths y Organizaciones Documentales.

La pregunta central que deja abierta es:

> ¿Qué debe representar visualmente Docs Standard, para quién, con qué simbología, bajo qué costo y sin reemplazar los artifacts responsables de preservar conocimiento?
