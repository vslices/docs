# Front-matter base para Nexus artifacts

## Template

```yaml
---
artifact:
  kind: nexus
  type: <capability|service-consumption>
  scope: <%type-scopes%>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: []

composition:
  composes:
    - artifact: <artifact-id>
      role: <%type-composition-roles%>

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

> ¿Qué tipo de artifact es este, qué variante representa, sobre qué elemento aplica y en qué idioma está escrito?

No debe incluir información derivada que pueda calcularse por tooling, como `id`, `filename`, `path`, `slug` o título visible.

* `artifact.kind`: clase general del artifact dentro de VSlices Docs Standard. Para este grupo siempre debe ser `nexus`.
* `artifact.type`: variante específica del nexus. Para este grupo puede ser `capability` o `service-consumption`.
* `artifact.scope`: escala, naturaleza o contexto principal donde aplica el nexus. Su valor depende del tipo de nexus.
* `artifact.target`: elemento concreto que el nexus compone o ayuda a entender.
* `artifact.language`: idioma principal del artifact. Debe usar valores simples como `es` o `en`.

## `metadata`

Define el estado documental y las relaciones generales del artifact.

Esta sección responde:

> ¿En qué estado está este artifact y con qué otros artifacts se relaciona sin que esa relación forme parte directa de la composición?

No debe duplicar relaciones que pertenecen a `composition.composes`.

* `metadata.status`: estado actual del artifact dentro de su ciclo de vida documental.
* `metadata.relates`: lista de relaciones generales con otros artifacts, paths, documentos, notas o elementos relevantes.

### Valores permitidos para `metadata.status`

* `draft`: el artifact está incompleto, exploratorio o en construcción.
* `candidate`: el artifact está propuesto y puede usarse, pero aún no está consolidado como definitivo.
* `active`: el artifact está vigente y representa la versión actualmente recomendada.
* `deprecated`: el artifact sigue existiendo, pero ya no se recomienda para nuevos usos.
* `superseded`: el artifact fue reemplazado por otro artifact más nuevo o más correcto.

### Forma recomendada para `metadata.relates`

```yaml
metadata:
  relates:
    - relation: <relation-name>
      target: <artifact-id>
```

`metadata.relates` debe usarse para relaciones no compositivas, por ejemplo:

* `references`
* `referenced-by`
* `complements`
* `depends-on`
* `owned-by`
* `derived-from`
* `updates`
* `supersedes`
* `superseded-by`

## `composition`

Define los artifacts que componen el nexus.

Esta sección responde:

> ¿Qué artifacts explican juntos el elemento compuesto?

En un Nexus, esta sección es central. La composición vive principalmente en metadata para evitar duplicar contenido de los artifacts relacionados.

* `composition.composes`: lista de artifacts que forman parte de la explicación compuesta.
* `composition.composes[].artifact`: identificador del artifact compuesto.
* `composition.composes[].role`: rol que cumple ese artifact dentro de la composición.

Un Nexus puede partir incompleto.

No es obligatorio declarar todos los roles posibles desde el inicio.

### Regla de uso

`composition.composes` debe usarse solo para artifacts que forman parte de la explicación compuesta.

Si un artifact solo está relacionado, referenciado o asociado indirectamente, debe ir en `metadata.relates`.

## `tooling`

Define información mínima para que VSlices Tooling pueda validar, generar, migrar o actualizar el artifact.

Esta sección responde:

> ¿Con qué schema y template fue construido este artifact?

* `tooling.schema.version`: versión del schema de front-matter usado por este artifact.
* `tooling.template.name`: nombre del template usado para crear o mantener este artifact.
* `tooling.template.version`: versión del template usado.

## Placeholders

Los placeholders indican valores que deben resolverse según el tipo específico de Nexus.

* `<capability|service-consumption>`: conjunto permitido de tipos de nexus.
* `<%type-scopes%>`: scopes permitidos por el tipo específico de nexus.
* `<target-name>`: nombre estable del elemento compuesto.
* `<es|en>`: idiomas soportados inicialmente.
* `<draft|candidate|active|deprecated|superseded>`: estados documentales permitidos.
* `<artifact-id>`: identificador estable de otro artifact.
* `<%type-composition-roles%>`: roles de composición permitidos por el tipo específico de nexus.
* `<template-name>`: nombre del template usado por tooling.

## Reglas generales

* Un Nexus compone artifacts.
* Un Nexus no reemplaza los artifacts compuestos.
* Un Nexus no duplica contenido de los artifacts compuestos.
* Un Nexus no obliga a crear todos los artifacts listados por su tipo.
* Un Nexus puede partir con una composición mínima.
* `metadata.relates` no debe usarse para declarar composición.
* `composition.composes` no debe usarse para relaciones generales.
* Los campos derivados no deben escribirse manualmente.
* El front-matter debe facilitar tooling sin volver incómoda la autoría manual.

## Campos derivados

Estos campos no deberían escribirse manualmente en el front-matter base:

* `id`
* `slug`
* `filename`
* `path`
* `title`
* `display_name`
* `canonical_id`
* `last_modified`
* `line_count`

Deben ser calculados por tooling, derivados desde el archivo, el título, la ubicación física o la combinación de `artifact.kind`, `artifact.type`, `artifact.scope` y `artifact.target`.

## Identidad derivada sugerida

La identidad canónica puede derivarse con una regla como:

```text
<artifact.kind>.<artifact.type>.<artifact.scope>.<artifact.target>
```

Ejemplo:

```text
nexus.capability.capability.product-search
```

O, si decidimos omitir redundancia para ciertos tipos:

```text
nexus.capability.product-search
```

La regla exacta debe vivir en tooling o en la especificación de identidad documental, no como campo manual obligatorio.
