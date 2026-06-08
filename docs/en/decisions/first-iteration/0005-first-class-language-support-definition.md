# First Class Language Support Definition

## Status

Accepted.

## Context

VSlices documentation is evolving toward its first public v0.1.

Until now, the documentation has been primarily written in English to support international reach. However, VSlices is also born from a Spanish-speaking context, and some readers may be blocked from understanding the project if English is the only available entry point.

This creates a product and documentation concern:

* VSlices aims to teach engineering concepts, not hide them behind language barriers.
* Spanish should not be treated as an afterthought.
* Multilingual documentation should not add excessive maintenance burden during v0.1.
* Documentation structure should preserve continuity across languages.
* Read the Docs already provides native translation project support.
* MkDocs can be configured per language through dedicated configuration files.
* Read the Docs project variables can be used to select the correct MkDocs configuration per project.

The goal is to define Spanish as a first-class documentation language from the beginning.

## Decision

VSlices will support documentation in English and Spanish as first-class languages.

English will remain the default international documentation language for now.

Spanish will be maintained as an official documentation language, not as a secondary or informal translation.

The documentation repository will use folder-based language organization:

```text
docs/
  en/
    index.md
    start-here/
    products/

  es/
    index.md
    start-here/
    products/
```

Each language may have its own ReadTheDocs and MkDocs configuration:

```text
mkdocs.en.yml
mkdocs.es.yml
```

Read the Docs will use native translation projects:

```text
vslices      -> English
vslices-es   -> Spanish translation project
```

Both Read the Docs projects may point to the same repository.

The active MkDocs configuration will be selected through a specific `.readthedocs.yaml`. Local development may use three configurations:

```text
es/.readthedocs.yaml -> spanish docs
.readthedocs.yaml    -> english docs

mkdocs.local.yml -> multilingual local preview
mkdocs.en.yml    -> English-only preview
mkdocs.ess.yml   -> Spanish-only preview
```

## Rationale

Using folder-based language organization gives each language its own documentation space. This is preferred over suffix-based files such as:

```text
index.md
index.es.md
```

Because VSlices documentation is not only API reference material. It contains:

* philosophy
* product definitions
* design reasoning
* method documentation
* glossary terms
* decisions
* examples
* educational explanations

Spanish documentation may preserve the same intent as English documentation without always being a literal sentence-by-sentence translation.

The desired rule is:

```text
Same conceptual structure.
Equivalent intent.
Not necessarily literal translation.
```

This supports a healthier multilingual model. English and Spanish documents should usually share the same relative path:

```text
docs/en/products/framework/index.md
docs/es/products/framework/index.md
```

This preserves traceability between languages while allowing each language to express ideas naturally.

## Consequences

This decision allows VSlices to:

* provide Spanish-speaking readers with a real entry point
* preserve international accessibility through English
* avoid duplicating repositories
* keep Read the Docs native language support
* maintain language-specific navigation
* configure each language build explicitly
* and evolve translations progressively

This decision also introduces maintenance responsibilities:

* translated pages may drift from their English equivalents
* navigation may need to be updated per language
* new documents may require translation planning
* and each language build must be validated independently

These tradeoffs are accepted.

## Principle

Language support is part of documentation accessibility.

VSlices should not only preserve architectural continuity.

It should also preserve conceptual access for the people trying to learn, evaluate, and use it.
