# Front-matter base para Continuity Path artifacts

## Template

```yaml
---
artifact:
  kind: continuity-path
  type: <business-scenario|business-driver|domain-context|viability|evolution|software-initiative|client-product|consumable-service|software-project|ownership|impact|traceability|knowledge-handoff>
  scope: <%type-scopes%>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: []

continuity:
  question: <main-continuity-question>
  preserves: <%type-continuity-focus%>
  connects:
    - artifact: <artifact-id>
      role: <%type-connection-roles%>

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

Define la identidad documental del continuity path.

Esta sección responde:

> ¿Qué tipo de continuity path es este, sobre qué elemento aplica y en qué idioma está escrito?

* `artifact.kind`: clase general del artifact. Para este grupo siempre debe ser `continuity-path`.
* `artifact.type`: tipo específico del continuity path.
* `artifact.scope`: escala, naturaleza o contexto principal donde aplica el path. Su valor depende del tipo específico.
* `artifact.target`: elemento, situación, trayectoria o foco concreto cuya continuidad se quiere seguir.
* `artifact.language`: idioma principal del artifact. Debe usar valores simples como `es` o `en`.

## `metadata`

Define el estado documental y las relaciones generales del artifact.

Esta sección responde:

> ¿En qué estado está este path y con qué otros artifacts se relaciona de forma general?

* `metadata.status`: estado actual del artifact dentro de su ciclo de vida documental.
* `metadata.relates`: lista de relaciones generales con otros artifacts, paths, documentos, notas o elementos relevantes.

## `continuity`

Define la orientación de continuidad propia del path.

Esta sección responde:

> ¿Qué continuidad preserva este path y qué artifacts o paths conecta para sostenerla?

* `continuity.question`: pregunta principal que orienta el recorrido.
* `continuity.preserves`: tipo de continuidad que el path intenta preservar.
* `continuity.connects`: lista de artifacts o paths conectados por el recorrido.
* `continuity.connects[].artifact`: identificador del artifact o path conectado.
* `continuity.connects[].role`: rol que cumple ese artifact o path dentro del recorrido.

## `tooling`

Define información mínima para que VSlices Tooling pueda validar, generar, migrar o actualizar el artifact.

* `tooling.schema.version`: versión del schema de front-matter usado por este artifact.
* `tooling.template.name`: nombre del template usado para crear o mantener este artifact.
* `tooling.template.version`: versión del template usado.

## Placeholders

* `<%type-scopes%>`: scopes permitidos por el tipo específico de continuity path.
* `<target-name>`: nombre estable del elemento seguido por el path.
* `<main-continuity-question>`: pregunta principal del path.
* `<%type-continuity-focus%>`: foco de continuidad preservado por el path.
* `<%type-connection-roles%>`: roles permitidos para artifacts o paths conectados.
* `<template-name>`: nombre del template usado por tooling.

## Reglas generales

* Un Continuity Path orienta continuidad.
* Un Continuity Path puede conectar otros paths.
* Un Continuity Path no es un Nexus.
* Un Continuity Path no compone artifacts como un Nexus.
* Un Continuity Path no reemplaza los documentos que conecta.
* Un Continuity Path no obliga a crear todos los artifacts mencionados.
* Un Continuity Path puede usarse parcialmente.
* `metadata.relates` se usa para relaciones generales.
* `continuity.connects` se usa para artifacts o paths que participan directamente en el recorrido.
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
continuity-path.impact.change.pricing-update
```

La regla exacta debe vivir en tooling o en la especificación de identidad documental, no como campo manual obligatorio.
