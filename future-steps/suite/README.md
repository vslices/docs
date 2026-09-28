# VSlices Suite — superficie provisional

## Estado

Superficie provisional de definición de suite.

Esta ruta existe como staging hasta disponer de un repositorio canónico `vslices/suite`.

Su objetivo es preservar conocimiento cuya autoridad pertenece a **VSlices como suite**, o conocimiento necesario para declarar de forma explícita qué producto posee una definición.

No es documentación pública ni un reemplazo de los repositorios de los productos.

## Responsabilidad

La superficie de suite puede:

- definir fundamentos compartidos;
- definir mecanismos que pertenecen a VSlices como conjunto;
- declarar responsabilidades y límites de autoridad entre productos;
- registrar relaciones entre definiciones de suite y realizaciones de producto;
- conservar el estado de madurez de conceptos transversales;
- orientar promoción desde investigación o evidencia hacia conocimiento canónico.

La superficie de suite no debe:

- absorber semántica cuyo ownership pertenece claramente a un producto;
- convertirse en una segunda fuente de verdad para definiciones ya canónicas;
- definir una implementación tecnológica sólo porque hoy sea la realización dominante;
- promover hipótesis a definición estable sin evidencia suficiente.

## Regla de autoridad

```text
Suite-owned semantics
    -> defined by VSlices

Product-specific semantics
    -> defined by the owning product

Research / uncertain ownership
    -> preserved as candidate evidence until authority becomes clear
```

Un producto puede implementar, especializar, documentar u operacionalizar un mecanismo de VSlices sin convertirse por ello en la autoridad que define el mecanismo.

## Estructura provisional

```text
suite/
├── foundations/
├── mechanisms/
├── products/
├── relationships/
└── promotion/
```

### Foundations

Conceptos compartidos necesarios para que los productos puedan hablar el mismo lenguaje sin redefinirlo independientemente.

### Mechanisms

Mecanismos que VSlices ofrece como suite y que luego pueden ser usados o realizados por uno o más productos.

Candidatos iniciales:

- [Action Flow](mechanisms/action-flow.md)
- [Semantic Pressure](mechanisms/semantic-pressure.md)

### Products

Responsabilidades de Design, Method, Docs Standard, Framework, Tooling y otras superficies.

La suite declara el límite entre responsabilidades; cada producto conserva autoridad sobre su propia semántica interna.

### Relationships

Relaciones entre conceptos, mecanismos, productos, realizaciones y evidencia.

### Promotion

Cómo una observación o hipótesis puede llegar a definición canónica sin confundir evidencia, historia y autoridad.

## Relación con documentación pública

La documentación pública debe ser una proyección deliberada de conocimiento ya organizado.

```text
suite / product definitions
        ↓
public projection
        ↓
vslices/docs
        ↓
MkDocs / Read the Docs
```

La estructura pública no necesita reflejar físicamente la estructura interna de autoridad.

## Próximo traslado

Cuando exista `vslices/suite`, esta superficie debería migrarse como bootstrap inicial del repositorio, preservando historia y estados candidatos.
