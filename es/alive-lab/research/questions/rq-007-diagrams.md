---
type: research-question
state: candidate
code: RQ-007

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
* RN-0003

related_synthesis:
* SYN-0001

related_studies: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Tooling
* Surreal Atlas
---

# RQ-007 — Diagramas Documentales

## Pregunta

¿En qué condiciones los diagramas representan de manera efectiva necesidades documentales de VSlices Docs Standard sin reemplazar los artifacts responsables de explicar, apoyar, componer, conectar u organizar conocimiento?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0003 — Diagramas como representación visual exploratoria en VSlices Docs Standard](../notes/RN-0003-vslices-docs-standard-diagrams.md).

Docs Standard ya propone mecanismos documentales candidatos con responsabilidades relativamente claras:

* Document artifacts explican
* Support Notes apoyan, registran o referencian
* Nexus artifacts componen
* Continuity Paths conectan y orientan continuidad
* Organizaciones documentales ordenan
* Proyecciones navegables muestran organizaciones
* Navigation Documents explican recorridos

Los diagramas aparecen como una línea más exploratoria.

Su responsabilidad candidata no es explicar, apoyar, componer, conectar u organizar directamente.

Su responsabilidad candidata es representar visualmente relaciones, preguntas, recorridos, estructuras, estados o necesidades documentales.

## Problema observado

Algunos aspectos de Docs Standard pueden volverse difíciles de entender solo mediante texto lineal.

Por ejemplo:

* cómo una pregunta documental principal se ramifica en preguntas derivadas
* qué segmentos posibles puede activar un Document artifact
* qué conceptos aparecen en un Continuity Path
* qué nodos ya están documentados
* qué nodos solo fueron identificados
* qué nodos podrían requerir documentación
* qué rutas son principales o auxiliares
* qué artifacts participan en un Nexus
* cómo una organización documental puede proyectarse sin duplicar contenido

Los diagramas podrían ayudar a hacer visibles estas relaciones.

Sin embargo, también pueden introducir una nueva forma de complejidad.

Un diagrama puede verse claro, elegante o completo, pero aun así:

* reemplazar indebidamente la explicación textual
* duplicar contenido canónico
* volverse una segunda fuente de verdad
* exigir simbología difícil de recordar
* crecer hasta ser ilegible
* convertir cada nodo en obligación documental
* ocultar incertidumbre bajo una representación demasiado estable

## Hipótesis inicial

Los diagramas podrían ayudar a preservar continuidad documental cuando representan visualmente relaciones, recorridos, preguntas o necesidades documentales que serían difíciles de reconocer solo mediante texto.

Su valor estaría en hacer visible orientación, estado documental, composición o ramificación sin reemplazar el artifact que preserva el conocimiento principal.

Su riesgo estaría en convertirse en burocracia visual, fuente de verdad paralela o representación demasiado compleja para mantenerse.

## Qué busca observar esta pregunta

Esta pregunta busca observar si los diagramas ayudan a:

* representar necesidades documentales
* hacer visibles relaciones entre artifacts
* orientar recorridos de continuidad
* distinguir conceptos documentados de conceptos identificados
* mostrar posibles necesidades documentales sin convertirlas en obligación
* organizar preguntas derivadas desde una pregunta principal
* separar rutas principales de rutas auxiliares
* apoyar decisiones sobre qué documentar ahora y qué no
* reducir ambigüedad
* mejorar navegación o comprensión sin duplicar contenido

También busca observar cuándo los diagramas dejan de ayudar.

## Mecanismo candidato

El mecanismo candidato es el **diagrama documental**.

Por ahora no se propone como familia formal estable de Docs Standard.

Se entiende como una representación asociada y exploratoria.

Diagramas candidatos actuales:

| Diagrama                              | Necesidad que representa                                                                                                 |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Diagrama de Camino de Continuidad     | Recorridos de continuidad, preguntas orientadoras, conceptos conectados, artifacts existentes y necesidades documentales |
| Diagrama de Ramificación de Preguntas | Ramificación de una pregunta documental principal en preguntas derivadas, segmentos posibles o ramas de organización     |

Ambos diagramas se expresan inicialmente mediante Mermaid.

Mermaid se entiende como tecnología inicial de representación, no como la teoría visual definitiva de VSlices.

## Diagrama candidato 1: Diagrama de Camino de Continuidad

El Diagrama de Camino de Continuidad representa visualmente un Continuity Path.

Puede mostrar:

* target o concepto seguido
* preguntas orientadoras
* conceptos relacionados
* artifacts existentes
* artifacts candidatos
* conceptos identificados sin necesidad documental actual
* conceptos con posible necesidad documental
* rutas principales
* rutas auxiliares
* cambios de perspectiva

Su objetivo no es explicar todo el conocimiento conectado.

Su objetivo es mostrar un recorrido suficiente para preservar orientación.

## Diagrama candidato 2: Diagrama de Ramificación de Preguntas

El Diagrama de Ramificación de Preguntas representa cómo una pregunta documental principal se abre en preguntas derivadas.

Puede mostrar:

* pregunta principal
* preguntas derivadas
* segmentos documentales candidatos
* ramas principales
* ramas auxiliares
* costo o esfuerzo de incorporar una rama
* preguntas que pueden quedar pendientes
* preguntas que no deben convertirse todavía en contenido visible

Su objetivo no es imponer el formato final de un Document artifact.

Su objetivo es ayudar a pensar cómo organizar el conocimiento que ese artifact podría preservar.

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* [RN-0003](../notes/RN-0003-vslices-docs-standard-diagrams.md)
* el modelo candidato de VSlices Docs Standard
* el Diagrama de Camino de Continuidad
* el Diagrama de Ramificación de Preguntas
* la semántica visual inicial de nodos y líneas
* la decisión inicial de usar Mermaid
* la necesidad de representar continuidad sin convertir todo en texto, metadata o artifacts adicionales

## Evidencia faltante

Todavía falta observar:

* si los diagramas ayudan a comprender más rápido
* si reducen ambigüedad
* si la simbología se entiende sin explicación excesiva
* si Mermaid es suficiente para los casos iniciales
* si los diagramas se mantienen editables
* si los diagramas se vuelven ilegibles al crecer
* si ayudan a decidir qué documentar y qué no
* si evitan o introducen ceremonia visual
* si las personas distinguen diagrama, artifact y fuente de verdad
* si los diagramas funcionan sin tooling
* si Tooling puede generar diagramas útiles sin imponer estructura prematura
* si Surreal Atlas mejora la navegación visual sin reemplazar los artifacts

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde una representación visual pueda reducir incertidumbre documental.

Posibles escenarios:

* un Continuity Path de Domus Orbis que necesita mostrar conceptos documentados, identificados y pendientes
* un Document artifact cuyo mapa de preguntas derivadas necesita organizarse antes de escribir contenido
* un Capability Nexus que requiere mostrar artifacts compuestos
* una organización documental que necesita una proyección visual tipo TreeView
* un caso de Surreal Atlas donde relaciones entre documents puedan visualizarse sin duplicar contenido
* un cambio de alcance donde Evolution o Impact requieran mostrar recorrido visual

## Criterios iniciales de observación

Un diagrama podría considerarse útil si:

* reduce tiempo para entender el recorrido
* permite detectar relaciones relevantes
* ayuda a decidir qué artifact revisar
* ayuda a decidir qué no documentar todavía
* hace visible una necesidad documental candidata
* no reemplaza el artifact principal
* no duplica contenido canónico
* puede mantenerse con esfuerzo razonable
* se entiende con una leyenda pequeña
* no requiere tooling avanzado para tener valor mínimo

Un diagrama podría considerarse problemático si:

* requiere demasiada explicación para entenderse
* genera más preguntas que claridad
* reemplaza contenido que debería vivir en un artifact
* copia contenido canónico
* se vuelve una segunda fuente de verdad
* convierte cada nodo en obligación documental
* crece hasta ser ilegible
* depende de simbología difícil de recordar
* solo aporta estética, pero no continuidad

## Riesgos metodológicos

### Riesgo de validar estética en vez de utilidad

Un diagrama puede verse bien y aun así no preservar continuidad.

La investigación debe observar utilidad, no belleza visual.

### Riesgo de convertir diagramas en fuente de verdad

El diagrama debe representar conocimiento.

No debe reemplazar el artifact que preserva explicación, composición, continuidad u organización.

### Riesgo de burocracia visual

Si crear o mantener el diagrama cuesta más que el valor que entrega, puede introducir ceremonia innecesaria.

### Riesgo de simbología excesiva

Una leyenda demasiado grande puede hacer que el diagrama dependa de demasiadas convenciones.

### Riesgo de Mermaid como falsa estabilidad

Que un diagrama pueda escribirse en Mermaid no significa que su modelo visual esté validado.

### Riesgo de reemplazar texto necesario

Algunas explicaciones requieren narrativa, límites, evidencia o contexto.

Un diagrama puede mostrar relaciones, pero no siempre explicar intención.

### Riesgo de introducir Tooling prematuro

Tooling puede ayudar a generar o validar diagramas, pero no debe automatizar una representación que todavía no demostró utilidad.

## Relación con Docs Standard

Esta pregunta puede afectar:

* definición de representaciones asociadas
* uso de diagramas dentro de Document artifacts
* uso de diagramas dentro de Continuity Paths
* uso de diagramas para Nexus
* uso de diagramas para organizaciones documentales
* semántica visual de nodos y líneas
* leyendas y simbología
* criterios de cuándo usar o no usar diagramas
* futuras capacidades de VSlices Tooling
* futuras visualizaciones en Surreal Atlas

## Relación con RQ-002

[RQ-002](../questions/rq-002-continuity-paths.md) investiga los Caminos de Continuidad.

`RQ-007` puede observar cómo los diagramas representan esos caminos.

La diferencia es importante:

* el Continuity Path conecta y orienta continuidad
* el diagrama representa visualmente ese recorrido

El diagrama no debe confundirse con el path completo.

## Relación con RQ-003

[RQ-003](../questions/rq-003-document-nexus.md) investiga los Nexos Documentales.

`RQ-007` puede observar cómo los diagramas representan composición entre artifacts.

La diferencia es importante:

* el Nexus declara composición
* el diagrama muestra composición

Si la composición solo existe en el diagrama, puede perder trazabilidad estructurada.

## Relación con RQ-004

[RQ-004](../questions/rq-004-documents.md) investiga los Document artifacts.

`RQ-007` puede observar cómo el Diagrama de Ramificación de Preguntas ayuda a organizar preguntas derivadas sin imponer una plantilla rígida.

La diferencia es importante:

* el Document artifact explica
* el diagrama ayuda a representar cómo se organiza la pregunta

## Relación con RQ-005

[RQ-005](../questions/rq-005-documental-organization.md) investiga Organizaciones Documentales.

`RQ-007` puede observar cómo los diagramas representan proyecciones navegables, TreeViews o mapas de artifacts.

La diferencia es importante:

* la organización define criterio de orden
* la proyección muestra ese orden
* el diagrama puede ser una forma de proyección

## Relación con RQ-006

[RQ-006](../questions/rq-006-support-notes.md) investiga Support Notes.

`RQ-007` puede observar cómo los diagramas muestran notas de soporte, riesgos, validaciones o resultados sin convertirlos en conocimiento estable prematuramente.

La diferencia es importante:

* la Support Note preserva el detalle auxiliar
* el diagrama muestra su existencia, rol o relación

## Límite actual

Esta pregunta es más exploratoria que las RQs anteriores de Docs Standard.

No asume que los diagramas son necesarios.

No asume que Mermaid será suficiente.

No asume que la simbología actual será estable.

No asume que los diagramas deben convertirse en familia formal de artifacts.

Solo propone investigarlos como representaciones visuales candidatas para necesidades documentales de VSlices Docs Standard.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.
