# Front-matter base para Support Note artifacts

## Template

```yaml
---
artifact:
  kind: support-note
  type: <draft|result|validation|testing-spec|risk|external>
  scope: <%type-scopes%>
  target: <target-name>
  language: es

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references|referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes|superseded-by>
      target: <artifact-id>

support:
  question: <%type-question%>
  supports: <artifact-id>

tooling:
  schema:
    version: 0.1.0
  template:
    name: <template-name>
    version: 0.1.0
---
```

# Definiciones

## `artifact`

Define la identidad documental de la nota de soporte.

Esta sección responde:

> ¿Qué tipo de support note es esta, qué elemento apoya y en qué idioma está escrita?

* `artifact.kind`: clase general del artifact. Para este grupo siempre debe ser `support-note`.
* `artifact.type`: tipo específico de nota de soporte.
* `artifact.scope`: escala, naturaleza o contexto principal donde aplica la nota.
* `artifact.target`: elemento concreto que la nota apoya, registra o referencia.
* `artifact.language`: idioma principal de la nota. Debe usar valores simples como `es` o `en`.

## `metadata`

Define el estado documental y las relaciones generales de la nota.

Esta sección responde:

> ¿En qué estado está esta nota y con qué otros artifacts se relaciona?

* `metadata.status`: estado actual de la nota dentro de su ciclo de vida documental.
* `metadata.relates`: lista de relaciones generales con otros artifacts, paths, documentos, notas o elementos relevantes.

## `support`

Define el propósito específico de soporte.

Esta sección responde:

> ¿Qué necesita apoyo y qué pregunta auxiliar responde esta nota?

* `support.question`: pregunta específica del tipo de nota.
* `support.supports`: artifact, concepto o elemento principal que recibe apoyo de esta nota.

`support.supports` debe apuntar al elemento soportado principal. Si existen relaciones adicionales, deben declararse en `metadata.relates`.

## `tooling`

Define información mínima para que VSlices Tooling pueda validar, generar, migrar o actualizar la nota.

* `tooling.schema.version`: versión del schema de front-matter usado por esta nota.
* `tooling.template.name`: nombre del template usado para crear o mantener esta nota.
* `tooling.template.version`: versión del template usado.

## Placeholders

* `<draft|result|validation|testing-spec|risk|external>`: tipos permitidos de Support Note.
* `<%type-scopes%>`: scopes permitidos por el tipo específico de nota.
* `<target-name>`: nombre estable del elemento soportado, observado, evaluado o referenciado.
* `<%type-question%>`: pregunta auxiliar que responde el tipo específico de nota.
* `<artifact-id>`: identificador del artifact o elemento principal soportado.
* `<template-name>`: nombre del template usado por tooling.

## Reglas generales

* Una Support Note apoya, registra o referencia.
* Una Support Note no reemplaza un Document artifact.
* Una Support Note no reemplaza un Nexus.
* Una Support Note no reemplaza un Continuity Path.
* Una Support Note puede contener conocimiento incompleto.
* Una Support Note puede existir para evitar documentación prematura.
* Una Support Note debe tener un objeto soportado claro.
* Si la nota crece hasta responder una pregunta documental principal, debería promoverse a Document artifact.
* Si la nota conecta múltiples artifacts como composición, quizá corresponde un Nexus.
* Los campos derivados no deben escribirse manualmente.

## Campos derivados

Estos campos no deberían escribirse manualmente:

* `id`
* `slug`
* `filename`
* `path`
* `title`
* `display_name`
* `canonical_id`
* `last_modified`
* `line_count`

## Identidad derivada sugerida

La identidad canónica puede derivarse con una regla como:

```text
<artifact.kind>.<artifact.type>.<artifact.scope>.<artifact.target>
```

Ejemplo:

```text
support-note.risk.service.payment-api-consumption
```

La regla exacta debe vivir en tooling o en la especificación de identidad documental, no como campo manual obligatorio.
