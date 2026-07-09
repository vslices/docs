# Camino de continuidad "Impacto" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de efectos, consecuencias, dependencias y propagación de cambios se busca preservar.
-->

Este path busca preservar continuidad sobre qué puede verse afectado cuando `<tema>` cambia, aparece, se elimina, se valida, falla o evoluciona.

Ayuda a entender relaciones de impacto entre conceptos, reglas, decisiones, productos, servicios, capacidades, comportamientos, documentos, equipos y partes técnicas del sistema.

Este path es útil cuando no basta con entender un elemento en sí mismo, porque su modificación puede afectar otras piezas del negocio, del producto, del servicio, de la documentación o del proyecto de software.

En esta perspectiva, impacto no significa documentar todas las relaciones posibles.

Significa seguir los efectos relevantes de un cambio para evitar inconsistencias, rupturas, pérdida de intención o actualización incompleta.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar el cambio, decisión, concepto, comportamiento, producto, servicio o elemento cuyo impacto se quiere seguir.
-->

El recorrido debería comenzar desde el elemento cuyo impacto se quiere entender.

Ese punto de entrada puede ser:

* una decisión
* un cambio de alcance
* una regla modificada
* una capacidad nueva
* una feature
* un producto al cliente
* un servicio consumible
* un contrato
* un comportamiento
* un error
* una dependencia
* una validación
* un feedback
* una actualización
* una eliminación
* un reemplazo
* una parte del sistema que cambia

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado a Impact.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Impact Source</b><br/>[Elemento que genera impacto]<br/><small><a href='link'>Impact Path</a></small>"]]

    P1["¿Qué conceptos del dominio afecta?"]
    P2["¿Qué productos o experiencias afecta?"]
    P3["¿Qué servicios o contratos afecta?"]
    P4["¿Qué proyectos o estructuras técnicas afecta?"]
    P5["¿Qué decisiones deben revisarse?"]
    P6["¿Qué documentación debe actualizarse?"]
    P7["¿Qué validación necesita repetirse?"]

    D1[["<b>Domain Concept</b><br/>[Concepto afectado]<br/><small><a href='link'>Domain Context Path</a></small>"]]
    D2>"<b>Domain Rule</b><br/>[Regla afectada]"]

    Pdt1[["<b>Client Product</b><br/>[Producto afectado]<br/><small><a href='link'>Client Product Path</a></small>"]]
    UX1{{"<b>Visible Action</b><br/>[Acción visible afectada]<br/><small>Behavior Document</small>"}}

    S1[["<b>Consumable Service</b><br/>[Servicio afectado]<br/><small><a href='link'>Consumable Service Path</a></small>"]]
    C1{{"<b>Service Contract</b><br/>[Contrato afectado]<br/><small>Structure Document<br/>Decision Record</small>"}}

    SP1[["<b>Software Project</b><br/>[Proyecto afectado]<br/><small><a href='link'>Software Project Path</a></small>"]]
    T1>"<b>Technical Dependency</b><br/>[Dependencia afectada]"]

    DEC1{{"<b>Decision</b><br/>[Decisión a revisar]<br/><small>Decision Record</small>"}}
    UP1{{"<b>Documentation Update</b><br/>[Documento a actualizar]<br/><small>Update Document</small>"}}
    V1{{"<b>Validation</b><br/>[Validación a repetir]<br/><small>Support Note kind: validation</small>"}}

    A --> P1
    P1 --> D1 & D2

    A --> P2
    P2 --> Pdt1 & UX1

    A --> P3
    P3 --> S1 & C1

    A -.-> P4
    P4 -.-> SP1 & T1

    A -.-> P5
    P5 -.-> DEC1

    A -.-> P6
    P6 -.-> UP1

    A -.-> P7
    P7 -.-> V1
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto                  | Por qué revisarlo                                                        |
| ----- | ------------------------------------------ | ------------------------------------------------------------------------ |
| 1     | Elemento que genera impacto                | Permite identificar la fuente del impacto                                |
| 2     | Conceptos del dominio afectados            | Permite entender cambios semánticos, reglas o límites conceptuales       |
| 3     | Productos o experiencias afectadas         | Permite entender cambios visibles para usuarios                          |
| 4     | Servicios o contratos afectados            | Permite entender cambios para consumidores técnicos                      |
| 5     | Proyectos o estructuras técnicas afectadas | Permite entender cambios de implementación, dependencias o mantenimiento |
| 6     | Decisiones a revisar                       | Permite entender si el cambio invalida acuerdos previos                  |
| 7     | Documentación a actualizar                 | Permite preservar continuidad documental                                 |
| 8     | Validación a repetir                       | Permite confirmar que el cambio sigue siendo correcto                    |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
