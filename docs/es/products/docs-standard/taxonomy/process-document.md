# Documento de proceso

> Puedes acceder a la [plantilla de documento de proceso aquí](https://github.com/vslices/docs-standard/blob/main/templates/process-document.md)

Un Documento de proceso (*Process Document* en inglés) preserva cómo opera una línea de trabajo.

Su propósito es hacer visibles responsabilidades, roles, reglas de coordinación, flujos de trabajo, traspasos y resultados lo suficiente como para apoyar mejores decisiones de diseño e implementación.

Un Documento de proceso responde: __¿Cómo lo hacemos? ¿Qué se hace?__

Un Documento de proceso no es un manual operacional completo. Describe el conocimiento del proceso que importa para entender, mejorar, automatizar o preservar cómo se realiza el trabajo.

## Propósito

Un Documento de proceso ayuda al equipo a preservar:

* **proceso de trabajo**: cómo se realiza una línea de trabajo en la práctica.
* **responsabilidades**: quién posee, ejecuta, aprueba, apoya o reacciona al trabajo.
* **roles y cargos**: qué cargos, equipos, áreas o sistemas participan.
* **reglas de coordinación**: cómo los participantes organizan el trabajo entre ellos.
* **flujos de trabajo**: secuencias concretas de pasos, decisiones, traspasos y participantes responsables.
* **excepciones**: caminos alternativos, fallas, retrabajo o casos inusuales.
* **fricción**: retrasos, ambigüedad, duplicación, trabajo manual o coordinación frágil.

El objetivo es entender cómo se organiza el trabajo antes de cambiarlo o automatizarlo.

## Cuándo usarlo

Usa un Documento de proceso cuando la forma en que se realiza el trabajo afecte el entendimiento, la planificación o la implementación.

Es especialmente útil cuando:

* **la línea de trabajo necesita claridad operacional**: el equipo necesita entender cómo se produce valor actualmente.
* **las responsabilidades son importantes**: roles, propiedad, aprobaciones o reacciones afectan el proceso.
* **la coordinación es frágil**: el trabajo depende de traspasos, tiempos, comunicación o acuerdos implícitos.
* **existen varios flujos de trabajo**: el proceso contiene múltiples caminos, variantes o casos operacionales.
* **las reglas moldean el proceso**: condiciones de negocio afectan qué puede ocurrir y quién debe actuar.
* **se está considerando automatización**: el *software* puede apoyar, reemplazar o modificar trabajo existente.
* **el comportamiento actual es inconsistente**: distintas personas describen el proceso de forma diferente.

## Cuándo no usarlo

Un Documento de proceso puede ser innecesario cuando:

* **el proceso es trivial**: la forma en que se realiza el trabajo no afecta decisiones de diseño.
* **el escenario todavía no está claro**: puede necesitarse primero un Documento de contexto o una Nota de soporte.
* **solo importa una interacción**: un Documento de caso de uso puede ser suficiente.
* **solo importa una secuencia de pasos**: una pequeña nota de flujo de trabajo puede ser suficiente.
* **el equipo está documentando cada detalle operacional**: el documento se vuelve un manual de procedimiento exhaustivo.
* **el proceso es demasiado inestable**: una Nota de soporte puede ser mejor hasta que el proceso de trabajo sea más claro.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una descripción ligera de cómo se realiza el trabajo.

```md
# Process Document

## Work process

¿Cómo se realiza esta línea de trabajo?

## Purpose

¿Por qué existe este proceso?

## Participants and responsibilities

¿Quién participa y de qué es responsable?

## Main workflow

- Paso 1.
- Paso 2.
- Paso 3.

## Outcome

¿Qué produce este proceso?

## Pain points or risks

¿Qué hace que este proceso sea frágil, lento, poco claro o riesgoso?
```

## Versión ampliada

Usa la versión ampliada cuando el proceso sea complejo, riesgoso, transversal o probable de guiar implementación.

```md
# Process Document

## Work process

## Purpose

## Scope

## Related scenario or work line

## Participants, roles, and responsibilities

## Preconditions

## Coordination rules

## Main workflow

## Alternative workflows

## Exceptions and rework

## Business rules

## Handoffs

## Inputs

## Outputs

## Systems or tools involved

## Pain points

## Risks

## Related artifacts
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar           | Afinidad | Soporta                                                                                                                           |
| ------------------ | -------- | --------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148 | Media    | <ul><li>Requisitos relacionados con procesos</li><li>Supuestos</li><li>Reglas de negocio</li><li>Entradas de validación</li></ul> |
| ISO/IEC/IEEE 42010 | Media    | <ul><li>Intereses</li><li>Relaciones</li><li>Restricciones de proceso que pueden moldear la arquitectura</li></ul>                |

| Práctica  | Afinidad     | Soporta                                                                                                                                                          |
| --------- | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| arc42     | Media / Alta | <ul><li>Comportamiento en tiempo de ejecución</li><li>Movimiento del proceso</li><li>Riesgos</li><li>Responsabilidades</li><li>Intereses operacionales</li></ul> |
| C4 Model  | Baja / Media | <ul><li>Conciencia de límites</li><li>Conciencia de interacciones</li></ul>                                                                                      |
| 4+1 Model | Media        | <ul><li>Razonamiento orientado a vistas de proceso</li><li>Soporte de escenarios</li></ul>                                                                       |
| ADR       | Baja / Media | <ul><li>Restricciones de proceso que pueden justificar decisiones</li></ul>                                                                                      |

## Artefactos relacionados

Un Documento de proceso puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                                                     |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| [Documento de contexto](context-document.md)     | Explica el escenario y la línea de trabajo donde existe el proceso.                                          |
| [Vocabulario de dominio](domain-vocabulary.md)   | Preserva términos usados dentro del proceso.                                                                 |
| [Documento de caso de uso](use-case-document.md) | Describe el significado, consecuencias y validaciones de<br/>comportamientos específicos.                        |
| [Documento de capacidad](capability-document.md) | Identifica capacidades estables requeridas para realizar o mejorar el<br/>proceso.                               |
| [Registro de decisión](decision-record.md)       | Explica elecciones tomadas debido a restricciones del proceso.                                               |
| [Nota de validación](validation-note.md)         | Captura lo aprendido después de cambiar o probar el proceso.                                                 |
| [Nota de soporte](support-note.md)               | Captura responsabilidades inciertas, variantes de flujo de trabajo,<br/>riesgos, supuestos o preguntas abiertas. |

## Errores comunes

Errores comunes incluyen:

* **confundir proceso con flujo de trabajo**: el documento solo lista pasos y omite responsabilidades o coordinación.
* **documentar cada detalle**: el proceso se vuelve demasiado grande para guiar decisiones.
* **escribir solo el camino feliz**: las excepciones y el retrabajo permanecen invisibles.
* **ignorar traspasos**: las partes más frágiles del proceso desaparecen.
* **mezclar comportamiento actual y objetivo**: los lectores no pueden distinguir qué existe hoy y qué se propone.
* **ocultar propiedad**: las responsabilidades permanecen implícitas.
* **saltar a automatización**: el equipo diseña *software* antes de entender el trabajo.
* **no actualizar después del cambio**: el proceso documentado ya no coincide con la realidad.

## Preguntas de ejemplo

Un Documento de proceso debería ayudar a responder:

* ¿Cómo se realiza esta línea de trabajo?
* ¿Por qué existe este proceso?
* ¿Quién participa y de qué es responsable?
* ¿Cómo coordinan el trabajo los participantes?
* ¿Qué flujos de trabajo existen dentro de este proceso?
* ¿Qué ocurre primero, después y al final?
* ¿Dónde se mueve el trabajo entre personas, áreas, sistemas o herramientas?
* ¿Qué hace que el proceso sea lento, frágil, riesgoso o poco claro?
* ¿Qué casos de uso, capacidades o decisiones dependen de este proceso?

## Continuidad

Un Documento de proceso preserva continuidad entre estructura operacional y comportamiento de *software*.

```text
Línea de trabajo
-> Proceso de trabajo
-> Responsabilidades y flujos de trabajo
-> Casos de uso y capacidades
-> Decisiones e implementación
-> Validación y evolución
```

Cuando el comportamiento del proceso permanece explícito, es menos probable que el equipo construya *software* que funciona técnicamente pero falla operacionalmente.
