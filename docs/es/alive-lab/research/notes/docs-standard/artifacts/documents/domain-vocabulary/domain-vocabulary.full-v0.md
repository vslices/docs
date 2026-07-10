---
artifact:
  kind: document
  type: domain-vocabulary
  scope: <domain-context|business-scenario|project|product|service|organization>
  target: <vocabulary-target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: []

document:
  question: ¿Cómo hablamos?

tooling:
  schema:
    version: 0.1.0
  template:
    name: domain-vocabulary.document
    version: 0.1.0
---

# Vocabulario de dominio: <tema>

## Organización

```mermaid
flowchart LR
    R["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]
    B1["Terminología<br/><small>¿Qué términos usamos?</small>"]
    B2["Términos en desuso<br/><small>¿Qué términos ya no usamos?</small>"]
    B3["Regla de uso<br/><small>¿Cuándo usar este vocabulario?</small>"]
    B4["Gobernanza<br/><small>¿Qué persona, equipo o rol mantiene este vocabulario?</small>"]

    R --> B1 & B2 & B3
    R -.-> B4
        
```

## Terminología

<!-- 
¿Qué términos usamos? 
-->

- <término 1>
- <término 2>
- <término 3>

## Términos en desuso

<!-- 
¿Qué términos ya no usamos?
-->

- <término 1>
- <término 2>

## Regla de uso

<!-- 
¿Cuándo usar este vocabulario? 

Explicar cuándo este vocabulario debe usarse como referencia común dentro del dominio, contexto, proyecto o línea de trabajo.
-->

## Gobernanza

<!-- 
¿Qué persona, equipo o rol mantiene este vocabulario?
-->