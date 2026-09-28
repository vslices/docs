# Product responsibilities

## Propósito

Esta superficie declara límites de responsabilidad entre productos desde la perspectiva de la suite.

No reemplaza la definición interna que cada producto hace de sí mismo.

## Independencia

Los productos deberían conservar valor independiente dentro de su responsabilidad.

VSlices Method es una excepción intencional en un sentido específico: su responsabilidad incluye componer y navegar capacidades de otros productos durante trabajo real.

Tooling no está subordinado a Method.

## Design

Define modalidades y herramientas de razonamiento para abordar problemas de ingeniería.

Ejemplos actuales:

- Context-First;
- Problem-First;
- Slice-First.

Design puede utilizar mecanismos suite-level como Action Flow o Semantic Pressure sin poseer su definición base.

## Method

Organiza cómo se navega trabajo real utilizando los productos y mecanismos que resulten útiles.

Puede:

- seleccionar o cambiar modalidad;
- decidir qué continuidad necesita prioridad;
- aplicar mecanismos como Semantic Pressure;
- decidir cuándo profundizar Action Flows;
- incorporar feedback hacia una nueva iteración.

## Docs Standard

Define cómo preservar, relacionar, componer y representar conocimiento documental.

Puede implementar documentalmente mecanismos suite-level sin apropiarse de su semántica base.

Ejemplos:

- Documents;
- Nexus;
- Continuity Paths;
- representaciones diagramáticas.

La autoridad suite-level de algunos mecanismos relacionados, como Continuity Path, debe revisarse explícitamente antes de cambiar ownership existente.

## Framework

Define cómo conocimiento suficientemente explícito puede representarse y materializarse como semántica ejecutable y realizaciones tecnológicas.

Superficies como Space, Work y Grounding pertenecen actualmente a Framework salvo evidencia que justifique promover alguna noción a nivel suite.

## Tooling

Hace operables, repetibles y verificables mecanismos soportados.

Puede apoyar:

- Docs Standard;
- Framework;
- otros productos o mecanismos cuando exista semántica suficientemente definida.

```text
Tooling owns mechanisms of operation.
It does not acquire semantic authority merely by automating them.
```

## Research / Alive Lab

Preserva observaciones, hipótesis, tensiones y evidencia antes de que una definición deba ser promovida.

```text
observation
-> candidate
-> repeated evidence
-> stabilization
-> promotion
```

La historia y evidencia no deben confundirse con la definición promovida.
