# Camino de continuidad "Responsabilidad" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de responsabilidad, conocimiento, decisión, validación, operación o mantenimiento se busca preservar.
-->

Este path busca preservar continuidad sobre quién entiende, decide, valida, mantiene, opera o responde por `<tema>`.

Ayuda a evitar que un concepto, artifact, producto, servicio, decisión o comportamiento quede documentado sin claridad sobre las personas, roles, equipos o áreas que sostienen su conocimiento y evolución.

Este path es especialmente útil cuando la pérdida de ownership puede producir abandono, decisiones inconsistentes, dependencia tácita o conocimiento atrapado en personas específicas.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el concepto, artifact, decisión, sistema, proceso, producto, servicio o responsabilidad que se quiere seguir.
-->

El recorrido debería comenzar desde el elemento cuya responsabilidad se quiere entender.

Ese punto de entrada puede ser:

* un concepto de dominio
* una decisión
* un artifact
* una línea de trabajo
* un proceso
* un producto
* un servicio consumible
* una capacidad
* una feature
* una operación
* una regla o invariante
* una parte del sistema que requiere mantenimiento

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Ownership.
-->

```mermaid
flowchart LR
    A[["<b>Owned Element</b><br/>[Elemento seguido]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Ownership Path</a></small>"]]

    P1["¿Quién lo entiende?"]
    P2["¿Quién decide sobre esto?"]
    P3["¿Quién lo valida?"]
    P4["¿Quién lo mantiene u opera?"]
    P5["¿Qué conocimiento depende de personas específicas?"]
    P6["¿Qué cambia si la responsabilidad se mueve?"]

    K1[["<b>Knowledge Owner</b><br/>[Responsable de conocimiento]<br/><small><a href='link'>Context Document</a></small>"]]
    K2>"<b>Knowledge Source</b><br/>[Persona o equipo identificado]"]

    D1[["<b>Decision Owner</b><br/>[Responsable de decisión]<br/><small><a href='link'>Decision Record</a></small>"]]
    D2{{"<b>Decision Gap</b><br/>[Responsabilidad de decisión no clara]<br/><small>Decision Record<br/>Support Note</small>"}}

    V1[["<b>Validation Owner</b><br/>[Responsable de validación]<br/><small><a href='link'>Support Note kind: validation</a></small>"]]
    V2>"<b>Validation Source</b><br/>[Fuente de validación identificada]"]

    M1[["<b>Maintenance Owner</b><br/>[Responsable de mantenimiento]<br/><small><a href='link'>Structure Document</a></small>"]]
    M2{{"<b>Operational Responsibility</b><br/>[Responsabilidad operativa pendiente]<br/><small>Context Document<br/>Decision Record</small>"}}

    T1{{"<b>Tacit Knowledge</b><br/>[Conocimiento tácito]<br/><small>Support Note<br/>Domain Vocabulary</small>"}}

    I1{{"<b>Ownership Impact</b><br/>[Impacto por cambio de responsabilidad]<br/><small>Impact Path</small>"}}

    A --> P1
    P1 --> K1 & K2

    A --> P2
    P2 --> D1 & D2

    A --> P3
    P3 --> V1 & V2

    A --> P4
    P4 --> M1 & M2

    A -.-> P5
    P5 -.-> T1

    A -.-> P6
    P6 -.-> I1
```

## Recorrido recomendado

| Orden | Nodo, artifact o concepto                | Por qué revisarlo                                                            |
| ----- | ---------------------------------------- | ---------------------------------------------------------------------------- |
| 1     | Elemento seguido                         | Permite identificar sobre qué responsabilidad estamos navegando              |
| 2     | Responsable de conocimiento              | Permite entender quién puede explicar el elemento                            |
| 3     | Responsable de decisión                  | Permite saber quién puede cambiar, aprobar o delimitar el elemento           |
| 4     | Responsable de validación                | Permite saber quién confirma si el elemento funciona o sigue siendo correcto |
| 5     | Responsable de mantenimiento u operación | Permite entender quién sostiene el elemento en el tiempo                     |
| 6     | Conocimiento tácito                      | Permite detectar riesgo de pérdida de continuidad                            |
| 7     | Impacto por cambio de responsabilidad    | Permite entender qué podría romperse si el ownership cambia                  |

Al terminar este recorrido debería entenderse:

* qué elemento se está siguiendo
* quién lo entiende
* quién puede decidir sobre él
* quién puede validarlo
* quién lo mantiene u opera
* qué conocimiento está explícito
* qué conocimiento depende de personas específicas
* qué riesgo existe si la responsabilidad cambia
* qué documentación podría preservar continuidad

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
