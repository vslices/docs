---
artifact:
  kind: support-note
  type: risk
  scope: <concept|artifact|document|decision|behavior|capability|initiative|product|service|project|handoff|ownership|impact|change|operation|integration>
  target: <risk-subject-name>
  language: <es>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

support:
  question: ¿Qué podría salir mal?
  supports: <artifact-id>

tooling:
  schema:
    version: 0.1.0
  template:
    name: support-note.risk
    version: 0.1.0
---

# Nota de Soporte - Riesgo - <tema>

## Objeto soportado

<!--
¿Qué concepto, decisión, artifact, comportamiento, iniciativa o cambio tiene riesgo asociado?
-->

## Riesgo identificado

<!--
¿Qué podría salir mal?
-->

## Condición de aparición

<!--
¿Cuándo o bajo qué condición podría aparecer este riesgo?
-->

## Posible consecuencia

<!--
¿Qué podría verse afectado si ocurre?
-->

## Uso esperado

<!--
¿Cómo debería usarse esta nota?
Indicar si debería alimentar viabilidad, decisión, alcance, impacto, actualización o validación.
-->