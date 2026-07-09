# Camino de continuidad "Proyecto de software" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad técnica y arquitectónica se busca preservar.
No explicar todavía toda la implementación ni convertir este path en documentación técnica detallada.
-->

Este path busca preservar continuidad entre `<tema>` y su materialización dentro del proyecto de software.

Ayuda a entender cómo un concepto, comportamiento, decisión, capacidad o necesidad vive dentro de la estructura técnica, implementación y evolución del sistema.

También ayuda a evitar que el código, la arquitectura o las decisiones técnicas se alejen del lenguaje, intención, reglas y decisiones que les dieron origen.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el elemento técnico, comportamiento, decisión, estructura o concepto materializado desde donde parte el recorrido.
-->

El recorrido debería comenzar desde el elemento del proyecto de software que se quiere entender o seguir.

Ese punto de entrada puede ser:

* una feature implementada
* un módulo
* un componente
* una decisión técnica
* una integración
* un servicio interno
* un adapter
* una dependencia
* una estructura del proyecto
* un comportamiento implementado
* una regla materializada en código
* una capacidad técnica
* un cambio técnico observado

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Software Project.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    CR[["<b>Software Project Element</b><br/>[Elemento del proyecto]<br/><small><a href='link'>Structure Document</a><br/><a href='link'>Software Project Path</a></small>"]]

    P1["¿Qué intención o concepto materializa?"]
    P2["¿Dónde vive dentro del proyecto?"]
    P3["¿Qué estructura técnica lo organiza?"]
    P4["¿Qué comportamiento implementa o habilita?"]
    P5["¿Qué decisiones técnicas lo explican?"]
    P6["¿Qué dependencias, capacidades o adapters necesita?"]
    P7["¿Qué impacto tiene su evolución?"]

    INT1[["<b>Source Concept</b><br/>[Concepto de origen]<br/><small><a href='link'>Domain Context Path</a><br/><a href='link'>Business Driver Path</a><br/><a href='link'>Software Initiative Path</a></small>"]]
    INT2{{"<b>Missing Intent</b><br/>[Intención no documentada]<br/><small>Context Document<br/>Decision Record</small>"}}

    LOC1[["<b>Project Location</b><br/>[Ubicación documentada]<br/><small><a href='link'>Structure Document</a></small>"]]
    LOC2>"<b>Project Location</b><br/>[Ubicación identificada]"]

    STR1[["<b>Technical Structure</b><br/>[Estructura documentada]<br/><small><a href='link'>Structure Document</a></small>"]]
    STR2{{"<b>Technical Boundary</b><br/>[Límite técnico que requiere documentación]<br/><small>Structure Document<br/>Decision Record</small>"}}

    BH1[["<b>Implemented Behavior</b><br/>[Comportamiento implementado]<br/><small><a href='link'>Behavior Document</a></small>"]]
    BH2{{"<b>Behavior Gap</b><br/>[Comportamiento sin documentación clara]<br/><small>Behavior Document<br/>Support Note kind: testing-spec</small>"}}

    DEC1[["<b>Technical Decision</b><br/>[Decisión documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    DEC2{{"<b>Technical Decision</b><br/>[Decisión pendiente]<br/><small>Decision Record</small>"}}

    DEP1>"<b>Dependency</b><br/>[Dependencia identificada]"]
    CAP1{{"<b>Technical Capability</b><br/>[Capacidad técnica que requiere documentación]<br/><small>Structure Document<br/>Decision Record</small>"}}

    IMP1{{"<b>Evolution Impact</b><br/>[Impacto de evolución]<br/><small>Impact Path<br/>Update Document</small>"}}

    CR --> P1
    P1 --> INT1 & INT2

    CR --> P2
    P2 --> LOC1 & LOC2

    CR --> P3
    P3 --> STR1 & STR2

    CR --> P4
    P4 --> BH1 & BH2

    CR -.-> P5
    P5 -.-> DEC1 & DEC2

    CR -.-> P6
    P6 -.-> DEP1 & CAP1

    CR -.-> P7
    P7 -.-> IMP1
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto            | Por qué revisarlo                                                               |
| ----- | ------------------------------------ | ------------------------------------------------------------------------------- |
| 1     | Elemento del proyecto                | Permite identificar qué parte del software estamos siguiendo                    |
| 2     | Intención o concepto de origen       | Permite conectar el software con negocio, dominio, iniciativa o decisión previa |
| 3     | Ubicación dentro del proyecto        | Permite entender dónde vive y cómo se encuentra                                 |
| 4     | Estructura técnica                   | Permite entender cómo se organiza y qué límites respeta                         |
| 5     | Comportamiento implementado          | Permite conectar la estructura técnica con lo que debe ocurrir                  |
| 6     | Decisiones técnicas                  | Permiten entender por qué se eligió esa forma de materialización                |
| 7     | Dependencias, capacidades o adapters | Permiten entender qué necesita para funcionar o evolucionar                     |
| 8     | Impacto de evolución                 | Permite entender qué podría cambiar si el elemento evoluciona                   |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
