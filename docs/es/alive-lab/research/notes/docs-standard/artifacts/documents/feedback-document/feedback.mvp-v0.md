---
artifact:
  kind: document
  type: feedback
  scope: <artifact|document|behavior|feature|product|service|initiative|experiment|decision|flow>
  target: <target-name>
  language: <es>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: ¿Qué recibimos al aplicar algo?
  feedback:
    source: <user|stakeholder|team|client|system|reviewer|ai|community|operation|usage>

tooling:
  schema:
    version: 0.1.0
  template:
    name: feedback.document
    version: 0.1.0
---

# Documento de Feedback - <tema>

## Organización

```mermaid
flowchart LR
    R["Documento de Feedback<br/><small>¿Qué recibimos al aplicar algo?</small>"]

    B1["Objeto observado<br/><small>¿Sobre qué recibimos feedback?</small>"]
    B2["Fuente del feedback<br/><small>¿Quién o qué entregó la respuesta?</small>"]
    B3["Feedback recibido<br/><small>¿Qué respuesta recibimos?</small>"]
    B4["Contexto de recepción<br/><small>¿Cuándo, dónde o bajo qué situación se recibió?</small>"]
    B5["Uso esperado<br/><small>¿Cómo debería usarse este feedback?</small>"]

    R --> B1 & B2 & B3 & B4 & B5
```

## Objeto observado

<!--
¿Sobre qué recibimos feedback?

Indicar el artifact, documento, comportamiento, producto, feature, experimento, decisión o elemento sobre el que se recibió feedback.
-->

## Fuente del feedback

<!--
¿Quién o qué entregó la respuesta?

Indicar usuario, stakeholder, equipo, cliente, sistema, reviewer, IA, comunidad u otra fuente externa.
-->

## Feedback recibido

<!--
¿Qué respuesta recibimos?

Registrar el feedback recibido sin convertirlo todavía en decisión, actualización o validación.
-->

## Contexto de recepción

<!--
¿Cuándo, dónde o bajo qué situación se recibió?

Preservar las condiciones mínimas necesarias para entender el feedback.
-->

## Uso esperado

<!--
¿Cómo debería usarse este feedback?

Indicar si este feedback debería alimentar una decisión, actualización documental, validación, investigación o iteración futura.
-->