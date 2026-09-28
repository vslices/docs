# Action Flow

## Estado

`candidate`

## Ownership

`VSlices Suite`

## Propósito

Un **Action Flow** representa trabajo mediante acciones ordenadas, condiciones, consecuencias, participantes y relaciones relevantes entre acciones.

Su objetivo es permitir que el trabajo pueda elaborarse progresivamente desde una perspectiva organizacional hasta una perspectiva sistematizada sin confundir ambas.

## Proyecciones principales

### Abstract Action Flow

Representa el trabajo sin comprometerse con una realización concreta.

Puede mostrar:

- acciones;
- orden;
- condiciones;
- cardinalidad;
- consecuencias;
- actores o roles cuando sean semánticamente relevantes;
- handoffs;
- alternativas;
- repetición.

Su afinidad natural está con la comprensión organizacional del trabajo.

### Systematized Action Flow

Representa cómo el trabajo es realizado, o se propone realizar, mediante actores humanos y responsabilidades del sistema.

Puede distinguir carriles como:

```text
Human
  External User
  Internal User
  Reviewer

System
  View
  Product / BFF
  Service
  Worker
  Provider
```

Los carriles representan responsabilidad útil para la decisión actual; no implican automáticamente repositorios, procesos, deployments o proyectos separados.

## Espacio de elaboración

Action Flow se relaciona con esta jerarquía de trabajo:

```text
Scenario
  -> Work Line
      -> Work Process
          -> Work Flow
              -> Work Step
```

Existen dos recorridos naturales.

### Organización hacia concreción

```text
Work Line
-> Work Process
-> Work Flow
```

El recorrido puede detenerse en Flow porque continuar hacia Steps exige normalmente una realización más concreta e instructiva.

### Sistema hacia composición

```text
Work Step
-> Work Flow
-> Work Process
```

El recorrido puede detenerse en Process porque subir hacia Work Line requiere conocimiento organizacional que no debería inferirse sólo desde la realización del sistema.

## Matriz organizacional / sistematizada

```text
                    ORGANIZATION        SYSTEM
                  +----------------+----------------+
Line              | Work Line      |       -        |
Process           | Work Process   | Work Process   |
Flow              | Work Flow      | Work Flow      |
Step              |       -        | Work Step      |
                  +----------------+----------------+
```

La zona compartida Process / Flow permite preservar continuidad entre trabajo organizacional y realización del sistema sin tratarlos como equivalentes.

## Movimientos candidatos

Los siguientes nombres describen transformaciones útiles dentro de este espacio.

### Concretize

```text
Organization / Line
-> Organization / Process
```

Pregunta típica:

> Reconocemos estas líneas de trabajo. ¿Qué procesos las realizan, cómo comienzan y qué relaciones o dependencias tienen?

### Abstract

```text
Organization / Process
-> Organization / Line
```

Pregunta típica:

> Tenemos estos procesos, entradas y resultados. ¿Qué línea de trabajo coordinada revelan?

### Digitize

```text
Organization / Process
-> System / Process
```

Busca una realización sistematizada de un proceso organizacional.

### Materialize

```text
System / Flow
-> Organization / Flow
```

Busca reconocer qué trabajo organizacional está siendo materializado por una realización observada.

El nombre permanece candidato porque invierte el sentido en que `materialization` suele utilizarse en otros contextos de VSlices.

### Compose

```text
System / Flow
-> System / Process
```

Compone varias capacidades o acciones sistematizadas en una responsabilidad de proceso mayor.

### Segment

```text
System / Process
-> System / Flow
```

Divide una realización demasiado amplia para hacer visibles responsabilidades o acciones diferenciables.

## Esfuerzos compuestos

Un esfuerzo puede combinar varias transformaciones cuando convergen en un mismo objetivo.

Ejemplo:

```text
Organization / Processes
    -- Digitize --\
                   -> System / Process
System / Flows
    -- Compose ---/
```

Esto permite preguntar:

> La organización necesita este proceso y ya poseemos estas capacidades sistematizadas. ¿Cómo componemos una realización que acerque ambos puntos?

Un esfuerzo relacionado puede contener varias transformaciones con destino común.

Esfuerzos con destinos distintos deberían preservarse como esfuerzos independientes aunque compartan evidencia o material de origen.

## Relación con productos

### Design

Puede usar Action Flow para razonar sobre trabajo, responsabilidades, fronteras y realizaciones candidatas.

### Method

Puede decidir cuándo producir, profundizar o contrastar Action Flows durante el lifecycle.

### Docs Standard

Puede definir una realización documental y visual del mecanismo, incluyendo metadata, simbología, preservación y relaciones con artifacts.

### Tooling

Puede eventualmente apoyar authoring, validación, transformación, navegación o rendering.

### Framework

Puede relacionar Action Flows sistematizados con semántica ejecutable cuando exista continuidad justificable, sin asumir equivalencia automática entre Work Flow documental y runtime Flow.

## Límite

Action Flow no decide arquitectura por sí mismo.

Tampoco implica:

- una Feature por acción;
- un Service por carril;
- un deployment por responsabilidad;
- que organización y sistema deban tener la misma forma.

Su valor está en hacer visibles las transformaciones entre perspectivas.
