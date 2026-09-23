# VSlices Blog

El blog es la superficie editorial de VSlices.

Aquí viven historias, argumentos, experimentos, trayectorias de diseño y reflexiones técnicas que vale la pena contar como narrativa, sin convertirlas automáticamente en documentación canónica.

## Autores

- **Hernán Álvarez** — _The Semantic Feeler_
- **VSlices Development** — _The Semantic Bringer_

> We poke abstractions until they confess what they actually mean.

## Relación con otras superficies

El blog no reemplaza la documentación de producto ni el [Alive Lab](../alive-lab/index.md).

- La documentación canónica expresa cómo entendemos VSlices actualmente.
- Alive Lab preserva evidencia, investigación y aprendizaje en curso.
- El blog cuenta las historias, argumentos y trayectorias que ayudan a entender cómo llegamos hasta ciertas ideas.

Un artículo puede apoyarse en evidencia de Alive Lab, código, decisiones o documentación de producto sin convertirse por eso en una fuente canónica.

## Publicación

Los posts viven bajo:

```text
blog/posts/
```

y pueden declarar uno o más autores mediante front matter.

Ejemplo:

```yaml
---
date: 2026-09-23
authors:
  - hernan
  - development
categories:
  - VSlices Framework
  - Architecture
---
```

La política editorial detallada y el primer artículo se definirán antes del merge de esta rama.
