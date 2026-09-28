# Relationships

## Propósito

La suite necesita distinguir la autoridad de una definición de las formas en que esa definición es utilizada o realizada.

Relaciones candidatas:

- `owned-by`
- `used-by`
- `implemented-by`
- `realized-by`
- `preserved-by`
- `rendered-by`
- `operationalized-by`
- `supported-by`
- `challenged-by`
- `derived-from`
- `supersedes`

Esta lista no es un schema estable.

## Regla central

```text
physical location
!= semantic authority

implementation
!= definition

automation
!= authority
```

## Ejemplo: Action Flow

```text
Action Flow
    owned-by -> VSlices Suite
    used-by -> Design
    used-by -> Method
    realized-by -> Docs Standard diagram notation
    operationalized-by -> Tooling (future candidate)
    related-to -> Framework realization (when justified)
```

## Ejemplo: Semantic Pressure

```text
Semantic Pressure
    owned-by -> VSlices Suite
    used-by -> Design
    used-by -> Method
    preserved-by -> Docs Standard
    operationalized-by -> Tooling (possible future)
```

## Continuity between organization and software

Una relación importante que debe seguir explorándose es la continuidad entre:

```text
Business Scenario
    -> organizational view of work

Software Project
    -> systematized view of work
```

El uso normal de VSlices debería preservar esta continuidad de forma proactiva.

`Traceability` cobra especial importancia cuando la relación necesita reconstruirse, verificarse o repararse de forma reactiva.

Esta interpretación permanece candidata y debería tensionarse contra los Continuity Paths existentes antes de cambiar su semántica canónica.
