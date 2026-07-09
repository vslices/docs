# Camino de continuidad "Trazabilidad" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de origen, transformación y materialización se busca preservar.
-->

Este path busca preservar continuidad entre el origen de `<tema>`, las decisiones que lo transformaron, los artifacts que explican su intención y las materializaciones donde terminó viviendo.

Ayuda a responder de dónde viene un concepto, por qué cambió, qué decisiones lo afectaron, qué documentación preserva su intención y dónde terminó expresándose en producto, servicio, proyecto, implementación o documentación.

Este path es útil cuando necesitamos reconstruir una historia de continuidad, no solo entender una perspectiva aislada.

En esta perspectiva, trazabilidad no significa mapear todas las relaciones posibles.

Significa reconstruir las conexiones necesarias para entender origen, transformación y materialización sin convertir cada vínculo en trazabilidad formal obligatoria.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el concepto, decisión, artifact, comportamiento, feature, servicio, producto o implementación cuyo recorrido se quiere reconstruir.
-->

El recorrido debería comenzar desde el elemento cuya historia se quiere reconstruir.

Ese punto de entrada puede ser:

* una necesidad
* una oportunidad
* una regla
* una decisión
* una feature
* un comportamiento
* un artifact
* un producto al cliente
* un servicio consumible
* una capacidad
* una implementación
* una validación
* un feedback
* un cambio observado
* una actualización documental
* una exclusión o postergación
* una materialización que perdió contexto

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Traceability.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Traceable Element</b><br/>[Elemento trazado]<br/><small><a href='link'>Traceability Path</a></small>"]]

    P1["¿Cuál fue su origen?"]
    P2["¿Qué decisiones lo transformaron?"]
    P3["¿Qué artifacts preservan su intención?"]
    P4["¿Dónde se materializó?"]
    P5["¿Qué validaciones o feedback cambiaron su forma?"]
    P6["¿Qué quedó pendiente, excluido o reemplazado?"]
    P7["¿Qué evolución explica su estado actual?"]

    O1[["<b>Business Driver</b><br/>[Motivación de origen]<br/><small><a href='link'>Business Driver Path</a></small>"]]
    O2[["<b>Domain Context</b><br/>[Origen conceptual]<br/><small><a href='link'>Domain Context Path</a></small>"]]
    O3>"<b>Observed Need</b><br/>[Necesidad observada]"]

    D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    D2{{"<b>Decision Gap</b><br/>[Decisión no documentada]<br/><small>Decision Record</small>"}}

    A1[["<b>Artifact</b><br/>[Artifact relacionado]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Behavior Document</a></small>"]]
    A2>"<b>Support Note</b><br/>[Nota relacionada]"]

    M1[["<b>Client Product</b><br/>[Materialización visible]<br/><small><a href='link'>Client Product Path</a></small>"]]
    M2[["<b>Consumable Service</b><br/>[Materialización consumible]<br/><small><a href='link'>Consumable Service Path</a></small>"]]
    M3[["<b>Software Project</b><br/>[Materialización técnica]<br/><small><a href='link'>Software Project Path</a></small>"]]

    V1[["<b>Feedback</b><br/>[Feedback documentado]<br/><small><a href='link'>Feedback Document</a></small>"]]
    V2{{"<b>Validation</b><br/>[Validación relevante]<br/><small>Support Note kind: validation</small>"}}

    PND{{"<b>Pending / Excluded / Replaced</b><br/>[Pendiente, excluido o reemplazado]<br/><small>Scope Document<br/>Update Document<br/>Decision Record</small>"}}

    E1[["<b>Evolution</b><br/>[Evolución documentada]<br/><small><a href='link'>Evolution Path</a></small>"]]
    E2>"<b>Scope Change</b><br/>[Cambio de alcance identificado]"]

    A --> P1
    P1 --> O1 & O2 & O3

    A --> P2
    P2 --> D1 & D2

    A --> P3
    P3 --> A1 & A2

    A --> P4
    P4 --> M1 & M2 & M3

    A -.-> P5
    P5 -.-> V1 & V2

    A -.-> P6
    P6 -.-> PND

    A -.-> P7
    P7 -.-> E1 & E2
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto         | Por qué revisarlo                                                |
| ----- | --------------------------------- | ---------------------------------------------------------------- |
| 1     | Elemento trazado                  | Permite identificar qué historia se quiere reconstruir           |
| 2     | Origen                            | Permite entender de dónde nace la necesidad, concepto o decisión |
| 3     | Decisiones de transformación      | Permite entender por qué cambió de forma                         |
| 4     | Artifacts que preservan intención | Permite encontrar dónde quedó explicado                          |
| 5     | Materialización                   | Permite entender dónde terminó viviendo                          |
| 6     | Feedback o validación             | Permite entender qué aprendizaje cambió su forma                 |
| 7     | Pendiente, excluido o reemplazado | Permite entender qué no se materializó y por qué                 |
| 8     | Evolución relevante               | Permite entender qué cambios explican su estado actual           |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
