---
type: research-question
state: candidate
code: RQ-002

related_questions:
* RQ-001

related_notes:
* RN-0001
* RN-0002

related_synthesis:
* SYN-0001

related_studies: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
---

# RQ-002 — Caminos de Continuidad

## Pregunta

¿En qué condiciones los Caminos de Continuidad ayudan a preservar continuidad de conocimiento entre perspectivas, artifacts, decisiones y conceptos sin convertirse en checklist documental obligatorio?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0002-vslices-docs-standard.md).

Docs Standard propone los Caminos de Continuidad como artifacts capaces de conectar y orientar continuidad alrededor de un target.

La idea aparece como respuesta candidata al problema fundacional de VSlices Research: la continuidad de conocimiento puede romperse, dispersarse, concentrarse o escaparse cuando las conexiones entre intención, dominio, documentación, decisiones, arquitectura, implementación y evolución dejan de ser visibles.

## Problema observado

En proyectos de software, un elemento puede aparecer en múltiples superficies:

* escenario de negocio
* contexto de dominio
* decisión
* iniciativa de software
* producto al cliente
* servicio consumible
* estructura técnica
* cambio de alcance
* validación
* feedback
* handoff de conocimiento

Aunque existan documentos o implementación, puede perderse la relación entre esos elementos.

Podemos saber qué se implementó, pero no necesariamente:

* por qué importaba
* dónde apareció
* qué significado tenía
* qué decisión lo transformó
* qué alcance cambió
* dónde se materializó
* qué impacto produjo
* quién lo sostiene

Los Caminos de Continuidad intentan hacer visible ese recorrido.

## Hipótesis inicial

Los Caminos de Continuidad podrían ayudar a preservar continuidad de conocimiento cuando permiten seguir un target a través de perspectivas relevantes sin obligar a documentar todo el mapa.

Su valor estaría en orientar la exploración, identificar relaciones significativas y mostrar necesidades documentales candidatas.

Su riesgo estaría en transformarse en checklist, grafo obligatorio o lista de documentos exigidos.

## Qué busca observar esta pregunta

Esta pregunta busca observar si los Caminos de Continuidad ayudan a:

* identificar conexiones relevantes entre artifacts
* descubrir conocimiento faltante
* evitar pérdida de intención
* separar conceptos documentados de conceptos solo identificados
* decidir cuándo detener la exploración
* evitar documentación prematura
* preservar continuidad entre dominio, producto, servicio, proyecto y evolución

También busca observar cuándo dejan de ayudar.

## Mecanismo candidato

El mecanismo candidato es el **Continuity Path**.

Un Continuity Path:

* conecta y orienta continuidad alrededor de un target
* declara una pregunta de continuidad
* declara qué continuidad intenta preservar
* conecta artifacts o paths relevantes
* diferencia rutas principales y auxiliares
* puede usar diagramas para mostrar el recorrido
* no reemplaza los artifacts conectados
* no obliga a crear todos los artifacts mencionados

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [SYN-0001](../synthesis/syn-0001-escenarios-iniciales-ruptura-escape-continuidad-conocimiento.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* el modelo candidato de VSlices Docs Standard
* los Continuity Paths candidatos definidos para Docs Standard

Continuity Paths candidatos iniciales:

* Business Scenario
* Business Driver
* Domain Context
* Viability
* Evolution
* Software Initiative
* Client Product
* Consumable Service
* Software Project
* Ownership
* Impact
* Traceability
* Knowledge Handoff

## Evidencia faltante

Todavía falta observar:

* si un path ayuda realmente a encontrar conocimiento relevante
* si reduce incertidumbre documental
* si evita fragmentación entre artifacts
* si las personas entienden cuándo usarlo
* si las personas entienden cuándo detenerse
* si el path se interpreta como mapa y no como checklist
* si los nodos con necesidad documental se tratan como candidatos y no como obligación inmediata
* si el path sigue siendo útil sin tooling
* si el path mejora con tooling o solo agrega complejidad

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde exista riesgo de pérdida, dispersión, concentración o escape de conocimiento.

Posibles escenarios:

* una transición de conocimiento entre personas o equipos
* un concepto de dominio que aparece en producto, servicio e implementación
* una iniciativa de software que conecta escenario de negocio, comportamiento, servicio y proyecto técnico
* una evolución de alcance que requiere seguir intención, decisión, cambio e impacto
* una documentación existente donde las conexiones no son visibles

## Riesgos metodológicos

### Riesgo de validar el path como checklist

Un caso exitoso no debe llevar a concluir que todos los proyectos deben recorrer todos los paths.

### Riesgo de confundir visibilidad con continuidad

Un diagrama puede mostrar relaciones sin preservar realmente intención, criterio o aprendizaje.

### Riesgo de documentar cada nodo

Identificar un concepto no implica documentarlo inmediatamente.

### Riesgo de sobreinterpretar tres casos

Los casos iniciales pueden sugerir utilidad local, pero no validan universalmente la familia de Continuity Paths.

## Relación con Docs Standard

Esta pregunta puede afectar:

* definición de Continuity Paths
* categorías Core, Supporting y Contextual
* diagramas de Camino de Continuidad
* reglas para elegir paths
* reglas para detener recorridos
* criterios anti-checklist
* futura integración con Tooling
* futura integración con Surreal Atlas

## Límite actual

Esta pregunta no asume que los Caminos de Continuidad funcionan.

Solo propone investigarlos como mecanismo candidato para preservar continuidad de conocimiento.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.
