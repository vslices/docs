# Vocabulario de dominio

> Puedes acceder a la [plantilla de vocabulario de dominio aquí](https://github.com/vslices/docs-standard/blob/main/templates/domain-vocabulary.md)

Un Vocabulario de dominio (*Domain Vocabulary* en inglés) preserva el lenguaje usado dentro de un área de negocio, sistema, proceso o capacidad.

Su propósito es hacer explícitos los términos importantes para que descubrimiento, documentación, diseño, implementación y validación no deriven hacia significados distintos.

Un vocabulario no es un diccionario de cada palabra usada por el negocio. Es un conjunto curado de términos que importan para entender y construir el sistema.

## Propósito

Un Vocabulario de dominio ayuda al equipo a preservar:

* **lenguaje compartido**: términos usados por expertos de dominio, usuarios, analistas, ingenieros y partes interesadas.
* **significado**: qué significa un término en el contexto actual del dominio.
* **límites**: dónde un término es válido y dónde puede significar otra cosa.
* **ambigüedad**: términos que son usados de forma distinta por diferentes personas o áreas.
* **alineación con implementación**: nombres que pueden aparecer más adelante en casos de uso, capacidades, código, pruebas o documentación.

El objetivo no es forzar lenguaje demasiado pronto. Es hacer visible el lenguaje importante antes de que se convierta silenciosamente en comportamiento del sistema.

## Cuándo usarlo

Usa un Vocabulario de dominio cuando el lenguaje afecte el entendimiento, las decisiones o la implementación. Es especialmente útil cuando:

* **el dominio tiene términos recurrentes**: las personas siguen usando las mismas palabras durante descubrimiento o planificación.
* **los términos son ambiguos**: la misma palabra significa cosas distintas según el equipo, proceso, área o sistema.
* **los términos son críticos para el negocio**: una interpretación incorrecta podría cambiar comportamiento, reglas, alcance o arquitectura.
* **el equipo es nuevo en el dominio**: ingenieros o analistas necesitan una referencia estable para el lenguaje del dominio.
* **los nombres de implementación importan**: es probable que los términos aparezcan en código, pruebas, APIs, pantallas o documentación.
* **colaboran varias áreas**: diferentes roles necesitan significado compartido para evitar confusión accidental.

## Cuándo no usarlo

Un Vocabulario de dominio puede ser innecesario cuando:

* **el cambio es pequeño y aislado**: el trabajo no depende de términos nuevos o ambiguos.
* **los términos son genéricos**: documentarlos no reduciría confusión o riesgo.
* **el vocabulario se volvería exhaustivo**: el equipo intenta documentar cada palabra en lugar de los términos que importan.
* **el lenguaje todavía es demasiado inestable**: una Nota de soporte puede ser suficiente hasta que el término demuestre ser útil.

## Versión mínima

Usa la versión mínima cuando el equipo solo necesite una referencia compartida ligera.

```md
# Domain Vocabulary

## Terms

- __Term__: significado corto, ejemplo de uso, términos relacionados.
```

Ejemplo:

```md
- __Reservation__: retención temporal de un recurso antes de la confirmación. Términos relacionados: booking, availability.
- __Booking__: reserva confirmada que crea un compromiso con el cliente. Términos relacionados: reservation, cancellation.
```

## Versión ampliada

Usa la versión ampliada cuando los términos sean ambiguos, reutilizados, críticos para el negocio o probables de influir en la implementación.

```md
# Domain Vocabulary

## Terms

### Term name

- __Meaning__: qué significa el término en este contexto.
- __Used by__: personas, equipos, roles, sistemas o documentos que usan este término.
- __Examples__: situaciones donde el término aplica.
- __Counterexamples__: situaciones donde el término no aplica.
- __Aliases__: palabras alternativas usadas para el mismo concepto o uno similar.
- __Conflicting meanings__: significados usados en otros lugares que pueden causar confusión.
- __Related terms__: conceptos cercanos.
- __Implementation notes__: posibles implicancias de nombrado o modelado.
- __Status__: draft, active, superseded, or archived.
```

## Afinidad con estándares

Este documento puede apoyar la alineación con estándares y prácticas de documentación existentes. No vuelve la documentación conforme por sí mismo.

| Estándar | Afinidad     | Soporta                                                                                                                                                   |
| ------------------- | ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ISO/IEC/IEEE 29148  | Media        | <ul><li>Terminología de requisitos</li><li>Definiciones</li><li>Reducción de ambigüedad</li><li>Trazabilidad</li></ul>                                    |
| ISO/IEC/IEEE 42010  | Media        | <ul><li>Términos consistentes para partes interesadas</li><li>Intereses</li><li>Vistas</li><li>Decisiones</li><li>Descripciones de arquitectura</li></ul> |

| Práctica | Afinidad     | Soporta                                                                                                                                                   |
| ------------------- | ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| arc42               | Alta         | <ul><li>Glosario</li><li>Terminología</li><li>Alias</li><li>Ejemplos</li><li>Lenguaje compartido</li></ul>                                                |
| C4 Model            | Baja / Media | <ul><li>Consistencia de nombres para sistemas</li><li>Contenedores</li><li>Componentes</li><li>Límites</li></ul>                                          |
| 4+1 Model      | Baja / Media | <ul><li>Lenguaje compartido entre escenarios</li><li>Vistas de arquitectura</li></ul>                                                                     |
| ADR                 | Baja / Media | Elecciones de nombres que pueden influir en decisiones                                                                                  |## Artefactos relacionados

Un Vocabulario de dominio puede apoyar o ser apoyado por:

| Artefacto                                        | Relación                                                                                                    |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| [Documento de contexto](context-document.md)     | Explica dónde aparece el lenguaje.                                                                          |
| [Documento de proceso](process-document.md)      | Muestra cómo se usan los términos dentro de flujos de negocio.                                              |
| [Documento de caso de uso](use-case-document.md) | Depende de términos claros para definir comportamiento esperado.                                            |
| [Documento de capacidad](capability-document.md) | Puede reutilizar vocabulario para nombrar capacidades estables de<br/>negocio.                                  |
| [Registro de decisión](decision-record.md)       | Puede explicar por qué se eligió un término o interpretación.                                               |
| [Nota de soporte](support-note.md)               | Puede capturar términos tempranos, inciertos o disputados antes de<br/>que se vuelvan entradas del vocabulario. |

## Errores comunes

Errores comunes incluyen:

* **documentar cada palabra**: el vocabulario se convierte en ruido en lugar de una referencia útil.
* **forzar nombres finales demasiado pronto**: el equipo trata lenguaje inestable como si ya estuviera resuelto.
* **ignorar significados conflictivos**: el mismo término sigue causando confusión entre áreas.
* **reescribir lenguaje de negocio demasiado pronto**: los nombres de implementación reemplazan el lenguaje del dominio antes de que el equipo lo entienda.
* **olvidar ejemplos**: las definiciones quedan abstractas y difíciles de validar.
* **no actualizar términos**: significados antiguos permanecen activos después de que el negocio o sistema cambia.

## Preguntas de ejemplo

Un Vocabulario de dominio debería ayudar a responder:

* ¿Qué significa este término en este contexto?
* ¿Quién usa este término?
* ¿Este término se usa de forma distinta en otro lugar?
* ¿Qué ejemplos prueban el significado?
* ¿Qué no debería significar este término?
* ¿Qué términos están relacionados o se confunden fácilmente?
* ¿Podría este término influir en nombres de implementación o límites?

## Continuidad

Un Vocabulario de dominio preserva continuidad entre lenguaje de negocio y estructura del sistema.

```text
Lenguaje de dominio
-> Significado documentado
-> Casos de uso y procesos
-> Capacidades y decisiones
-> Nombres de implementación
-> Validación y evolución
```

Cuando el lenguaje permanece explícito, es menos probable que el sistema se aleje del dominio que representa.
