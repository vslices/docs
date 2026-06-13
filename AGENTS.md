# VSlices Documentation Translation Instructions

## Project context

This repository contains the VSlices documentation.

VSlices is a progressive software engineering suite focused on preserving continuity between:

- domain discovery
- documentation
- design reasoning
- architecture
- implementation
- system evolution

The documentation is multilingual.

English source documents live under:

```text
docs/en/
````

Spanish translated documents live under:

```text
docs/es/
```

## Translation goal

Translate English documentation into Spanish using a 1:1 structural translation strategy.

The goal is not to rewrite, improve, summarize, reorganize, or reinterpret the documentation.

The goal is to create Spanish equivalents that preserve:

* the same document structure
* the same heading hierarchy
* the same conceptual intent
* the same Markdown formatting
* the same relative links
* the same code examples
* the same admonitions
* the same document boundaries

The Spanish version should be readable and natural, but structurally equivalent to the English version.

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

Use `__bold__` for bold text when editing existing bold text or adding translated bold text.

Do not convert list markers from `-` to `*`.

Do not reflow documents aggressively.

## Do not translate

Do not translate:

* code blocks
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
```

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
```

When needed, Spanish may explain the meaning of a retained English term, but do not rename VSlices concepts casually.

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

If the English document says that something is experimental, early, possible, current, near-term, or future, preserve that nuance.

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
