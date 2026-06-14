# Documento de contexto

> Puedes acceder a la [plantilla de documento de contexto aquí](https://github.com/vslices/docs-standard/blob/main/templates/context-document.md)

Un Documento de contexto (*Context Document* en inglés) preserva el escenario donde está trabajando el equipo.

Su propósito es hacer visible el contexto de negocio, organizacional, operativo o del sistema lo suficiente como para apoyar mejores decisiones. Un Documento de contexto responde:

* ¿Dónde estamos trabajando?
* ¿Qué ofrece, opera o mantiene esta área?

Un Documento de contexto no es un mapa completo del negocio. Captura el contexto que importa para entender qué puede necesitar ser diseñado, mejorado, automatizado, integrado o preservado.

## Propósito

Un Documento de contexto ayuda al equipo a preservar:

* **escenario**: el contexto de negocio, organizacional, operativo o del sistema que se está observando.
* **líneas de trabajo**: las áreas, departamentos, servicios, líneas de negocio u ofertas dentro del escenario.
* **actores y áreas**: quién participa en el contexto.
* **situación actual**: cómo se comporta el escenario hoy a alto nivel.
* **puntos de dolor y oportunidades**: qué podría justificar trabajo futuro.
* **límites**: dónde comienza, termina o se vuelve poco claro el escenario.
* **incertidumbre**: supuestos, riesgos y preguntas abiertas que todavía necesitan atención.

El objetivo es crear suficiente entendimiento compartido para evitar diseñar desde requisitos aislados.

## Cuándo usarlo

Usa un Documento de contexto cuando el escenario circundante afecte el entendimiento, la planificación o la implementación. Es especialmente útil cuando:

* **el escenario no está claro**: el equipo todavía no entiende dónde ocurre el trabajo.
* **existen varias líneas de trabajo**: el área incluye varios departamentos, servicios u ofertas.
* **participan muchos actores**: las responsabilidades, la propiedad o la colaboración pueden importar.
* **la situación actual está fragmentada**: el trabajo ocurre a través de pasos manuales, herramientas, documentos o sistemas heredados.
* **el cambio puede afectar trabajo adyacente**: una mejora local podría impactar áreas o servicios cercanos.
* **el equipo necesita una base compartida**: documentos posteriores necesitan una referencia contextual estable.
* **el costo de malentender es alto**: construir desde un contexto débil podría crear complejidad accidental.

## Cuándo no usarlo

Un Documento de contexto puede ser innecesario cuando:

* **el cambio es pequeño y aislado**: el contexto circundante no afecta la decisión.
* **el escenario ya se entiende**: la documentación existente o el conocimiento del equipo es suficiente.
* **solo importa el proceso**: un Documento de proceso puede ser más útil.
* **solo importa el comportamiento**: un Documento de caso de uso puede ser suficiente.
* **el equipo necesita retroalimentación rápida**: una pequeña *slice* puede producir aprendizaje mejor y más seguro.
* **el documento se convertiría en un mapa completo del negocio**: el equipo intenta documentarlo todo en lugar del contexto relevante.
* **basta con una Nota de soporte**: el contexto sigue siendo temprano, pequeño o incierto.

## Versión mínima

Usa la versión mínima cuando el equipo necesite una base compartida ligera.

```md
# Documento de contexto

## Scenario

¿Dónde estamos trabajando?

## Why it matters

Por qué este scenario es relevante ahora.

## Scope

Qué está incluido y qué está intencionalmente fuera.

## Work lines

Qué áreas, departamentos, servicios u ofertas existen dentro de este scenario.

## Current situation

Cómo se comporta el scenario hoy a alto nivel.

## Actors and areas

¿Quién participa en este scenario?

## Pain points or opportunities

¿Qué podría justificar trabajo futuro?

## Open questions

¿Qué todavía necesita entenderse?
```

## Versión ampliada

Usa la versión ampliada cuando el scenario sea amplio, riesgoso, fragmentado o probable de guiar varios documentos futuros.

```md
# Documento de contexto

## Scenario

## Purpose

## Scope

## Out of scope

## Business background

## Work lines

## Actors, areas, and responsibilities

## Current situation

## Current systems or tools

## Pain points and opportunities

## Boundaries

## Relevant vocabulary

## Assumptions

## Risks

## Open questions

## Related artifacts
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar           | Afinidad | Soporta                                                                                                                                |
| ------------------ | -------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148 | Media    | <ul><li>Contexto para requisitos</li><li>Supuestos</li><li>Riesgos</li><li>Trazabilidad</li></ul>                                      |
| ISO/IEC/IEEE 42010 | Alta     | <ul><li>Contexto</li><li>Intereses</li><li>Stakeholders</li><li>Límites</li><li>Relaciones</li><li>Entradas de justificación</li></ul> |


| Práctica       | Afinidad     | Soporta                                                                                                                                |
| -------------- | ------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| arc42          | Alta         | <ul><li>Contexto y alcance</li><li>Interfaces externas</li><li>Restricciones</li><li>Riesgos</li><li>Conexiones con glosario</li></ul> |
| C4 Model       | Alta         | <ul><li>Razonamiento de contexto de sistema</li><li>Actores</li><li>Sistemas</li><li>Conciencia de límites</li></ul>                   |
| 4+1 Model | Media        | <ul><li>Fundamento de escenarios</li><li>Contexto para vistas posteriores</li></ul>                                                    |
| ADR            | Baja / Media | <ul><li>Contexto para decisiones</li><li>*Tradeoffs*</li></ul>                                                                         |## Artefactos relacionados

Un Documento de contexto puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                                   |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| [Vocabulario de dominio](domain-vocabulary.md)   | Preserva términos importantes descubiertos dentro del escenario.                           |
| [Documento de proceso](process-document.md)      | Describe cómo operan las líneas de trabajo mediante responsabilidades<br/>y flujos de trabajo. |
| [Documento de caso de uso](use-case-document.md) | Define el comportamiento esperado respaldado por el escenario.                             |
| [Documento de capacidad](capability-document.md) | Identifica capacidades estables necesarias dentro del escenario o línea<br/>de trabajo.        |
| [Registro de decisión](decision-record.md)       | Explica decisiones tomadas por restricciones contextuales.                                 |
| [Nota de validación](validation-note.md)         | Captura aprendizaje que cambia o confirma el escenario.                                    |
| [Nota de soporte](support-note.md)               | Captura hallazgos tempranos antes de que formen parte del contexto.                        |


## Errores comunes

Errores comunes incluyen:

* **documentar todo el negocio**: el documento se vuelve demasiado amplio para guiar decisiones.
* **saltarse a soluciones**: el documento empieza a describir qué construir en lugar de dónde trabaja el equipo.
* **confundir escenario con proceso**: el documento sobreexplica cómo se realiza el trabajo.
* **confundir línea de trabajo con flujo de trabajo**: las áreas o servicios se describen como flujos paso a paso.
* **ignorar límites**: el equipo no puede decir dónde termina el escenario.
* **ocultar incertidumbre**: los supuestos y preguntas abiertas se escriben como hechos.
* **no actualizar después del aprendizaje**: la retroalimentación de implementación cambia el escenario, pero el documento permanece congelado.

## Preguntas de ejemplo

Un Documento de contexto debería ayudar a responder:

* ¿Dónde estamos trabajando?
* ¿Por qué importa este escenario ahora?
* ¿Qué líneas de trabajo existen dentro de este escenario?
* ¿Quién participa en este escenario?
* ¿Qué ocurre actualmente a alto nivel?
* ¿Qué puntos de dolor u oportunidades son visibles?
* ¿Qué límites son claros o poco claros?
* ¿Qué todavía no entendemos?
* ¿Qué documentos o decisiones dependen de este contexto?

## Continuidad

Un Documento de contexto preserva la continuidad entre la realidad de negocio descubierta y las decisiones de software posteriores.

```text
Escenario
-> Líneas de trabajo
-> Entendimiento compartido
-> Procesos y casos de uso
-> Capacidades y decisiones
-> Alcance de implementación
-> Validación y evolución
```

Cuando el contexto sigue visible, los artefactos posteriores tienen menos probabilidades de quedar aislados del escenario que los justificó.
