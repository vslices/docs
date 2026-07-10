# Front-matter base para Document artifacts

## Template

```yaml
---
artifact:
  kind: document
  type: <context|structure|behavior|consistency|scope|viability|feedback|decision-record|navigation|domain-vocabulary|update>
  scope: <%type-scopes%>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: <%type-question%>

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

Define la identidad documental del artifact.

Esta sección responde:

> ¿Qué tipo de documento es este, qué elemento explica y en qué idioma está escrito?

* `artifact.kind`: clase general del artifact. Para este grupo siempre debe ser `document`.
* `artifact.type`: tipo específico de documento.
* `artifact.scope`: escala, naturaleza o contexto principal donde aplica el documento.
* `artifact.target`: elemento concreto que el documento explica.
* `artifact.language`: idioma principal del documento. Debe usar valores simples como `es` o `en`.

## `metadata`

Define el estado documental y las relaciones generales del documento.

Esta sección responde:

> ¿En qué estado está este documento y con qué otros artifacts se relaciona?

* `metadata.status`: estado actual del documento dentro de su ciclo de vida documental.
* `metadata.relates`: lista de relaciones generales con otros artifacts, paths, documentos, notas o elementos relevantes.

## `document`

Define la pregunta documental principal.

Esta sección responde:

> ¿Qué pregunta intenta responder este documento?

* `document.question`: pregunta principal que orienta el contenido del documento.

No debe incluir resumen, propósito largo, conclusiones ni contenido explicativo. Eso pertenece al cuerpo del documento.

## `tooling`

Define información mínima para que VSlices Tooling pueda validar, generar, migrar o actualizar el documento.

* `tooling.schema.version`: versión del schema de front-matter usado por este documento.
* `tooling.template.name`: nombre del template usado para crear o mantener este documento.
* `tooling.template.version`: versión del template usado.

## Placeholders

* `<%type-scopes%>`: scopes permitidos por el tipo específico de documento.
* `<target-name>`: nombre estable del elemento explicado.
* `<%type-question%>`: pregunta principal del tipo documental.
* `<template-name>`: nombre del template usado por tooling.

## Reglas generales

* Un Document artifact explica.
* Un Document artifact responde una pregunta documental principal.
* Un Document artifact no compone artifacts como un Nexus.
* Un Document artifact no orienta recorridos como un Continuity Path.
* Un Document artifact no debe duplicar relaciones que pertenecen a otros artifacts.
* `metadata.relates` se usa para relaciones generales.
* `document.question` se usa para orientar el contenido, no para reemplazar el cuerpo.
* Los campos derivados no deben escribirse manualmente.
* No incluir `depth` ni `level` hasta que la profundidad documental esté mejor definida.

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
document.context.process.document-generation
```

La regla exacta debe vivir en tooling o en la especificación de identidad documental, no como campo manual obligatorio.
