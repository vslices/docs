---
artifact:
  kind: document
  type: behavior
  scope: <concept|process|flow|feature|capability|product|service|operation|integration|rule>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: ¿Qué debe ocurrir?

tooling:
  schema:
    version: 0.1.0
  template:
    name: behavior.document
    version: 0.1.0
---

# Documento de Comportamiento - <tema>

## Organización

```mermaid
flowchart LR
    R["Documento de Comportamiento<br/><small>¿Qué debe ocurrir?</small>"]

    B1["Comportamiento esperado<br/><small>¿Qué debe pasar?</small>"]
    B2["Situación inicial<br/><small>¿Desde qué situación parte?</small>"]
    B3["Resultado esperado<br/><small>¿Qué debería quedar como resultado?</small>"]
    B4["Criterios de comportamiento<br/><small>¿Qué debe cumplirse para considerarlo correcto?</small>"]
    B5["Variaciones esperadas<br/><small>¿Qué caminos alternativos pueden ocurrir?</small>"]
    B6["Errores esperados<br/><small>¿Qué puede fallar de forma conocida?</small>"]

    R --> B1 & B2 & B3 & B4 & B5 & B6
```

## Comportamiento esperado

<!--
¿Qué debe pasar?

Describir el comportamiento esperado sin explicar todavía cómo se implementa.
-->

## Situación inicial

<!--
¿Desde qué situación parte?

Indicar el estado, condición o situación observable antes de que ocurra el comportamiento.
-->

## Resultado esperado

<!--
¿Qué debería quedar como resultado?

Describir el resultado visible, conceptual o esperado después de que ocurre el comportamiento.
-->

## Criterios de comportamiento

<!--
¿Qué debe cumplirse para considerar correcto este comportamiento?

Definir criterios verificables sin convertir esta sección en una especificación completa de testing.
-->

- <criterio de comportamiento>

## Variaciones esperadas

<!--
¿Qué caminos alternativos pueden ocurrir?

Describir variaciones normales del comportamiento, no errores.
-->

| Variación | Resultado esperado |
| --- | --- |
| <variación esperada> | <qué debería ocurrir> |

## Errores esperados

<!--
¿Qué puede fallar de forma conocida?

Registrar errores esperados como parte del comportamiento, sin usar excepciones o fallas técnicas inesperadas como control de flujo documental.
-->

| Error esperado | Cuándo ocurre | Resultado esperado |
| --- | --- | --- |
| <error> | <situación que lo produce> | <qué debería ocurrir> |
