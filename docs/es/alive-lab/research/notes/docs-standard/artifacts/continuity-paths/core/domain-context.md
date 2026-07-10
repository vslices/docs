---
artifact:
  kind: continuity-path
  type: domain-context
  scope: domain-context
  target: <domain-context-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: []

continuity:
  question: ¿Qué lenguaje, conceptos, reglas y comportamientos pertenecen a este contexto?
  preserves: semantic-continuity
  connects:
    - artifact: <artifact-id>
      role: <language|domain-concept|domain-invariant|behavior|capability|client-product|consumable-service|decision|boundary>

tooling:
  schema:
    version: 0.1.0
  template:
    name: domain-context.continuity-path
    version: 0.1.0
---

# Camino de continuidad "Contexto de dominio" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad semántica del negocio se busca preservar.
No explicar todavía todo el escenario operativo; eso pertenece al Camino de continuidad de Escenario de negocio.
-->

Este path busca preservar continuidad entre `<tema>` y el lenguaje, conceptos, reglas, comportamientos, responsabilidades y límites conceptuales que pertenecen a una parte específica del negocio.

Ayuda a entender cómo se organiza semánticamente una parte del negocio antes de convertirla en productos, servicios, capacidades, decisiones de software o estructuras técnicas.

Un contexto de dominio puede representar una zona conceptual del negocio donde ciertos términos, reglas, comportamientos y responsabilidades tienen un significado específico.

No todo escenario de negocio necesita ser un único contexto de dominio.

Un mismo escenario puede contener varios contextos de dominio, y un mismo término puede cambiar de significado entre contextos distintos.

## Punto de entrada

<!--
¿Por dónde empieza este camino?

Indicar la parte del negocio, zona conceptual, término, regla, comportamiento, capacidad, límite semántico o ambigüedad desde donde parte el recorrido.
-->

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Domain Context.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    A[["<b>Domain Context</b><br/>[Contexto de dominio]<br/><small>Domain Context Path<br/>Context Document<br/>Domain Vocabulary<br/>Scope Document<br/>Support Note kind: draft</small>"]]

    A --> P1["¿Qué lenguaje pertenece a este contexto?"]
    A --> P2["¿Qué conceptos abarca?"]
    A --> P3["¿Qué comportamientos expresa?"]
    A --> P4["¿Qué capacidades nacen desde este dominio?"]
    A -.-> P5["¿Qué productos o servicios usan este significado?"]
    A -.-> P6["¿Qué decisiones delimitan este contexto?"]

    P1 --> L1[["<b>Domain Vocabulary</b><br/>[Definiciones de términos]<br/><small>Domain Vocabulary<br/>Support Note kind: draft<br/>Support Note kind: risk<br/>Decision Record</small>"]]

    P2 --> C1[["<b>Domain Concept</b><br/>[Concepto documentado]<br/><small>Domain Vocabulary<br/>Context Document<br/>Consistency Document</small>"]]
    P2 --> C2{{"<b>Domain Concept</b><br/>[Concepto que requiere definición]<br/><small>Domain Vocabulary<br/>Context Document<br/>Scope Document<br/>Consistency Document<br/>Support Note kind: draft<br/>Support Note kind: risk</small>"}}
    P2 --> I1{{"<b>Domain Invariant</b><br/>[Invariante que requiere documentación]<br/><small>Consistency Document<br/>Behavior Document<br/>Decision Record<br/>Support Note kind: validation<br/>Support Note kind: risk</small>"}}

    P3 --> B1[["<b>Behavior</b><br/>[Comportamiento documentado]<br/><small>Behavior Document<br/>Consistency Document<br/>Support Note kind: testing-spec<br/>Support Note kind: validation<br/>Support Note kind: risk</small>"]]
    P3 --> B2>"<b>Behavior</b><br/>[Comportamiento identificado]"]

    P4 --> CA1{{"<b>Capability</b><br/>[Capacidad candidata]<br/><small>Capability Nexus<br/>Scope Document<br/>Behavior Document<br/>Structure Document<br/>Consistency Document<br/>Viability Document<br/>Decision Record<br/>Support Note kind: draft<br/>Support Note kind: risk</small>"}}
    P4 --> CA2>"<b>Capability</b><br/>[Capacidad identificada]"]

    P5 -.-> Pdt[["<b>Client Product</b><br/>[Producto al cliente]<br/><small>Client Product Path<br/>Context Document<br/>Behavior Document<br/>Mockup Flow<br/>Feedback Document<br/>Domain Vocabulary</small>"]]
    P5 -.-> Svc[["<b>Consumable Service</b><br/>[Servicio consumible]<br/><small>Consumable Service Path<br/>Structure Document<br/>Behavior Document<br/>Consistency Document<br/>Domain Vocabulary<br/>Decision Record</small>"]]

    P6 -.-> D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small>Decision Record<br/>Scope Document<br/>Context Document<br/>Update Document</small>"]]
    P6 -.-> D2{{"<b>Domain Boundary Decision</b><br/>[Decisión pendiente]<br/><small>Decision Record<br/>Scope Document<br/>Context Document<br/>Update Document<br/>Support Note kind: draft<br/>Support Note kind: risk</small>"}}
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
| 3     | Conceptos, reglas e invariantes            | Permite reconocer qué significados y condiciones deben respetarse dentro del contexto                        |
| 4     | Comportamientos propios                    | Permite entender qué acciones o respuestas expresan intención del dominio                                    |
| 5     | Capacidades candidatas                     | Permite reconocer qué capacidades podrían nacer desde este dominio                                           |
| 6     | Productos o servicios que usan el contexto | Permite entender qué piezas dependen de este significado                                                     |
| 7     | Decisiones de límite                       | Permite entender por qué ciertos conceptos, nombres o responsabilidades pertenecen aquí y no a otro contexto |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender este contexto sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con el contexto | Path o artifact sugerido |
| ----------------------- | ------------------------ | ------------------------ |
| <concepto>              | <relación>               | <path o artifact>        |
