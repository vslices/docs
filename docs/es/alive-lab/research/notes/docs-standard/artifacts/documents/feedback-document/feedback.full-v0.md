---
artifact:
  kind: document
  type: feedback
  scope: <artifact|document|behavior|feature|product|service|initiative|experiment|decision|flow>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: ¿Qué recibimos al aplicar algo?
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

    B6["Tipo de feedback<br/><small>¿Qué clase de respuesta recibimos?</small>"]
    B7["Señal principal<br/><small>¿Qué mensaje o patrón parece más relevante?</small>"]
    B8["Impacto potencial<br/><small>¿Qué podría verse afectado por este feedback?</small>"]
    B9["Respuesta sugerida<br/><small>¿Qué acción podría considerarse después?</small>"]
    B10["Feedback no resuelto<br/><small>¿Qué queda pendiente de entender?</small>"]

    R --> B1 & B2 & B3 & B4 & B5
    R -.-> B6 & B7 & B8 & B9 & B10
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

## Tipo de feedback

<!--
¿Qué clase de respuesta recibimos?

Clasificar el feedback solo si aporta claridad. No forzar clasificación cuando el feedback sea ambiguo.
-->

| Tipo | Descripción |
| --- | --- |
| <problema, duda, sugerencia, aprobación, rechazo, confusión, validación, etc.> | <descripción breve> |

## Señal principal

<!--
¿Qué mensaje o patrón parece más relevante?

Identificar la señal más importante del feedback sin convertirla todavía en decisión.
-->

## Impacto potencial

<!--
¿Qué podría verse afectado por este feedback?

Explorar qué documento, artifact, comportamiento, decisión, feature, producto o línea de trabajo podría verse afectado.
-->

| Elemento potencialmente afectado | Posible impacto |
| --- | --- |
| <elemento> | <cómo podría verse afectado> |

## Respuesta sugerida

<!--
¿Qué acción podría considerarse después?

Registrar una posible respuesta sin convertirla todavía en decisión formal.
-->

- <acción posible>

## Feedback no resuelto

<!--
¿Qué queda pendiente de entender?

Registrar dudas, ambigüedades o señales que requieren más observación antes de decidir.
-->

| Pendiente | Por qué importa |
| --- | --- |
| <duda o ambigüedad> | <por qué debería aclararse> |