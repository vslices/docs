# Camino de continuidad "Evolución" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de cambio, alcance, intención preservada, actualización y aprendizaje se busca sostener.
-->

Este path busca preservar continuidad cuando `<tema>` cambia en el tiempo.

Ayuda a entender qué cambió, por qué cambió, qué intención debe seguir viva, qué alcance entra o sale, qué decisiones explican la evolución, qué aprendizaje la justifica y qué artifacts deben actualizarse para no perder continuidad.

Este path es especialmente útil cuando aparecen cambios de alcance, cambios de dirección, nuevas restricciones, feedback de usuarios, validaciones, reemplazos, exclusiones, postergaciones o ajustes importantes de comprensión.

En esta perspectiva, evolución no significa documentar cada cambio menor.

Significa seguir cambios que pueden alterar intención, alcance, comportamiento esperado, reglas, decisiones relevantes, productos, servicios o continuidad futura.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el elemento cuyo cambio o evolución se quiere seguir.
-->

El recorrido debería comenzar desde el elemento cuya evolución se quiere entender.

Ese punto de entrada puede ser:

* un cambio de alcance
* una inclusión nueva
* una exclusión nueva
* una reducción de alcance
* una ampliación de alcance
* una postergación
* una decisión de reemplazo
* una nueva restricción
* un feedback recibido
* una validación realizada
* una idea del cliente que cambió
* una feature que cambió de forma
* un producto que cambió su experiencia
* un servicio que cambió su contrato
* una regla que cambió su aplicación
* una documentación que quedó obsoleta
* una implementación que necesita ajustarse

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Evolution.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Evolving Element</b><br/>[Elemento que evoluciona]<br/><small><a href='link'>Evolution Path</a></small>"]]

    P1["¿Cuál era su intención original?"]
    P2["¿Qué cambió?"]
    P3["¿Por qué cambió?"]
    P4["¿Qué intención debe preservarse?"]
    P5["¿Qué entra, sale o queda pendiente?"]
    P6["¿Qué debe actualizarse?"]
    P7["¿Qué aprendizaje confirma o corrige la evolución?"]
    P8["¿Qué impacto genera el cambio?"]

    O1[["<b>Original Intent</b><br/>[Intención original]<br/><small><a href='link'>Business Driver Path</a><br/><a href='link'>Domain Context Path</a></small>"]]
    O2>"<b>Initial Assumption</b><br/>[Supuesto inicial]"]

    C1[["<b>Change</b><br/>[Cambio documentado]<br/><small><a href='link'>Update Document</a></small>"]]
    C2{{"<b>Change</b><br/>[Cambio que requiere documentación]<br/><small>Update Document<br/>Decision Record</small>"}}

    R1[["<b>Change Reason</b><br/>[Razón documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    R2{{"<b>Change Reason</b><br/>[Razón no clara]<br/><small>Decision Record<br/>Support Note</small>"}}

    PZ1[["<b>Preserved Intent</b><br/>[Intención preservada]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Behavior Document</a></small>"]]
    PZ2>"<b>Preserved Constraint</b><br/>[Restricción preservada]"]

    SC1{{"<b>Scope Change</b><br/>[Cambio de alcance]<br/><small>Scope Document<br/>Update Document<br/>Decision Record</small>"}}
    SC2>"<b>Deferred Scope</b><br/>[Alcance postergado]"]
    SC3>"<b>Excluded Scope</b><br/>[Alcance excluido]"]

    U1{{"<b>Documentation Update</b><br/>[Documento a actualizar]<br/><small>Update Document</small>"}}
    U2>"<b>Implementation Update</b><br/>[Implementación a ajustar]"]

    L1[["<b>Learning</b><br/>[Aprendizaje documentado]<br/><small><a href='link'>Feedback Document</a><br/><a href='link'>Support Note kind: validation</a></small>"]]
    L2{{"<b>Validation</b><br/>[Validación necesaria]<br/><small>Support Note kind: validation</small>"}}

    I1{{"<b>Impact</b><br/>[Impacto a revisar]<br/><small>Impact Path</small>"}}

    A --> P1
    P1 --> O1 & O2

    A --> P2
    P2 --> C1 & C2

    A --> P3
    P3 --> R1 & R2

    A --> P4
    P4 --> PZ1 & PZ2

    A --> P5
    P5 --> SC1 & SC2 & SC3

    A -.-> P6
    P6 -.-> U1 & U2

    A -.-> P7
    P7 -.-> L1 & L2

    A -.-> P8
    P8 -.-> I1
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto                   | Por qué revisarlo                                                 |
| ----- | ------------------------------------------- | ----------------------------------------------------------------- |
| 1     | Elemento que evoluciona                     | Permite identificar qué cambio estamos siguiendo                  |
| 2     | Intención original                          | Permite entender qué no debería perderse al cambiar               |
| 3     | Cambio realizado o propuesto                | Permite reconocer qué se modificó                                 |
| 4     | Razón del cambio                            | Permite entender por qué la evolución era necesaria               |
| 5     | Intención preservada                        | Permite distinguir evolución de ruptura accidental                |
| 6     | Cambio de alcance                           | Permite entender qué entra, sale, se posterga o queda excluido    |
| 7     | Documentación o implementación a actualizar | Permite mantener continuidad entre conocimiento y materialización |
| 8     | Aprendizaje o validación                    | Permite entender qué evidencia confirmó o corrigió la evolución   |
| 9     | Impacto del cambio                          | Permite identificar qué otros elementos pueden verse afectados    |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
