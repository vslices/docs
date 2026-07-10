---
artifact:
  kind: document
  type: context
  scope: <concept|process|flow|feature|capability|initiative|product|service|project|organization|domain-context|handoff>
  target: <target-name>
  language: es

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references|referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes|superseded-by>
      target: <artifact-id>

document:
  question: ¿Dónde existe?

tooling:
  schema:
    version: 0.1.0
  template:
    name: context.document
    version: 0.1.0
---

# Documento de Contexto - <tema>

## Organización

```mermaid
flowchart LR
    R["Documento de Contexto<br/><small>¿Dónde existe?</small>"]

    B1["Escenario<br/><small>¿En qué situación aparece?</small>"]
    B2["Motivación contextual<br/><small>¿Por qué importa entender este contexto?</small>"]
    B3["Situación actual<br/><small>¿Qué ocurre hoy?</small>"]
    B4["Elementos involucrados<br/><small>¿Qué personas, sistemas, procesos o artifacts participan?</small>"]
    B5["Límites iniciales<br/><small>¿Dónde aplica este contexto?</small>"]

    R --> B1 & B2 & B3 & B4 & B5
```

## Escenario

<!--
¿En qué situación aparece este concepto, problema, sistema, capacidad, decisión o artifact?
-->

## Motivación contextual

<!--
¿Por qué importa entender este contexto?

Explicar qué se pierde, confunde o dificulta si este contexto no se preserva.
-->

## Situación actual

<!--
¿Qué ocurre hoy?

Describir el estado actual de la situación sin entrar todavía en solución detallada.
-->

## Elementos involucrados

<!--
¿Qué personas, sistemas, procesos o artifacts participan en este contexto?

No describir todavía estructura completa, ownership detallado ni responsabilidades formales.
-->

| Tipo | Elemento | Participación en el contexto |
| --- | --- | --- |
| <actor, sistema, proceso o artifact> | <nombre> | <cómo participa o por qué importa> |

## Límites iniciales

<!--
¿Dónde aplica este contexto?

Indicar los límites iniciales del contexto sin convertir esta sección en un Documento de Alcance completo.
-->