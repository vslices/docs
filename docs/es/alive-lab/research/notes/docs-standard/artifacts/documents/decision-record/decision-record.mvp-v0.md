---
artifact:
  kind: document
  type: decision-record
  scope: <concept|domain-context|feature|capability|initiative|product|service|project|architecture|scope|viability|ownership|handoff>
  target: <decision-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: ¿Qué se decidió?
  decision_status: <proposed|accepted|active|rejected|superseded|archived>

tooling:
  schema:
    version: 0.1.0
  template:
    name: decision-record.document
    version: 0.1.0
---

# Decision Record - <tema>

## Organización

```mermaid
flowchart LR
    R["Decision Record<br/><small>¿Qué se decidió?</small>"]

    B1["Decisión<br/><small>¿Qué decisión se tomó?</small>"]
    B2["Contexto de decisión<br/><small>¿Por qué fue necesario decidir?</small>"]
    B3["Alternativas consideradas<br/><small>¿Qué otras opciones se evaluaron?</small>"]
    B4["Razón principal<br/><small>¿Por qué se eligió esta opción?</small>"]
    B5["Consecuencias esperadas<br/><small>¿Qué cambia por esta decisión?</small>"]
    B6["Estado de la decisión<br/><small>¿En qué estado queda esta decisión?</small>"]

    R --> B1 & B2 & B3 & B4 & B5 & B6
```

## Decisión

<!--
¿Qué decisión se tomó?

Declarar la decisión de forma directa.
-->

## Contexto de decisión

<!--
¿Por qué fue necesario decidir?

Explicar el contexto mínimo que hizo necesaria esta decisión.
No convertir esta sección en un Documento de Contexto completo.
-->

## Alternativas consideradas

<!--
¿Qué otras opciones se evaluaron?

Registrar alternativas relevantes sin hacer un análisis exhaustivo innecesario.
-->

| Alternativa | Motivo para no elegirla |
| --- | --- |
| <alternativa> | <por qué no fue elegida> |

## Razón principal

<!--
¿Por qué se eligió esta opción?

Explicar el criterio central que justificó la decisión.
-->

## Consecuencias esperadas

<!--
¿Qué cambia por esta decisión?

Describir efectos esperados, ajustes o consecuencias relevantes sin convertir esta sección en planificación completa.
-->

- <consecuencia esperada>

## Estado de la decisión

<!--
¿En qué estado queda esta decisión?

Indicar si la decisión está propuesta, aceptada, activa, reemplazada, descartada o archivada.
-->