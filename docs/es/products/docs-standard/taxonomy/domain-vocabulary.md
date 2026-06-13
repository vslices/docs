# Vocabulario de dominio

> Puedes acceder a la [plantilla de vocabulario de dominio aquí](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)

Un Vocabulario de dominio preserva el lenguaje usado dentro de un área de negocio, sistema, proceso o capacidad.

Su propósito es hacer explícitos los términos importantes para que el descubrimiento, la documentación, el diseño, la implementación y la validación no deriven hacia significados distintos.

Un vocabulario no es un diccionario de cada palabra usada por el negocio. Es un conjunto curado de términos que importan para entender y construir el sistema.

## Propósito

Un Vocabulario de dominio ayuda al equipo a preservar:

- __lenguaje compartido__: términos usados por expertos del dominio, usuarios, analistas, ingenieros y stakeholders.
- __significado__: qué significa un término en el contexto actual del dominio.
- __límites__: dónde es válido un término y dónde puede significar otra cosa.
- __ambigüedad__: términos usados de forma diferente por personas o áreas distintas.
- __alineación de implementación__: nombres que luego pueden aparecer en casos de uso, capacidades, código, pruebas o documentación.

El objetivo no es imponer el lenguaje demasiado pronto. Es hacer visible el lenguaje importante antes de que se convierta silenciosamente en comportamiento del sistema.

## Cuándo usarlo

Usa un Vocabulario de dominio cuando el lenguaje afecte el entendimiento, las decisiones o la implementación. Es especialmente útil cuando:

- __el dominio tiene términos recurrentes__: las personas siguen usando las mismas palabras durante el descubrimiento o la planificación.
- __los términos son ambiguos__: la misma palabra significa cosas distintas según el equipo, proceso, área o sistema.
- __los términos son críticos para el negocio__: una interpretación incorrecta podría cambiar el comportamiento, las reglas, el alcance o la arquitectura.
- __el equipo es nuevo en el dominio__: ingenieros o analistas necesitan una referencia estable para el lenguaje del dominio.
- __los nombres de implementación importan__: es probable que los términos aparezcan en código, pruebas, APIs, screens o documentación.
- __colaboran múltiples áreas__: distintos roles necesitan significado compartido para evitar confusión accidental.

## Cuándo no usarlo

Un Vocabulario de dominio puede ser innecesario cuando:

- __el cambio es pequeño y aislado__: el trabajo no depende de términos nuevos o ambiguos.
- __los términos son genéricos__: documentarlos no reduciría confusión ni riesgo.
- __el vocabulario se volvería exhaustivo__: el equipo intenta documentar cada palabra en lugar de los términos que importan.
- __el lenguaje sigue demasiado inestable__: una Nota de soporte puede ser suficiente hasta que el término demuestre ser útil.

## Versión mínima

Usa la versión mínima cuando el equipo solo necesita una referencia compartida ligera.

```md
# Vocabulario de dominio

## Términos

- __Term__: significado breve, ejemplo de uso, términos relacionados.
```

Ejemplo:

```md
- __Reservation__: retención temporal de un recurso antes de la confirmación. Términos relacionados: booking, availability.
- __Booking__: reserva confirmada que crea un compromiso con el cliente. Términos relacionados: reservation, cancellation.
```

## Versión ampliada

Usa la versión ampliada cuando los términos sean ambiguos, reutilizados, críticos para el negocio o probables de influir en la implementación.

```md
# Vocabulario de dominio

## Términos

### Nombre del término

- __Meaning__: qué significa el término en este contexto.
- __Used by__: personas, equipos, roles, sistemas o documentos que usan este término.
- __Examples__: situaciones en las que el término aplica.
- __Counterexamples__: situaciones en las que el término no aplica.
- __Aliases__: palabras alternativas usadas para el mismo concepto o uno similar.
- __Conflicting meanings__: significados usados en otros lugares que pueden causar confusión.
- __Related terms__: conceptos cercanos.
- __Implementation notes__: posibles implicaciones de nombrado o modelado.
- __Status__: draft, active, superseded o archived.
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Standard or practice | Affinity | Supports | Missing for stricter alignment |
| --- | --- | --- | --- |
| arc42 | High | Glossary, terminology, aliases, examples, and shared language. | Formal glossary governance and complete arc42 structure. |
| ISO/IEC/IEEE 29148 | Medium | Requirement terminology, definitions, ambiguity reduction, and traceability. | Formal requirements terminology controls and requirements management. |
| ISO/IEC/IEEE 42010 | Medium | Consistent terms for stakeholders, concerns, views, decisions, and architecture descriptions. | Formal architecture description language or controlled vocabulary model. |
| C4 Model | Low / Medium | Naming consistency for systems, containers, components, and boundaries. | Diagram model and structural hierarchy. |
| 4+1 View Model | Low / Medium | Shared language across scenarios and architecture views. | Complete architecture view model. |
| ADR | Low / Medium | Naming choices that may influence decisions. | Decision-specific rationale and governance. |

## Artefactos relacionados

Un Vocabulario de dominio puede apoyar o ser apoyado por:

- __Documento de contexto__: explica dónde aparece el lenguaje.
- __Documento de proceso__: muestra cómo se usan los términos dentro de los flujos de negocio.
- __Documento de caso de uso__: depende de términos claros para definir el comportamiento esperado.
- __Documento de capacidad__: puede reutilizar vocabulario para nombrar capacidades estables del negocio.
- __Registro de decisión__: puede explicar por qué se eligió un término o interpretación.
- __Nota de soporte__: puede capturar términos tempranos, inciertos o discutidos antes de que se conviertan en entradas del vocabulario.

## Errores comunes

Errores comunes incluyen:

- __documentar cada palabra__: el vocabulario se vuelve ruido en lugar de una referencia útil.
- __forzar nombres finales demasiado pronto__: el equipo trata como resuelto un lenguaje todavía inestable.
- __ignorar significados conflictivos__: el mismo término sigue causando confusión entre áreas.
- __reescribir demasiado pronto el lenguaje de negocio__: los nombres de implementación reemplazan al lenguaje del dominio antes de entenderlo.
- __olvidar ejemplos__: las definiciones quedan abstractas y son difíciles de validar.
- __no actualizar términos__: significados antiguos siguen activos después de que el negocio o el sistema cambia.

## Preguntas de ejemplo

Un Vocabulario de dominio debería ayudar a responder:

- ¿Qué significa este término en este contexto?
- ¿Quién usa este término?
- ¿Se usa este término de forma distinta en otro lugar?
- ¿Qué ejemplos prueban el significado?
- ¿Qué no debería significar este término?
- ¿Qué términos están relacionados o son fáciles de confundir?
- ¿Podría este término influir en nombres o límites de implementación?

## Continuidad

Un Vocabulario de dominio preserva continuidad entre el lenguaje del negocio y la estructura del sistema.

```text
domain language
-> documented meaning
-> use cases and processes
-> capabilities and decisions
-> implementation names
-> validation and evolution
```

Cuando el lenguaje permanece explícito, el sistema es menos propenso a alejarse del dominio que representa.
