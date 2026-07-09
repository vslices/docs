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
    CR[["<b>Business Scenario</b><br/>[Escenario de negocio]<br/><small><a href='link'>Context Document</a></small>"]]

    P1["¿Qué líneas de trabajo existen dentro del escenario?"]
    P2["¿Qué conceptos complementan este escenario?"]

    CR --> P1
    CR -.-> P2

    WL1[["<b>Work Line</b><br/>[Línea de trabajo documentada]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Structure Document</a></small>"]]
    WL2>"<b>Work Line</b><br/>[Línea de trabajo identificada]"]

    P1 --> WL1 & WL2

    CO1[["<b>Domain Context</b><br/>[Contexto de dominio relacionado]<br/><small><a href='link'>Domain Context Path</a></small>"]]
    CO2[["<b>Business Driver</b><br/>[Motivación relacionada]<br/><small><a href='link'>Business Driver Path</a></small>"]]

    P2 -.-> CO1 & CO2

    P3["¿Qué procesos explican cómo opera esta línea?"]
    P4["¿Qué conceptos complementan esta línea de trabajo?"]

    WL1 --> P3
    WL1 -.-> P4

    PR1[["<b>Process</b><br/>[Proceso documentado]<br/><small><a href='link'>Structure Document</a></small>"]]
    PR2{{"<b>Process</b><br/>[Proceso que requiere documentación]<br/><small>Structure Document<br/>Behavior Document</small>"}}

    P3 --> PR1 & PR2

    SI1[["<b>Software Initiative</b><br/>[Iniciativa relacionada]<br/><small><a href='link'>Software Initiative Path</a></small>"]]
    VI1{{"<b>Viability</b><br/>[Viabilidad identificada]<br/><small>Viability Path</small>"}}

    P4 -.-> SI1 & VI1

    P5["¿Qué flujos muestran cómo avanza este proceso?"]
    P6["¿Qué conceptos complementan este proceso?"]

    PR1 --> P5
    PR1 -.-> P6

    FL1>"<b>Flow</b><br/>[Flujo identificado]"]
    FL2{{"<b>Flow</b><br/>[Flujo que requiere documentación]<br/><small>Behavior Document</small>"}}

    P5 --> FL1 & FL2

    CP1[["<b>Client Product</b><br/>[Producto relacionado]<br/><small><a href='link'>Client Product Path</a></small>"]]
    CS1[["<b>Consumable Service</b><br/>[Servicio relacionado]<br/><small><a href='link'>Consumable Service Path</a></small>"]]

    P6 -.-> CP1 & CS1

    P7["¿Qué comportamientos específicos aparecen en este flujo?"]

    FL2 --> P7

    BH1[["<b>Behavior</b><br/>[Comportamiento documentado]<br/><small><a href='link'>Behavior Document</a></small>"]]
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
