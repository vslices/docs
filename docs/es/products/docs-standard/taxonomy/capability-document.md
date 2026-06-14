# Documento de capacidad

> Puedes acceder a la [plantilla de documento de capacidad aquí](https://github.com/vslices/docs-standard/blob/main/templates/capability-document.md)

Un Documento de capacidad (_Capability Document_ en inglés) preserva una capacidad estable requerida por el negocio o el sistema.

Su propósito es describir qué debe ser posible sin decidir demasiado pronto cómo debe implementarse. Un Documento de capacidad responde:

> ¿Qué debe poder hacer este negocio o sistema?

Una capacidad no es una _feature_, _endpoint_, _screen_, _service_ o componente técnico. Es una habilidad que puede apoyar varios casos de uso, _workflows_, procesos o decisiones.

## Propósito

Un Documento de capacidad ayuda al equipo a preservar:

- __capacidades estables__: qué debe poder hacer el negocio o sistema.
- __valor de negocio__: por qué importa esta capacidad.
- __comportamiento soportado__: qué casos de uso o _workflows_ dependen de la capacidad.
- __delimitaciones__: qué incluye y qué excluye la capacidad.
- __reglas y contradicciones__: qué da forma o limita la capacidad.
- __resultados esperados__: qué permite esta capacidad.
- __independencia a implementación__: la capacidad puede entenderse antes de elegir una estructura de código.

El objetivo es identificar capacidades significativas sin convertirlas demasiado pronto en componentes técnicos.

## Cuándo usarlo

Usa un Documento de capacidad cuando una habilidad sea lo suficientemente estable como para guiar diseño o implementación. Es especialmente útil cuando:

- __varios casos de uso tienen la misma capacidad__: la capacidad aparece repetidamente en el comportamiento.
- __un proceso depende de una habilidad estable__: el proceso no puede funcionar sin esta capacidad.
- __la capacidad define un límite__: la propiedad, la responsabilidad o la arquitectura pueden surgir alrededor de ella.
- __el valor de negocio debe ser visible__: el equipo debe recordar por qué importa la capacidad.
- __no se ha implementado aún__: el equipo necesita claridad antes de elegir un diseño.
- __se espera evolución futura__: la capacidad puede crecer, dividirse o volverse más formal después.

## Cuándo no usarlo

Un Documento de capacidad puede ser innecesario cuando:

- __el comportamiento es aislado__: un Documento de caso de uso es suficiente.
- __la capacidad es reducida__: el equipo todavía no puede explicar qué debe ser posible.
- __parece desglose de componentes__: el documento se está usando para justificar arquitectura demasiado pronto.
- __solo es un nombre__: no hay una capacidad estable detrás.
- __el dominio es desconocido aún__: primero puede necesitarse un Documento de contexto, un Documento de proceso o una Nota de soporte.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una definición ligera de la capacidad.

```md
# Documento de capacidad

## Capability

¿Qué debe poder hacer el negocio o sistema?

## Why it matters

¿Qué valor proporciona esta capacidad?

## Supported behavior

¿Qué casos de uso, _workflows_ o procesos dependen de ella?

## Boundaries

¿Qué está incluido y qué está fuera?

## Rules or constraints

¿Qué da forma o limita esta capacidad?

## Related artifacts

¿Qué contexto, proceso, caso de uso, decisión o validación apoya esta capacidad?
```

## Versión ampliada

Usa la versión ampliada cuando la capacidad sea importante, reutilizada, riesgosa o probable de influir en la arquitectura.

```md
# Documento de capacidad

## Capability

## Purpose

## Business value

## Related scenario or work line

## Supported processes

## Supported workflows

## Supported use cases

## Boundaries

## Responsibilities

## Inputs

## Outputs

## Rules and constraints

## Expected outcomes

## Expected errors

## Dependencies

## Related decisions

## Validation notes

## Evolution notes
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar | Afinidad | Soporta |
| --- | --- | --- |
| ISO/IEC/IEEE<br/>42010 | Media / Alta | <ul><li>Intereses de arquitectura</li><li>Límites</li><li>Justificación</li><li>Relaciones entre capacidades y decisiones</li></ul> |
| ISO/IEC/IEEE<br/>29148 | Media | <ul><li>Requisitos relacionados con capacidades</li><li>Restricciones</li><li>Resultados esperados</li><li>Trazabilidad</li></ul> |

| Práctica | Afinidad | Soporta |
| --- | --- | --- |
| arc42 | Media / Alta | Razonamiento de:<ul><li>Bloques de construcción</li><li>Responsabilidades</li><li>Límites</li><li>Riesgos</li><li>Decisiones</li></ul> |
| C4 Model | Media | Conciencia de límites que puede influir más adelante<br/>en vistas de contenedores o componentes. |
| 4+1 Model | Media | Razonamiento arquitectónico orientado a vistas: <ul><li>Lógicas</li><li>Proceso</li></ul> |
| ADR | Media | Decisiones sobre implementación de capacidades: <ul><li>Forma</li><li>División</li><li>Propiedad</li><li>Dirección</li></ul> |

## Artefactos relacionados

Un Documento de capacidad puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                                               |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| [Documento de contexto](context-document.md)     | Explica el escenario o línea de trabajo donde importa la capacidad.                                    |
| [Documento de proceso](process-document.md)      | Muestra qué procesos requieren la capacidad.                                                           |
| [Documento de caso de uso](use-case-document.md) | Describe comportamientos habilitados por la capacidad.                                                 |
| [Vocabulario de dominio](domain-vocabulary.md)   | Preserva el lenguaje usado para nombrar y explicar la capacidad.                                       |
| [Registro de decisión](decision-record.md)       | Explica por qué la capacidad fue moldeada, dividida, fusionada o<br/>implementada de una forma específica. |
| [Nota de validación](validation-note.md)         | Captura evidencia de si la capacidad apoya necesidades reales.                                         |
| [Nota de soporte](support-note.md)               | Captura ideas tempranas de capacidad antes de que se vuelvan<br/>capacidades estables.                     |

## Errores comunes

Errores comunes incluyen:

- __confundir capacidad con _feature___: una _feature_ entrega un comportamiento concreto, mientras que una capacidad describe una habilidad estable.
- __confundir capacidad con componente__: el documento se convierte en arquitectura antes de que la necesidad del dominio sea clara.
- __nombrar demasiado pronto__: el equipo asigna nombres formales a habilidades que todavía son vagas.
- __hacerla demasiado amplia__: la capacidad se convierte en un contenedor para comportamiento no relacionado.
- __hacerla demasiado estrecha__: la capacidad solo repite un caso de uso.
- __ignorar límites__: los lectores no pueden distinguir qué incluye o excluye la capacidad.
- __olvidar el valor__: la capacidad existe, pero nadie recuerda por qué importa.

## Preguntas de ejemplo

Un Documento de capacidad debería ayudar a responder:

- ¿Qué debe poder hacer el negocio o el sistema?
- ¿Por qué importa esta capacidad?
- ¿Qué casos de uso, _workflows_ o procesos dependen de ella?
- ¿Qué incluye esta capacidad?
- ¿Qué queda fuera de esta capacidad?
- ¿Qué reglas, restricciones o resultados la moldean?
- ¿Podría esta capacidad convertirse en un límite?
- ¿Qué decisiones o validaciones dependen de esta capacidad?

## Continuidad

Un Documento de capacidad preserva continuidad entre las necesidades del dominio y la posible estructura de implementación.

```text
Escenario o línea de trabajo
-> Procesos y casos de uso
-> Capacidades estables
-> Decisiones y opciones de implementación
-> Validación y evolución
```

Cuando las capacidades se mantienen independientes de decisiones de implementación prematuras, el equipo puede razonar sobre qué debe proporcionar el sistema antes de decidir cómo debe estructurarse.
