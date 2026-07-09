# Camino de continuidad "Viabilidad" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de viabilidad se busca preservar.
No limitar la viabilidad a costo económico; el kind indica la dimensión evaluada.
-->

Este path busca preservar continuidad entre `<tema>`, las condiciones que hacen posible abordarlo y las restricciones que podrían volverlo inviable.

Ayuda a entender si un concepto, iniciativa, cambio, feature, capability, servicio, producto, experimento, decisión o artifact puede sostenerse bajo las condiciones actuales.

En esta perspectiva, viabilidad no significa únicamente viabilidad económica.

Puede referirse a viabilidad económica, técnica, operacional, temporal, organizacional, de adopción u otra dimensión relevante según el kind evaluado.

Este path ayuda a evitar que una idea avance solo porque parece valiosa, deseable o técnicamente interesante, sin revisar si existen las condiciones necesarias para realizarla, sostenerla, validarla o evolucionarla.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el elemento cuya viabilidad se quiere entender.
-->

El recorrido debería comenzar desde el elemento cuya viabilidad se quiere evaluar.

Ese punto de entrada puede ser:

* una iniciativa
* un cambio de alcance
* una feature
* una capability
* un producto al cliente
* un servicio consumible
* una decisión
* un experimento
* un artifact
* una automatización
* una integración
* una migración
* una mejora operativa
* una alternativa de solución
* una inversión propuesta
* una evolución de alcance

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Viability.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Viability Subject</b><br/>[Objeto evaluado]<br/><small><a href='link'>Viability Document</a><br/><a href='link'>Viability Path</a></small>"]]

    P1["¿Qué estamos evaluando?"]
    P2["¿Qué kind de viabilidad aplica?"]
    P3["¿Qué condiciones deben cumplirse?"]
    P4["¿Qué restricciones limitan la viabilidad?"]
    P5["¿Qué tan viable parece ahora?"]
    P6["¿Qué podría volverlo inviable?"]
    P7["¿Qué alternativa lo haría más viable?"]
    P8["¿Cuándo debe reevaluarse?"]

    O1[["<b>Evaluated Object</b><br/>[Objeto evaluado]<br/><small><a href='link'>Viability Document</a></small>"]]
    O2>"<b>Candidate Object</b><br/>[Objeto identificado]"]

    K1[["<b>Viability Kind</b><br/>[Kind definido]<br/><small><a href='link'>Viability Document</a></small>"]]
    K2{{"<b>Viability Kind</b><br/>[Kind no claro]<br/><small>Viability Document</small>"}}

    C1[["<b>Necessary Condition</b><br/>[Condición documentada]<br/><small><a href='link'>Viability Document</a></small>"]]
    C2{{"<b>Necessary Condition</b><br/>[Condición que requiere definición]<br/><small>Viability Document</small>"}}

    R1[["<b>Known Restriction</b><br/>[Restricción documentada]<br/><small><a href='link'>Viability Document</a></small>"]]
    R2>"<b>Known Restriction</b><br/>[Restricción identificada]"]

    E1[["<b>Initial Evaluation</b><br/>[Evaluación inicial]<br/><small><a href='link'>Viability Document</a></small>"]]
    E2{{"<b>Evaluation Gap</b><br/>[Evaluación insuficiente]<br/><small>Viability Document<br/>Support Note kind: validation</small>"}}

    IV1{{"<b>Inviability Risk</b><br/>[Riesgo de inviabilidad]<br/><small>Viability Document<br/>Risk Note</small>"}}

    ALT1>"<b>Viability Alternative</b><br/>[Alternativa identificada]"]
    ALT2{{"<b>Smaller Alternative</b><br/>[Alternativa más pequeña]<br/><small>Scope Document<br/>Decision Record</small>"}}

    RV1{{"<b>Review Condition</b><br/>[Condición de revisión]<br/><small>Viability Document<br/>Update Document</small>"}}

    A --> P1
    P1 --> O1 & O2

    A --> P2
    P2 --> K1 & K2

    A --> P3
    P3 --> C1 & C2

    A --> P4
    P4 --> R1 & R2

    A --> P5
    P5 --> E1 & E2

    A -.-> P6
    P6 -.-> IV1

    A -.-> P7
    P7 -.-> ALT1 & ALT2

    A -.-> P8
    P8 -.-> RV1
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto  | Por qué revisarlo                                                      |
| ----- | -------------------------- | ---------------------------------------------------------------------- |
| 1     | Objeto evaluado            | Permite identificar qué elemento se está evaluando                     |
| 2     | Kind de viabilidad         | Permite saber qué dimensión de viabilidad se está observando           |
| 3     | Criterio de viabilidad     | Permite entender qué significa que el elemento sea viable en ese kind  |
| 4     | Condiciones necesarias     | Permite reconocer qué debe cumplirse para sostener la viabilidad       |
| 5     | Restricciones conocidas    | Permite entender qué limita o condiciona la viabilidad                 |
| 6     | Evaluación inicial         | Permite registrar qué tan viable parece con la información disponible  |
| 7     | Riesgos de inviabilidad    | Permite identificar qué podría volverlo inviable                       |
| 8     | Alternativas de viabilidad | Permite encontrar una versión más pequeña, más simple o más sostenible |
| 9     | Condiciones de revisión    | Permite saber cuándo reevaluar la viabilidad                           |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
