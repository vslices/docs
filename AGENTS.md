# VSlices Documentation Translation Instructions

## Project context

This repository contains the VSlices documentation.

VSlices is a progressive software engineering suite focused on preserving continuity between:

* domain discovery
* documentation
* design reasoning
* architecture
* implementation
* system evolution

The documentation is multilingual.

English source documents live under:

```text
docs/en/
```

Spanish translated documents live under:

```text
docs/es/
```

## Translation goal

Translate English documentation into Spanish using a 1:1 structural translation strategy.

The goal is not to rewrite, improve, summarize, reorganize, normalize, or reinterpret the documentation.

The goal is to create Spanish equivalents that preserve:

* the same document structure
* the same heading hierarchy
* the same order of ideas
* the same conceptual intent
* the same level of certainty or uncertainty
* the same Markdown formatting
* the same relative links
* the same code examples
* the same admonitions
* the same document boundaries
* the same historical meaning when translating decisions

The Spanish version should be readable and natural, but structurally equivalent to the English version.

If a translation sounds more elegant but changes the intent, keep the less elegant but more faithful version.

## File mapping rule

For every Markdown file under:

```text
docs/en/
```

create or update the equivalent file under:

```text
docs/es/
```

using the same relative path.

Example:

```text
docs/en/products/framework/index.md
docs/es/products/framework/index.md
```

Do not change file names.

Do not change folder names.

Do not invent a different Spanish folder structure.

Do not skip files in the requested batch unless explicitly instructed.

## Markdown preservation rules

Preserve Markdown syntax.

Preserve heading levels.

Preserve list nesting.

Preserve tables.

Preserve admonitions.

Preserve front matter if present.

Preserve comments if present.

Preserve blank-line structure unless a small formatting fix is required for valid Markdown.

Use `-` for unordered lists.

Use `_italic_` for italic text when editing existing italic text or adding translated italic text.

Use `__bold__` for bold text when editing existing bold text or adding translated bold text.

Do not convert list markers from `-` to `*`.

Do not convert `_italic_` to `*italic*`.

Do not convert `__bold__` to `**bold**`.

Do not reflow documents aggressively.

Do not collapse sections into one-line summaries.

Do not merge paragraphs unless the source already does so.

If content appears collapsed because of a fetch or render artifact, treat it as a warning and inspect the local file before making structural changes.

## Headings and visible text

Translate headings into Spanish unless the heading is a product name, project name, file name, command, code identifier, or intentionally retained VSlices concept.

Translate visible table headers.

Translate visible table cell text unless it is a code identifier, file path, URL, command, package name, type name, or retained concept.

Translate visible prose inside blockquotes.

Translate visible prose inside prose-only `text` code blocks when the block is documentation text rather than code or terminal output.

Preserve code fence language markers such as:

````text
```csharp
```yaml
```text
````

Do not add custom code fence ids.

## Do not translate

Do not translate:

* code identifiers
* inline code identifiers
* file names
* folder names
* URLs
* package names
* class names
* method names
* function names
* type names
* CLI commands
* YAML keys
* Markdown anchor fragments
* product names
* project names

Keep these names unchanged:

* VSlices
* VSlices Framework
* VSlices Design
* VSlices Docs Standard
* VSlices Method
* Alive Lab
* Domus Orbis
* LanguageExt
* .NET
* MkDocs
* Read the Docs

## Retained VSlices terms

Keep these terms in English unless the source document clearly requires a Spanish explanation:

```text
Framework
Design
Docs Standard
Method
Feature
Flow
Slice
Trait
Domain Type
Expected Error
Alive Lab
Context-First
Problem-First
Slice-First
Understanding
Contextualizing
Planning
Building
```

When used as ordinary English terms inside Spanish prose, retained technical terms should normally be written in `_italic_`, unless they are product names, modality names, headings, inline code, URLs, file names, or table labels where italics would reduce readability.

Examples:

```text
_feature_
_slice_
_vertical slice_
_feedback_
_workflow_
_endpoint_
_tradeoff_
_tradeoffs_
_stack_
```

Do not casually rename VSlices concepts.

## Terminology

Use these preferred translations:

```text
software engineering -> ingeniería de software
domain discovery -> descubrimiento del dominio
documentation -> documentación
design reasoning -> razonamiento de diseño
architecture -> arquitectura
implementation -> implementación
system evolution -> evolución del sistema
accidental complexity -> complejidad accidental
architectural intent -> intención arquitectónica
living documentation -> documentación viva
bounded context -> contexto delimitado
use case -> caso de uso
capability -> capacidad
expected error -> error esperado
invariant -> invariante
decision -> decisión
tradeoff -> tradeoff
validation -> validación
adoption -> adopción
lifecycle -> ciclo de vida
design pressure -> presión real de diseño
progressive complexity -> complejidad progresiva
progressive architecture -> arquitectura progresiva
low ceremony -> baja ceremonia
business intent -> intención de negocio
domain understanding -> entendimiento del dominio
software artifact -> artefacto de software
implementation feedback -> feedback de implementación
business value -> valor de negocio
business context -> contexto de negocio
domain knowledge -> conocimiento de dominio
system boundary -> límite del sistema
```

Use natural Spanish while preserving the source intent.

Do not strengthen cautious wording.

Examples:

```text
may support -> puede apoyar
may help -> puede ayudar
does not make compliant by itself -> no vuelve conforme por sí mismo
may influence later -> puede influir más adelante
```

## Style

Use neutral technical Spanish.

Prefer clarity over elegance.

Avoid marketing language.

Avoid poetic rewrites.

Avoid regional slang.

Avoid adding enthusiasm that is not present in the original.

Do not add new claims.

Do not remove uncertainty.

Preserve cautious wording.

If the English document says that something is experimental, early, possible, current, near-term, future, optional, partial, or not guaranteed, preserve that nuance.

Do not convert guidance into a rule unless the English source does so.

Do not convert a possible future product direction into a promise.

## Links

Preserve relative links exactly unless they are broken because of the language folder structure.

Most links should remain unchanged.

Example:

```md
[What is VSlices?](start-here/what-is-vslices.md)
```

may become:

```md
[¿Qué es VSlices?](start-here/what-is-vslices.md)
```

The link text may be translated.

The link target should usually remain unchanged.

Do not add `/es/` to local relative links.

Do not convert relative links to absolute URLs.

Do not translate Markdown anchor fragments.

## Code blocks

Never translate code blocks unless the code block is clearly prose-only documentation text.

Do not translate:

```csharp
public sealed class Something
```

Do not translate:

```yaml
site_name: VSlices
plugins:
  - search
```

Do not translate terminal commands.

Do not translate file trees except comments or descriptions outside the path names.

For prose-only `text` blocks, translate the visible prose but preserve:

* the fence
* the language marker
* the structure
* arrows if used as diagrams
* concept names intentionally kept in English

Example:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

should usually remain unchanged because those are VSlices Design stage names.

## Tables

Preserve table structure.

Translate visible table headers and cell prose.

Do not add or remove rows unless the source changed.

Do not add columns unless explicitly instructed.

If a table contains multiple items inside one cell, prefer clean HTML lists when needed for valid Markdown:

```html
<ul><li>First item</li><li>Second item</li></ul>
```

Every `<ul>` must close with `</ul>`.

Every `<li>` must close with `</li>`.

Use `<br/>` only when it improves readability and a list would be too heavy.

If a table appears collapsed only because of a fetch or render artifact, inspect the local Markdown before editing.

## Related artifacts sections

When a section named `Related artifacts` or `Artefactos relacionados` exists and the batch requires table normalization, convert the list into a table.

The Spanish table should use:

```text
Artefacto | Relación
```

The English table should use:

```text
Artifact | Relationship
```

Use these Spanish link labels when applicable:

```md
[Documento de contexto](context-document.md)
[Documento de proceso](process-document.md)
[Documento de caso de uso](use-case-document.md)
[Documento de capacidad](capability-document.md)
[Vocabulario de dominio](domain-vocabulary.md)
[Registro de decisión](decision-record.md)
[Nota de validación](validation-note.md)
[Nota de soporte](support-note.md)
```

Use these English link labels when applicable:

```md
[Context Document](context-document.md)
[Process Document](process-document.md)
[Use Case Document](use-case-document.md)
[Capability Document](capability-document.md)
[Domain Vocabulary](domain-vocabulary.md)
[Decision Record](decision-record.md)
[Validation Note](validation-note.md)
[Support Note](support-note.md)
```

Do not invent related artifacts that are not present in the source section.

Preserve the relationship meaning.

Preserve the source order unless explicitly instructed otherwise.

## Standard affinity tables

When translating VSlices Docs Standard taxonomy documents, keep standard affinity sections lightweight.

If instructed to normalize these tables, separate standards and practices into two tables:

```text
Estándar | Afinidad | Soporta
Práctica | Afinidad | Soporta
```

Do not include columns such as:

```text
Alineación faltante
Faltante para una alineación más estricta
Missing for stricter alignment
No provee
```

Those limits belong in `compliance-support.md`, not in every specific document.

When both standards appear, order them as:

```text
ISO/IEC/IEEE 29148
ISO/IEC/IEEE 42010
```

When practices appear, order them as:

```text
arc42
C4 Model
4+1 Model
ADR
```

Do not invent standards or practices that are not present in the source.

Preserve the intent: affinity and support do not mean formal compliance.

## Decision records

When translating files under `docs/en/decisions/`, preserve the decision record as historical documentation.

Preserve:

* file names
* decision title meaning
* decision status meaning
* decision date if present
* context
* decision
* rationale
* consequences
* tradeoffs
* principles
* uncertainty
* historical sequence
* accepted limitations
* future considerations

Do not rewrite the decision to sound more current.

Do not normalize old decision history.

Do not add justification.

Do not remove uncertainty.

Do not make accepted decisions sound stronger than the English source.

Do not turn an exploratory decision into a final product promise.

Do not turn a temporary decision into a permanent principle.

Do not change decision status semantics.

Translate status labels only if the surrounding document style requires Spanish, but preserve the meaning exactly.

Examples:

```text
Accepted -> Aceptada
Proposed -> Propuesta
Superseded -> Superada
Rejected -> Rechazada
Deprecated -> Obsoleta
```

If status values are used as machine-readable metadata, preserve them exactly.

## Batch discipline

Translate only the requested batch.

Do not edit unrelated files.

Do not opportunistically improve nearby documents.

Do not apply formatting-only changes outside the requested scope unless required to keep the translated files valid.

Report any source issues separately instead of silently rewriting them.

## Validation

After translating a batch, run:

```bash
mkdocs build -f mkdocs.es.yml --strict
```

If the multilingual local config exists, also run:

```bash
mkdocs build -f mkdocs.yml --strict
```

Report:

* files translated
* files created
* files skipped
* build result
* warnings
* unresolved questions

Do not commit changes automatically unless explicitly asked.
