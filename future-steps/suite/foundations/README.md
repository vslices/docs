# Foundations

## Estado

Candidatos de fundación compartida para VSlices.

Estas definiciones se mantienen pequeñas. Su propósito es evitar que cada producto reconstruya de forma independiente conceptos necesarios para comunicarse con el resto de la suite.

## Domain

`Domain` es el ámbito de realidad, conocimiento o actividad acerca del cual una responsabilidad necesita comprender, representar, apoyar o actuar.

No es una capa arquitectónica ni equivale a un namespace histórico.

## Domain Knowledge

`Domain Knowledge` es el conocimiento que un actor o sistema posee, adquiere, infiere o preserva acerca de un dominio.

## Domain Model

`Domain Model` es una representación selectiva y estructurada de Domain Knowledge construida para un propósito.

```text
Domain
    -> knowledge about it

Domain Knowledge
    -> selective formalization

Domain Model
```

Un Domain Model no pretende agotar el dominio.

## Otros fundamentos candidatos

El inventario inicial a validar incluye:

- Semantics;
- Semantic Authority;
- Evidence;
- Continuity;
- Transformation;
- Realization;
- Materialization;
- Representability;
- Admissibility;
- Unknown / Underdetermination.

Estos nombres no constituyen todavía una taxonomía cerrada.

## Regla de crecimiento

Un fundamento debería vivir aquí sólo cuando:

1. varios productos necesitan utilizarlo;
2. ningún producto específico debería poder redefinirlo unilateralmente;
3. su definición compartida reduce ambigüedad real;
4. existe suficiente evidencia para formular al menos un significado candidato estable.

Si una definición pertenece de forma clara a Design, Method, Docs Standard, Framework, Tooling u otro producto, la suite debería registrar la relación de ownership en vez de duplicar la definición.
