# Camino de continuidad "Knowledge Handoff" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos este handoff?

Explicar qué continuidad se busca preservar cuando una persona, rol o equipo deja de estar disponible.
-->

Este path busca preservar continuidad cuando una persona, rol o equipo posee conocimiento relevante que debe quedar disponible para otros bajo restricciones reales de tiempo, capacidad o prioridad.

Ayuda a responder:

> ¿Qué conocimiento debe quedar disponible para que el equipo pueda continuar sin depender de una persona específica?

Este path no intenta documentar todo lo que alguien sabe.

Intenta identificar qué conocimiento, si se pierde, afecta continuidad operativa, técnica, de producto, de dominio o de decisión.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar desde qué situación concreta nace el handoff.
-->

El recorrido debería comenzar desde la situación concreta que genera el traspaso.

Ejemplos:

* salida de una persona del equipo
* cambio de célula
* reemplazo de responsable técnico
* cierre de participación en un proyecto
* traspaso entre equipos
* rotación de ownership
* pérdida de disponibilidad de una persona clave
* transición operacional
* entrega de conocimiento antes de una fecha límite
* preparación de soporte para continuidad futura

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Knowledge Handoff.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid id="kh-path"
flowchart LR
    A[["<b>Knowledge Handoff</b><br/>[Traspaso de conocimiento]<br/><small><a href='link'>Knowledge Handoff Path</a></small>"]]

    P1["¿Qué conocimiento debe transferirse?"]
    P2["¿Quién necesita recibirlo?"]
    P3["¿Qué riesgo aparece si no queda disponible?"]
    P4["¿Qué debe priorizarse por tiempo limitado?"]
    P5["¿Qué decisiones o criterios deben preservarse?"]
    P6["¿Qué partes técnicas deben poder navegarse?"]
    P7["¿Qué comportamientos deben entenderse?"]
    P8["¿Qué queda pendiente, incompleto o fuera del traspaso?"]

    K1[["<b>Knowledge Area</b><br/>[Área de conocimiento documentada]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Navigation Document</a></small>"]]
    K2{{"<b>Tacit Knowledge</b><br/>[Conocimiento tácito relevante]<br/><small>Support Note<br/>Context Document</small>"}}

    O1[["<b>Receiver / Owner</b><br/>[Responsable receptor]<br/><small><a href='link'>Ownership Path</a></small>"]]
    O2>"<b>Receiver</b><br/>[Persona, rol o equipo identificado]"]

    I1{{"<b>Continuity Risk</b><br/>[Riesgo de pérdida de continuidad]<br/><small>Impact Path<br/>Support Note</small>"}}
    I2>"<b>Operational Impact</b><br/>[Impacto operativo identificado]"]

    V1[["<b>Viability</b><br/>[Priorización viable]<br/><small><a href='link'>Viability Path</a><br/><a href='link'>Viability Document kind: temporal</a></small>"]]
    S1{{"<b>Handoff Scope</b><br/>[Alcance del traspaso]<br/><small>Scope Document</small>"}}

    D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    D2{{"<b>Decision Criteria</b><br/>[Criterio no documentado]<br/><small>Decision Record<br/>Support Note</small>"}}

    T1[["<b>Software Project Area</b><br/>[Zona técnica documentada]<br/><small><a href='link'>Software Project Path</a><br/><a href='link'>Structure Document</a></small>"]]
    T2{{"<b>Technical Entry Point</b><br/>[Punto técnico crítico]<br/><small>Structure Document<br/>Navigation Document</small>"}}

    B1[["<b>Behavior</b><br/>[Comportamiento documentado]<br/><small><a href='link'>Behavior Document</a></small>"]]
    B2{{"<b>Expected Behavior</b><br/>[Comportamiento relevante]<br/><small>Behavior Document<br/>Support Note kind: testing-spec</small>"}}

    PND{{"<b>Pending / Incomplete</b><br/>[Pendiente o incompleto]<br/><small>Support Note<br/>Update Document</small>"}}
    EXC>"<b>Out of Handoff Scope</b><br/>[Fuera del traspaso actual]"]

    A --> P1
    P1 --> K1 & K2

    A --> P2
    P2 --> O1 & O2

    A --> P3
    P3 --> I1 & I2

    A --> P4
    P4 --> V1 & S1

    A -.-> P5
    P5 -.-> D1 & D2

    A -.-> P6
    P6 -.-> T1 & T2

    A -.-> P7
    P7 -.-> B1 & B2

    A -.-> P8
    P8 -.-> PND & EXC
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para organizar el handoff sin intentar documentarlo todo.
-->

| Orden | Nodo, artifact o concepto  | Por qué revisarlo                                                              |
| ----- | -------------------------- | ------------------------------------------------------------------------------ |
| 1     | Situación de handoff       | Permite entender por qué el traspaso existe y qué restricción lo condiciona    |
| 2     | Áreas de conocimiento      | Permite identificar qué conocimiento relevante posee la persona, rol o equipo  |
| 3     | Receptores u owners        | Permite saber quién necesita recibir, validar o mantener el conocimiento       |
| 4     | Riesgos de continuidad     | Permite priorizar lo que puede romper operación, soporte, decisión o evolución |
| 5     | Viabilidad temporal        | Permite decidir qué cabe en el tiempo disponible                               |
| 6     | Alcance del traspaso       | Permite separar lo que entra, queda fuera o queda pendiente                    |
| 7     | Decisiones y criterios     | Permite preservar por qué se trabaja de cierta forma                           |
| 8     | Puntos técnicos críticos   | Permite navegar zonas del proyecto que otros necesitarán tocar                 |
| 9     | Comportamientos relevantes | Permite entender qué debe ocurrir y cómo reconocer fallos                      |
| 10    | Pendientes e incompletos   | Permite dejar claro qué no alcanzó a transferirse                              |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
