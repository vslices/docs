---
artifact:
  kind: support-note
  type: external
  scope: <artifact|document|service|operation|integration|dependency|specification|contract|schema|repository|tool|dashboard|runbook>
  target: <external-reference-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

support:
  question: ¿Dónde vive el artifact externo y cómo debe usarse?
  supports: <artifact-id>

tooling:
  schema:
    version: 0.1.0
  template:
    name: support-note.external
    version: 0.1.0
---

# Nota de Soporte - Externa - <tema>

## Objeto soportado

<!--
¿Qué concepto, servicio, behavior, capability, decisión o artifact necesita esta referencia externa?
-->

## Referencia externa

<!--
¿Dónde vive el artifact externo?

Puede ser archivo, URL, ruta de repo, spec generada, contrato externo o herramienta.
-->

## Qué representa

<!--
¿Qué representa esta referencia dentro de la continuidad documental?
-->

## Cómo se usa

<!--
¿Cómo debería usarse esta referencia?

Indicar si sirve para consumir un servicio, validar contrato, generar cliente, revisar schema, entender integración o complementar documentación.
-->

## Límites de la referencia

<!--
¿Qué no explica esta referencia?

Indicar qué debe seguir viviendo en documentos VSlices: intención, decisiones, contexto, reglas, garantías, riesgos o comportamiento de dominio.
-->
