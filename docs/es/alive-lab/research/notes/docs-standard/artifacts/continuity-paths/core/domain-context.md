# Camino de continuidad "Contexto de dominio" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad semántica del negocio se busca preservar.
No explicar todavía todo el escenario operativo; eso pertenece al Camino de continuidad de Escenario de negocio.
-->

Este path busca preservar continuidad entre `<tema>` y el lenguaje, reglas, comportamientos, responsabilidades y límites conceptuales que pertenecen a una parte específica del negocio.

Ayuda a entender cómo se organiza semánticamente una parte del negocio antes de convertirla en productos, servicios, capacidades, decisiones de software o estructuras técnicas.

Un contexto de dominio puede representar una zona conceptual del negocio donde ciertos términos, reglas, comportamientos y responsabilidades tienen un significado específico.

No todo escenario de negocio necesita ser un único contexto de dominio.

Un mismo escenario puede contener varios contextos de dominio, y un mismo término puede cambiar de significado entre contextos distintos.

## Punto de entrada

<!--
¿Por dónde conviene empezar?

Indicar la parte del negocio, zona conceptual, término, regla, comportamiento, capacidad o límite semántico desde donde parte el recorrido.
-->

El recorrido debería comenzar desde la parte del negocio o zona conceptual que se quiere entender o seguir.

Ese punto de entrada puede ser:

* una parte del negocio
* una zona conceptual
* un término del dominio
* una regla de negocio
* una invariante
* un comportamiento propio del contexto
* una responsabilidad del dominio
* una capacidad candidata
* una frontera conceptual
* una ambigüedad semántica
* un término que cambia de significado entre contextos
* una decisión que delimita un contexto

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Domain Context.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Domain Context</b><br/>[Contexto de dominio]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Domain Context Path</a></small>"]]

    P1["¿Qué lenguaje pertenece a este contexto?"]
    P2["¿Qué conceptos abarca?"]
    P3["¿Qué comportamientos expresa?"]
    P4["¿Qué capacidades nacen desde este dominio?"]
    P5["¿Qué productos o servicios usan este significado?"]
    P6["¿Qué decisiones delimitan este contexto?"]

    L1[["<b>Domain Vocabulary</b><br/>[Definiciones de términos]<br/><small><a href='link'>Domain Vocabulary</a></small>"]]
    
    R1[["<b>Domain concept</b><br/>[Nombre concepto]<br/><small><a href='link'>Consistency Document</a></small>"]]
    R2{{"<b>Domain Invariant</b><br/>[Invariante que requiere documentación]<br/><small>Consistency Document</small>"}}

    B1[["<b>Behavior</b><br/>[Comportamiento documentado]<br/><small><a href='link'>Behavior Document</a></small>"]]
    B2>"<b>Behavior</b><br/>[Comportamiento identificado]"]

    C1{{"<b>Capability</b><br/>[Capacidad candidata]<br/><small>Scope Document<br/>Structure Document<br/>Behavior Document</small>"}}
    C2>"<b>Capability</b><br/>[Capacidad identificada]"]

    Pdt[["<b>Client Product</b><br/>[Producto al cliente]<br/><small><a href='link'>Client Product Path</a></small>"]]
    Svc[["<b>Consumable Service</b><br/>[Servicio consumible]<br/><small><a href='link'>Consumable Service Path</a></small>"]]

    D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small><a href='link'>Decision Record</a></small>"]]
    D2{{"<b>Domain Boundary Decision</b><br/>[Decisión pendiente]<br/><small>Decision Record</small>"}}

    A --> P1 --> L1

    A --> P2
    P2 --> R1 & R2

    A --> P3
    P3 --> B1 & B2

    A --> P4
    P4 --> C1 & C2

    A -.-> P5
    P5 -.-> Pdt & Svc

    A -.-> P6
    P6 -.-> D1 & D2
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto                  | Por qué revisarlo                                                                                            |
| ----- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| 1     | Contexto de dominio                        | Permite identificar qué zona conceptual del negocio estamos siguiendo                                        |
| 2     | Lenguaje del contexto                      | Permite entender qué términos y significados pertenecen a esta parte del negocio                             |
| 3     | Reglas o invariantes                       | Permite reconocer qué condiciones deben respetarse dentro del contexto                                       |
| 4     | Comportamientos propios                    | Permite entender qué acciones o respuestas expresan intención del dominio                                    |
| 5     | Capacidades candidatas                     | Permite reconocer qué capacidades podrían nacer desde este dominio                                           |
| 6     | Productos o servicios que usan el contexto | Permite entender qué piezas dependen de este significado                                                     |
| 7     | Decisiones de límite                       | Permite entender por qué ciertos conceptos, nombres o responsabilidades pertenecen aquí y no a otro contexto |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este escenario sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el escenario | Path o artifact sugerido |
| ----------------------- | ------------------------- | ------------------------ |
| <concepto>              | <relación>                | <path o artifact>        |
