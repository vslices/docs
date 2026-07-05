# Prelude de Continuity Paths

## Propósito

Este documento introduce el concepto de **Continuity Paths** dentro de VSlices Docs Standard.

Su objetivo es preparar la lectura de la familia de caminos de continuidad sin entrar todavía en el detalle de cada path específico.

Los Continuity Paths existen para preservar continuidad cuando un concepto no vive en un solo documento, una sola decisión, una sola estructura o una sola superficie del sistema.

## Problema que resuelven

En proyectos de software, un mismo concepto puede aparecer en muchas partes:

* en una conversación de negocio
* en una decisión
* en un contexto de dominio
* en una feature
* en un producto visible
* en un servicio consumible
* en una estructura técnica
* en una validación
* en un cambio de alcance
* en documentación futura

Cuando esas conexiones no son visibles, el conocimiento se fragmenta.

El equipo puede saber qué se implementó, pero perder:

* por qué importaba
* dónde apareció originalmente
* qué significado tenía en el dominio
* qué decisión lo transformó
* qué alcance se redujo o postergó
* qué producto o servicio lo materializó
* qué efectos produjo
* quién lo valida o mantiene

Los Continuity Paths ayudan a que esas conexiones no dependan únicamente de memoria informal.

## Qué es un Continuity Path

Un **Continuity Path** es una estructura de navegación que conecta un concepto a través de una o más perspectivas de continuidad.

No es, por sí solo, un documento detallado.

Su responsabilidad principal es conectar.

Un Continuity Path puede apoyarse en:

* diagramas
* documentos
* referencias
* metadata
* notas de soporte
* decisiones
* feedback
* validaciones
* artifacts relacionados

Definición compacta:

> Un Continuity Path conecta un concepto a través de perspectivas relevantes para preservar continuidad.

## Qué no es un Continuity Path

Un Continuity Path no debería confundirse con:

* una explicación completa del concepto
* una matriz de trazabilidad obligatoria
* una arquitectura de carpetas
* un proceso de gestión de proyecto
* una lista exhaustiva de documentos requeridos
* una regla para documentar todo
* un grafo vivo obligatorio
* una auditoría formal

El path orienta el recorrido.

Los artifacts conectados preservan el detalle.

## Regla semántica base

VSlices Docs Standard separa responsabilidades:

* Los **documentos** explican.
* Los **continuity paths** conectan.
* Los **diagramas** muestran.
* Los **mockups** representan.
* La **organización documental** ordena.

Esta separación evita que un solo artifact intente hacerlo todo.

## Cómo se lee un Continuity Path

Un Continuity Path normalmente se lee como un mapa.

El mapa no reemplaza los lugares que conecta.

Ayuda a saber:

* por dónde empezar
* qué preguntas seguir
* qué artifacts revisar
* qué conceptos están documentados
* qué conceptos fueron identificados pero no necesitan documentación ahora
* qué conceptos podrían requerir documentación
* cuándo cambiar de perspectiva
* cuándo detener el recorrido

La metáfora útil es una ciudad:

* el path muestra rutas
* los documentos son lugares visitables
* los diagramas muestran relaciones
* la organización documental ordena barrios, colecciones o recorridos mayores

## Semántica visual recomendada

Los diagramas de Continuity Paths pueden usar una semántica visual simple:

| Forma       | Significado                                           |
| ----------- | ----------------------------------------------------- |
| `[[texto]]` | Concepto documentado                                  |
| `[texto]`   | Pregunta orientadora u orientación definida           |
| `>texto]`   | Concepto identificado sin necesidad documental actual |
| `{{texto}}` | Concepto identificado con necesidad documental        |

Regla importante:

> `{{texto}}` no significa obligación inmediata de documentar.
> Significa que existe una posible necesidad documental que debe evaluarse.

## Tipos de relaciones

Los diagramas pueden usar relaciones con distinta intención:

| Relación | Significado                                        |
| -------- | -------------------------------------------------- |
| `-->`    | Camino principal o relación directa                |
| `-.->`   | Camino auxiliar, contextual, secundario u opcional |

La diferencia ayuda a evitar que todo parezca igual de importante.

## Core Continuity Paths

Los **Core Continuity Paths** observan un concepto desde perspectivas principales de continuidad.

| Path                | Pregunta central                                                                      |
| ------------------- | ------------------------------------------------------------------------------------- |
| Business Scenario   | ¿Dónde estoy trabajando?                                                              |
| Business Driver     | ¿Por qué importa intervenir?                                                          |
| Domain Context      | ¿Qué lenguaje, reglas y límites pertenecen a esta parte del negocio?                  |
| Viability           | ¿Es viable abordar esto bajo las condiciones actuales?                                |
| Evolution           | ¿Cómo cambia este elemento en el tiempo sin perder su intención?                      |
| Software Initiative | ¿Qué herramientas de software tengo o necesito para abordar esta parte del trabajo?   |
| Client Product      | ¿Qué puede hacer el usuario con este sistema y qué aprendimos sobre esa experiencia?  |
| Consumable Service  | ¿Qué puede consumir otro sistema o producto, y qué garantías debe recibir al hacerlo? |

## Supporting Continuity Paths

Los **Supporting Continuity Paths** observan preocupaciones transversales.

No reemplazan a los core paths.

Los complementan cuando la pregunta principal cambia hacia responsabilidad, impacto, trazabilidad o materialización técnica.

| Path             | Pregunta central                                          |
| ---------------- | --------------------------------------------------------- |
| Software Project | ¿Cómo vive este concepto dentro del proyecto de software? |
| Ownership        | ¿Quién lo entiende, decide, valida, mantiene u opera?     |
| Impact           | ¿Qué otros elementos se ven afectados?                    |
| Traceability     | ¿De dónde viene y dónde terminó materializándose?         |

## Cómo elegir un path

La elección del path depende de la pregunta que necesitamos responder.

| Pregunta actual                                                   | Path sugerido       |
| ----------------------------------------------------------------- | ------------------- |
| Necesitamos entender dónde ocurre el trabajo                      | Business Scenario   |
| Necesitamos entender por qué importa intervenir                   | Business Driver     |
| Necesitamos entender lenguaje, reglas o límites del dominio       | Domain Context      |
| Necesitamos saber si algo puede abordarse bajo condiciones reales | Viability           |
| Necesitamos entender cómo algo cambia sin perder intención        | Evolution           |
| Necesitamos entender qué esfuerzo de software aborda el trabajo   | Software Initiative |
| Necesitamos entender qué puede hacer un usuario                   | Client Product      |
| Necesitamos entender qué puede consumir otro sistema o producto   | Consumable Service  |
| Necesitamos entender cómo algo vive técnicamente                  | Software Project    |
| Necesitamos entender quién entiende, decide, valida o mantiene    | Ownership           |
| Necesitamos entender qué se ve afectado                           | Impact              |
| Necesitamos reconstruir origen y materialización                  | Traceability        |

## Relación con documentos

Un Continuity Path no obliga a crear documentos nuevos.

Puede conectar artifacts existentes o señalar necesidades documentales candidatas.

Por ejemplo:

* Business Driver puede conectar Context Document, Scope Document o Decision Record.
* Domain Context puede conectar Domain Vocabulary, Consistency Document o Behavior Document.
* Viability puede conectar Viability Document, Scope Document o Support Note kind: validation.
* Evolution puede conectar Update Document, Decision Record, Feedback Document o Scope Document.
* Client Product puede conectar Behavior Document, Feedback Document, mockups o decisiones de experiencia.
* Consumable Service puede conectar Structure Document, Behavior Document o Consistency Document.
* Software Project puede conectar Structure Document, Decision Record o artifacts técnicos.
* Traceability puede conectar origen, decisión, cambio y materialización.

La pregunta no es:

> ¿Qué documentos obliga este path a crear?

La pregunta correcta es:

> ¿Qué artifacts ayudan a preservar continuidad alrededor de este concepto?

## Relación con Viability

Viability es un path core porque una idea puede ser valiosa, deseable o técnicamente interesante y aun así no ser viable bajo las condiciones actuales.

El Documento de Viabilidad responde:

> ¿Es viable?

El `kind` define la dimensión evaluada:

* economic
* technical
* operational
* temporal
* organizational
* adoption

Esto permite evaluar viabilidad sin crear un documento distinto para cada dimensión.

## Relación con Evolution

Evolution es un path core porque los sistemas cambian.

El cambio puede venir de:

* feedback
* validación
* cambio de alcance
* nueva restricción
* aprendizaje
* decisión de producto
* decisión técnica
* reducción de alcance
* postergación
* exclusión
* reemplazo

Evolution no reemplaza al Update Document.

Evolution conecta la historia del cambio.

Update Document explica qué se actualizará.

## Relación entre Software Initiative y Software Project

Software Initiative y Software Project no son lo mismo.

**Software Initiative** es core.

Observa qué esfuerzo de software aborda una parte del trabajo, qué piezas necesita, qué productos o servicios puede involucrar y qué proyectos puede originar.

**Software Project** es support.

Observa cómo un concepto vive técnicamente dentro del proyecto de software: estructura, implementación, decisiones técnicas, dependencias, adapters y evolución del código.

Regla simple:

> Software Initiative mira el esfuerzo de software.
> Software Project mira la materialización técnica.

## Cuándo detenerse

Un Continuity Path debe ayudar a preservar continuidad, no a producir documentación infinita.

Conviene detener el recorrido cuando:

* la pregunta inicial ya fue respondida
* los artifacts relevantes ya están identificados
* no hay pérdida real de continuidad
* documentar más agregaría ceremonia
* el concepto solo necesitaba visibilidad
* una relación no aporta decisión, orientación ni aprendizaje

## Riesgos comunes

| Riesgo                                           | Consecuencia                                     |
| ------------------------------------------------ | ------------------------------------------------ |
| Usar paths como checklist obligatorio            | Se genera documentación prematura                |
| Intentar recorrer todos los paths siempre        | Se pierde foco                                   |
| Confundir path con documento detallado           | Se duplica contenido                             |
| Convertir cada nodo en artifact                  | Se infla la taxonomía                            |
| Confundir soporte con core                       | Se sobredimensionan preocupaciones transversales |
| Confundir diagramas con explicación completa     | Se pierde contexto                               |
| Confundir navegación con organización documental | Se mezclan responsabilidades                     |
| Documentar antes de observar necesidad real      | Se resuelve Iteración 5 en Iteración 1           |

## Estado de validación

Esta familia de Continuity Paths debe entenderse como candidata.

Fue definida a partir de observaciones de diseño documental, modelado de dominio, continuidad entre negocio y software, y necesidades detectadas durante la evolución de VSlices Docs Standard.

Todavía debe validarse mediante casos reales, uso aplicado y aprendizaje dentro de VSlices Research.

Hasta que exista evidencia suficiente, estos paths no deben tratarse como una taxonomía cerrada u obligatoria.

## Principio de continuidad

!!! principle "Principio de Continuidad"

```
Los Continuity Paths deberían ayudar a preservar conexiones relevantes entre intención, contexto, dominio, viabilidad, evolución, software, producto, servicio y evidencia sin convertir la documentación en una obligación exhaustiva.
```
