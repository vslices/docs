---
artifact:
  kind: continuity-path
  type: software-initiative
  scope: initiative
  target: <software-initiative-name>
  language: es

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references|referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes|superseded-by>
      target: <artifact-id>

continuity:
  question: ¿Qué intenta cubrir esta iniciativa y qué piezas participan?
  preserves: software-coverage-continuity
  connects:
    - artifact: <artifact-id>
      role: <business-scenario|business-driver|work-line|initiative-scope|client-product|consumable-service|capability|decision|software-project|viability|feedback|result|update|evolution>

tooling:
  schema:
    version: 0.1.0
  template:
    name: software-initiative.continuity-path
    version: 0.1.0
---

# Camino de continuidad "Iniciativa de software" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de cobertura funcional, alcance de intervención y materialización por software se busca preservar.
No explicar todavía la estructura interna de los proyectos de software originados; eso pertenece al Camino de continuidad de Proyecto de software.
-->

Este path busca preservar continuidad entre una parte del escenario de negocio y las herramientas de software que permiten abordarla.

En esta perspectiva, "herramientas" no se refiere solo a tooling técnico.

Se refiere a productos, servicios, capacidades, procesos soportados, decisiones, límites y proyectos de software que permiten intervenir una parte del trabajo mediante software.

Ayuda a entender qué intenta cubrir una iniciativa, qué piezas participan, qué queda dentro o fuera del alcance y qué decisiones explican esa cobertura.

También ayuda a separar la cobertura funcional de una iniciativa de su materialización técnica concreta.

## Punto de entrada

<!--
¿Por dónde empieza este camino?

Indicar la iniciativa, esfuerzo, mejora, modernización, migración, integración o parte del trabajo desde donde parte el recorrido.
-->

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Software Initiative.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Software Initiative</b><br/>[Iniciativa de software]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Scope Document</a><br/><a href='link'>Software Initiative Path</a></small>"]]

    A --> P1["¿Qué parte del escenario aborda?"]
    A --> P2["¿Qué líneas de trabajo incluye, excluye o posterga?"]
    A --> P3["¿Qué productos o servicios participan?"]
    A --> P4["¿Qué capacidades requiere?"]
    A -.-> P5["¿Qué decisiones explican su alcance?"]
    A -.-> P6["¿Qué proyectos de software originó o podría originar?"]
    A -.-> P7["¿Es viable abordar esta iniciativa ahora?"]
    A -.-> P8["¿Qué aprendizaje o cambio afecta su cobertura?"]

    P1 --> BS1[["<b>Business Scenario</b><br/>[Escenario de negocio]<br/><small><a href='link'>Business Scenario Path</a></small>"]]
    P1 --> BS2>"<b>Business Scenario</b><br/>[Escenario mencionado]"]
    P1 -.-> BD1[["<b>Business Driver</b><br/>[Motivación relacionada]<br/><small><a href='link'>Business Driver Path</a></small>"]]

    P2 --> WL1[["<b>Work Line</b><br/>[Línea incluida]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Scope Document</a></small>"]]
    P2 --> WL2>"<b>Work Line</b><br/>[Línea excluida o postergada]"]
    P2 --> SC1{{"<b>Initiative Scope</b><br/>[Cobertura de la iniciativa]<br/><small>Scope Document<br/>Decision Record</small>"}}

    P3 --> CP1[["<b>Client Product</b><br/>[Producto al cliente]<br/><small><a href='link'>Client Product Path</a></small>"]]
    P3 --> CS1[["<b>Consumable Service</b><br/>[Servicio consumible]<br/><small><a href='link'>Consumable Service Path</a></small>"]]
    P3 --> CS2>"<b>Consumable Service</b><br/>[Servicio identificado]"]
    P3 -.-> PX1{{"<b>Participation Gap</b><br/>[Participación no clara]<br/><small>Support Note kind: draft<br/>Support Note kind: validation</small>"}}

    P4 --> C1{{"<b>Capability</b><br/>[Capacidad requerida]<br/><small>Capability Nexus<br/>Scope Document<br/>Behavior Document<br/>Structure Document<br/>Consistency Document<br/>Viability Document</small>"}}
    P4 --> C2>"<b>Capability</b><br/>[Capacidad identificada]"]
    P4 -.-> C3{{"<b>Capability Risk</b><br/>[Riesgo de capacidad]<br/><small>Support Note kind: risk<br/>Viability Document</small>"}}

    P5 -.-> D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    P5 -.-> D2{{"<b>Scope Decision</b><br/>[Decisión pendiente]<br/><small>Decision Record<br/>Support Note kind: draft</small>"}}

    P6 -.-> SP1[["<b>Software Project</b><br/>[Proyecto originado]<br/><small><a href='link'>Software Project Path</a></small>"]]
    P6 -.-> SP2>"<b>Software Project</b><br/>[Proyecto candidato]"]
    P6 -.-> SP3{{"<b>Technical Materialization</b><br/>[Materialización técnica pendiente]<br/><small>Software Project Path<br/>Structure Document<br/>Decision Record</small>"}}

    P7 -.-> V1[["<b>Viability</b><br/>[Viabilidad evaluada]<br/><small><a href='link'>Viability Path</a><br/><a href='link'>Viability Document</a></small>"]]
    P7 -.-> V2{{"<b>Viability Gap</b><br/>[Viabilidad no clara]<br/><small>Viability Document<br/>Support Note kind: validation<br/>Support Note kind: risk</small>"}}

    P8 -.-> FB1[["<b>Feedback</b><br/>[Feedback documentado]<br/><small><a href='link'>Feedback Document</a></small>"]]
    P8 -.-> R1[["<b>Result</b><br/>[Resultado observado]<br/><small>Support Note kind: result</small>"]]
    P8 -.-> UP1{{"<b>Initiative Update</b><br/>[Actualización de cobertura]<br/><small>Update Document<br/>Decision Record<br/>Scope Document</small>"}}
    P8 -.-> EV1[["<b>Evolution</b><br/>[Evolución relacionada]<br/><small><a href='link'>Evolution Path</a></small>"]]
```

!!! note "¿Qué proyectos originó?"

```
Una iniciativa de software puede originar uno o varios proyectos de software.

Esta pregunta ayuda a separar la cobertura funcional de la iniciativa de la materialización técnica concreta donde los elementos viven, evolucionan y se mantienen.

Cuando la pregunta principal pasa a ser cómo vive un concepto dentro de un proyecto, conviene continuar el recorrido en el Camino de continuidad "Proyecto de software".
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto                            | Por qué revisarlo                                                                        |
| ----- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| 1     | Iniciativa de software                               | Permite identificar qué esfuerzo organizado estamos siguiendo                            |
| 2     | Escenario de negocio abordado                        | Permite entender qué parte del trabajo intenta intervenir                                |
| 3     | Líneas de trabajo incluidas, excluidas o postergadas | Permite entender la cobertura real de la iniciativa                                      |
| 4     | Productos o servicios participantes                  | Permite reconocer qué piezas de software entregan, sostienen o habilitan la intervención |
| 5     | Capacidades requeridas                               | Permite entender qué necesita construir, usar, estabilizar o preservar la iniciativa     |
| 6     | Decisiones de alcance                                | Permite entender por qué ciertas partes entran, quedan fuera o se postergan              |
| 7     | Proyectos de software originados                     | Permite conectar la iniciativa con su materialización técnica concreta                   |

## Cobertura y materialización

<!--
¿Cómo se distingue la cobertura de la iniciativa de su materialización técnica?

Usar esta sección para evitar confundir iniciativa de software con proyecto de software.
-->

| Concepto            | Cómo se interpreta                                                       | Cuándo usarlo                                                                          |
| ------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------------------------- |
| Software Initiative | Esfuerzo organizado para abordar una parte del trabajo mediante software | Cuando necesitamos entender cobertura, intención, alcance y piezas participantes       |
| Client Product      | Producto visible que participa en la iniciativa                          | Cuando la iniciativa entrega o modifica experiencia de uso                             |
| Consumable Service  | Servicio consumible que participa en la iniciativa                       | Cuando la iniciativa expone, coordina o consume capacidades entre sistemas o productos |
| Capability          | Capacidad requerida para que la iniciativa pueda sostenerse              | Cuando la iniciativa necesita construir, usar, estabilizar o preservar una capacidad   |
| Software Project    | Materialización técnica originada por la iniciativa                      | Cuando necesitamos entender dónde viven técnicamente los elementos dentro del proyecto |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender esta iniciativa sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con la iniciativa | Path o artifact sugerido |
| ----------------------- | -------------------------- | ------------------------ |
| <concepto>              | <relación>                 | <path o artifact>        |
