---
artifact:
  kind: document
  type: domain-vocabulary
  scope: <domain-context|business-scenario|project|product|service|organization>
  target: <vocabulary-target-name>
  language: <es>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
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

    B1_1_1["Ejemplo de uso<br/><small>¿Cómo se usa correctamente?</small>"]
    B1_1_2["Contraejemplo<br/><small>¿Cómo no debería usarse?</small>"]

    B1_3_1["Diferencia<br/><small>¿Qué lo distingue del término confundido?</small>"]
    B1_3_2["Riesgo de confusión<br/><small>¿Qué problema causa confundirlo?</small>"]

    B1_4_1["Tipo de relación<br/><small>¿Cómo se relacionan estos términos?</small>"]
    B1_4_2["Criterio de preferencia<br/><small>¿Cuándo preferir este término sobre otro?</small>"]

    B2_1["Reemplazo<br/><small>¿Qué término usamos ahora?</small>"]
    B2_2["Motivo de desuso<br/><small>¿Por qué dejamos de usarlo?</small>"]
    B2_3["Estado histórico<br/><small>¿Sigue apareciendo en artifacts antiguos?</small>"]

    B3_1["Ámbito de aplicación<br/><small>¿Dónde aplica este vocabulario?</small>"]
    B3_2["Audiencia<br/><small>¿Quién debería usarlo?</small>"]

    B4_1["Responsable<br/><small>¿Quién decide cambios?</small>"]
    B4_2["Criterio de actualización<br/><small>¿Cuándo debe actualizarse?</small>"]
    B4_3["Fuente de cambio<br/><small>¿De dónde puede venir una actualización?</small>"]
  

    R --> B1 & B2 & B3
    R -.-> B4

    B1 --> B1_1 & B1_2 & B1_3 & B1_4
    B1_1 --> B1_1_1 & B1_1_2
    B1_3 --> B1_3_1 & B1_3_2
    B1_4 --> B1_4_1 & B1_4_2

    B2 --> B2_1 & B2_2 & B2_3
    B3 --> B3_1 & B3_2
    B4 -.-> B4_1 & B4_2 & B4_3

```

## Terminología

<!--
¿Qué términos usamos?
- ¿Qué significa este término?
- ¿Cómo se usa correctamente?
- ¿Cómo no debería usarse?
- ¿Dónde aparece este término?
-->

| Término   | Definición                   | Ejemplo de uso              | Contraejemplo            | Contexto de uso                 |
| --------- | ---------------------------- | --------------------------- | ------------------------ | ------------------------------- |
| <término> | <qué significa este término> | <cómo se usa correctamente> | <cómo no debería usarse> | <dónde aparece o cuándo aplica> |

### Ambigüedades

<!--
¿Con qué se puede confundir?
- ¿Qué lo distingue del término confundido?
- ¿Qué problema causa confundirlo?
-->

| Término   | Se puede confundir con | Diferencia                     | Riesgo de confusión               |
| --------- | ---------------------- | ------------------------------ | --------------------------------- |
| <término> | <otro término>         | <qué distingue ambos términos> | <qué problema causa confundirlos> |

### Términos relacionados

<!--
¿Con qué otros términos se conecta?
- ¿Cómo se relacionan estos términos?
- ¿Cuándo preferir este término sobre el otro?
-->

| Término | Término relacionado | Tipo de relación | Preferir cuando |
| --- | --- | --- | --- |
| <término> | <otro término>      | <cómo se relacionan> | <cuándo preferirlo> |

## Términos en desuso

<!--
¿Qué términos ya no usamos?
- ¿Qué término usamos ahora?
- ¿Por qué dejamos de usarlo?
- ¿Sigue apareciendo en artifacts antiguos?
-->

| Término en desuso  | Reemplazo        | Motivo de desuso            | Estado histórico                     |
| ------------------ | ---------------- | --------------------------- | ------------------------------------ |
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
