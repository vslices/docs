---
artifact:
  kind: document
  type: domain-vocabulary
  scope: <domain-context|business-scenario|project|product|service|organization>
  target: <vocabulary-target-name>
  language: es

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references|referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes|superseded-by>
      target: <artifact-id>

document:
  question: ¿Cómo hablamos?

tooling:
  schema:
    version: 0.1.0
  template:
    name: domain-vocabulary.document
    version: 0.1.0
---

# Vocabulario de dominio - <tema>

## Organización

```mermaid
flowchart LR
    R["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]

    B1["Terminología<br/><small>¿Qué términos usamos?</small>"]
    B2["Términos en desuso<br/><small>¿Qué términos ya no usamos?</small>"]
    B3["Regla de uso<br/><small>¿Cuándo usar este vocabulario?</small>"]
    B4["Gobernanza<br/><small>¿Qué persona, equipo o rol mantiene este vocabulario?</small>"]

    B1_1["Definición<br/><small>¿Qué significa este término?</small>"]
    B1_2["Contexto de uso<br/><small>¿Dónde aparece este término?</small>"]
    B1_3["Ambigüedad<br/><small>¿Con qué se puede confundir?</small>"]
    B1_4["Términos relacionados<br/><small>¿Con qué otros términos se conecta?</small>"]

    B2_1["Reemplazo<br/><small>¿Qué término usamos ahora?</small>"]
    B2_2["Motivo de desuso<br/><small>¿Por qué dejamos de usarlo?</small>"]
    B2_3["Estado histórico<br/>¿Sigue apareciendo en artifacts antiguos?"]

    B3_1["Ámbito de aplicación<br/><small>¿Dónde aplica este vocabulario?</small>"]
    B3_2["Audiencia<br/><small>¿Quién debería usarlo?</small>"]

    B4_1["Responsable<br/><small>¿Quién decide cambios?</small>"]
    B4_2["Criterio de actualización<br/><small>¿Cuándo debe actualizarse?</small>"]
    B4_3["Fuente de cambio<br/><small>¿De dónde puede venir una actualización?</small>"]

    R --> B1 & B2 & B3
    R -.-> B4

    B1 --> B1_1 & B1_2 & B1_3 & B1_4
    B2 --> B2_1 & B2_2 & B2_3
    B3 --> B3_1 & B3_2
    B4 -.-> B4_1 & B4_2 & B4_3
```

## Terminología

<!-- 
¿Qué términos usamos? 
- ¿Qué significa este término?
- ¿Dónde aparece este término?
- ¿Con qué se puede confundir?
- ¿Con qué otros términos se conecta?
-->


| Término   | Definición                   | Contexto de uso                 | Ambigüedad                   | Términos relacionados |
| --------- | ---------------------------- | ------------------------------- | ---------------------------- | --------------------- |
| <término> | <qué significa este término> | <dónde aparece o cuándo aplica> | <con qué podría confundirse> | <términos conectados> |

## Términos en desuso

<!-- 
¿Qué términos ya no usamos?
- ¿Qué término usamos ahora?
- ¿Por qué dejamos de usarlo?
- ¿Sigue apareciendo en artifacts antiguos?
-->

| Término en desuso  | Reemplazo        | Motivo de desuso            | Estado histórico                     |
| ------------------ | ---------------- | --------------------------- | --- |
| <término anterior> | <término actual> | <por qué dejamos de usarlo> | <dónde sigue apareciendo, si aplica> |

## Regla de uso

<!-- 
¿Cuándo usar este vocabulario? 
-->

### Ámbito de aplicación

<!-- 
¿Dónde aplica este vocabulario? 

Explicar en qué dominio, bounded context, proyecto, producto, equipo o línea de trabajo aplica este vocabulario.
-->

### Audiencia

<!-- 
¿Quién debería usarlo? 

Indicar qué personas, roles o equipos deberían usar este vocabulario como referencia.
-->

## Gobernanza

<!-- 
¿Qué persona, equipo o rol mantiene este vocabulario? 
-->

### Responsable

<!-- 
¿Quién decide cambios? 

Indicar quién puede proponer, revisar, aprobar o mantener cambios sobre este vocabulario.
-->

### Criterio de actualización

<!-- 
¿Cuándo debe actualizarse? 

Explicar cuándo este vocabulario debería revisarse o actualizarse.
-->

### Fuente de cambio

<!--
¿De dónde puede venir una actualización?

Indicar si los cambios pueden venir de conversaciones de dominio, feedback, decisiones, implementación, investigación, uso real u otros artifacts.
-->
