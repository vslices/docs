---
artifact:
  kind: continuity-path
  type: business-scenario
  scope: business-scenario
  target: <business-scenario-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: []

continuity:
  question: ¿Dónde ocurre el trabajo y qué elementos ayudan a entender este escenario?
  preserves: operational-continuity
  connects:
    - artifact: <artifact-id>
      role: <work-line|process|flow|behavior|domain-context|business-driver|software-initiative|client-product|consumable-service|impact>

tooling:
  schema:
    version: 0.1.0
  template:
    name: business-scenario.continuity-path
    version: 0.1.0
---

# Camino de continuidad "Escenario de negocio" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad operativa se busca preservar.
No explicar todavía todo el negocio ni toda la organización.
-->

Este path busca preservar continuidad alrededor del contexto operativo donde ocurre el trabajo.

Ayuda a entender dónde aparece el conocimiento antes de enfocarse en proyectos, productos, servicios, decisiones o implementaciones específicas.

Permite recorrer un escenario de negocio desde una mirada amplia hacia líneas de trabajo, procesos, flujos, actores, responsabilidades, reglas operativas, comportamientos relevantes y conceptos relacionados.

## Punto de entrada

<!--
¿Por dónde empieza este camino?

Indicar el escenario, situación operativa o concepto raíz desde donde parte el recorrido.
-->

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Business Scenario.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart TD
    CR[["<b>Business Scenario</b><br/>[Escenario de negocio]<br/><small>Context Document<br/>Navigation Document<br/>Support Note kind: draft</small>"]]

    P1["¿Qué líneas de trabajo existen dentro del escenario?"]
    P2["¿Qué conceptos complementan este escenario?"]

    CR --> P1
    CR -.-> P2

    WL1[["<b>Work Line</b><br/>[Línea de trabajo documentada]<br/><small>Context Document<br/>Structure Document<br/>Scope Document</small>"]]
    WL2>"<b>Work Line</b><br/>[Línea de trabajo identificada]"]

    P1 --> WL1 & WL2

    CO1[["<b>Domain Context</b><br/>[Contexto de dominio relacionado]<br/><small>Domain Context Path<br/>Domain Vocabulary<br/>Consistency Document<br/>Behavior Document</small>"]]
    CO2[["<b>Business Driver</b><br/>[Motivación relacionada]<br/><small>Business Driver Path<br/>Context Document<br/>Decision Record<br/>Viability Document</small>"]]

    P2 -.-> CO1 & CO2

    P3["¿Qué procesos explican cómo opera esta línea?"]
    P4["¿Qué conceptos complementan esta línea de trabajo?"]

    WL1 --> P3
    WL1 -.-> P4

    PR1[["<b>Process</b><br/>[Proceso documentado]<br/><small>Structure Document<br/>Behavior Document<br/>Context Document</small>"]]
    PR2{{"<b>Process</b><br/>[Proceso que requiere documentación]<br/><small>Structure Document<br/>Behavior Document<br/>Context Document</small>"}}

    P3 --> PR1 & PR2

    SI1[["<b>Software Initiative</b><br/>[Iniciativa relacionada]<br/><small>Software Initiative Path<br/>Scope Document<br/>Context Document<br/>Decision Record</small>"]]
    VI1{{"<b>Viability</b><br/>[Viabilidad identificada]<br/><small>Viability Path<br/>Viability Document<br/>Support Note kind: validation</small>"}}

    P4 -.-> SI1 & VI1

    P5["¿Qué flujos muestran cómo avanza este proceso?"]
    P6["¿Qué conceptos complementan este proceso?"]

    PR1 --> P5
    PR1 -.-> P6

    FL1>"<b>Flow</b><br/>[Flujo identificado]"]
    FL2{{"<b>Flow</b><br/>[Flujo que requiere documentación]<br/><small>Behavior Document<br/>Mockup Flow<br/>Support Note kind: testing-spec</small>"}}

    P5 --> FL1 & FL2

    CP1[["<b>Client Product</b><br/>[Producto relacionado]<br/><small>Client Product Path<br/>Behavior Document<br/>Mockup Flow<br/>Feedback Document<br/>Scope Document</small>"]]
    CS1[["<b>Consumable Service</b><br/>[Servicio relacionado]<br/><small>Consumable Service Path<br/>Structure Document<br/>Behavior Document<br/>Consistency Document<br/>Domain Vocabulary</small>"]]
    IMP1{{"<b>Impact</b><br/>[Impacto potencial]<br/><small>Impact Path<br/>Update Document<br/>Support Note kind: validation</small>"}}

    P6 -.-> CP1 & CS1 & IMP1

    P7["¿Qué comportamientos específicos aparecen en este flujo?"]

    FL2 --> P7

    BH1[["<b>Behavior</b><br/>[Comportamiento documentado]<br/><small>Behavior Document<br/>Consistency Document<br/>Support Note kind: testing-spec<br/>Support Note kind: validation</small>"]]
    BH2>"<b>Behavior</b><br/>[Comportamiento identificado]"]

    P7 --> BH1 & BH2
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto   | Por qué revisarlo                                                                                    |
| ----- | --------------------------- | ---------------------------------------------------------------------------------------------------- |
| 1     | Escenario de negocio        | Permite ubicar dónde ocurre el trabajo                                                               |
| 2     | Líneas de trabajo           | Permiten organizar, entender y segmentar los servicios de valor del escenario                        |
| 3     | Procesos                    | Permiten entender cómo se organiza el trabajo de una línea para producir resultados                  |
| 4     | Flujos                      | Permiten observar secuencias concretas de pasos, decisiones, transferencias o participantes          |
| 5     | Comportamientos específicos | Permiten reconocer qué debe ocurrir dentro de una parte concreta del escenario                       |
| 6     | Conceptos complementarios   | Permiten identificar otros paths, documentos o artifacts que enriquecen la comprensión del escenario |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
