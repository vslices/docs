# Selección de modalidad

La selección de modalidad explica cómo elegir una modalidad de VSlices Design para la iteración actual.

El objetivo no es elegir la mejor modalidad en general. Es elegir la modalidad que ayude al equipo a reducir la incertidumbre que actualmente amenaza la continuidad.

## Idea central

Elige la modalidad según la incertidumbre que más importa ahora.

La pregunta no es: _¿Qué modalidad preferimos?_

La pregunta es: _¿Qué tipo de incertidumbre haría insegura la siguiente decisión?_

VSlices Method usa las modalidades definidas por VSlices Design:

* __[Context-First](../../design/modalities/context-first/index.md)__, cuando el equipo necesita una comprensión más amplia antes de decidir qué construir.
* __[Problem-First](../../design/modalities/problem-first/index.md)__, cuando existe un problema claro, pero sus causas, impacto o límites necesitan aclararse.
* __[Slice-First](../../design/modalities/slice-first/index.md)__, cuando el equipo puede aprender más rápido construyendo una vertical slice pequeña y reversible.

Method no redefine estas modalidades. Ayuda a decidir cuál debería guiar el trabajo actual.

## Context-First

Usa Context-First cuando el equipo todavía no puede explicar el escenario con seguridad. Esto puede ocurrir cuando:

* el dominio es nuevo o está poco entendido
* el trabajo es principalmente manual o implícito
* varios actores interpretan el mismo proceso de forma diferente
* el lenguaje es inestable o ambiguo
* los límites del workflow no están claros
* el equipo todavía no sabe qué problema importa más

Context-First ayuda a evitar construir software alrededor de una realidad mal entendida.

El riesgo principal es análisis sin movimiento. Usa Context-First solo hasta que el equipo tenga suficiente contexto para tomar una siguiente decisión más segura.

## Problem-First

Usa Problem-First cuando existe un problema visible, pero el equipo todavía no lo entiende lo suficiente como para resolverlo responsablemente. Esto puede ocurrir cuando:

* los usuarios reportan un dolor repetido
* un workflow tiene un cuello de botella conocido
* una feature existente no apoya el trabajo real
* el impacto de negocio es visible, pero la causa no está clara
* se proponen múltiples soluciones antes de entender el problema
* el problema puede cruzar varios workflows o responsabilidades

Problem-First ayuda a evitar resolver síntomas. El riesgo principal es la optimización local.

Usa Problem-First hasta que el equipo pueda explicar el problema, su contexto y la mejora esperada.

## Slice-First

Usa Slice-First cuando el equipo puede aprender con más seguridad construyendo una pequeña pieza de comportamiento. Esto puede ocurrir cuando:

* el contexto se entiende lo suficiente como para actuar
* el riesgo es acotado y reversible
* el equipo necesita feedback desde uso real
* la implementación revelará restricciones útiles
* una vertical slice pequeña puede validar un supuesto
* más análisis no mejoraría de forma significativa la siguiente decisión

Slice-First ayuda a evitar diseñar demasiado antes de que la realidad pueda enseñar al equipo. El riesgo principal es implementación sin entendimiento.

Usa Slice-First solo cuando la slice es lo suficientemente pequeña como para aprender de ella sin ocultar incertidumbre importante.

## Señales de selección

Una selección útil normalmente empieza nombrando la incertidumbre dominante.

| Señal actual | Comenzar con | Por qué |
| --- | --- | --- |
| El equipo no entiende el contexto circundante. | __[Context-First](../../design/modalities/context-first/index.md)__ | La siguiente decisión necesita comprensión más amplia antes de elegir qué construir. |
| El equipo entiende el área, pero no el problema. | __[Problem-First](../../design/modalities/problem-first/index.md)__ | La siguiente decisión necesita claridad del problema antes de elegir una solución. |
| El equipo entiende lo suficiente para aprender mediante entrega. | __[Slice-First](../../design/modalities/slice-first/index.md)__ | La siguiente decisión puede volverse más segura validando una vertical slice pequeña. |

La modalidad seleccionada debería reducir incertidumbre. No debería convertirse en la identidad de la iteración.

Un equipo puede comenzar con una modalidad y luego pasar a otra cuando cambia el tipo de incertidumbre.

## Errores comunes

La selección de modalidad puede fallar cuando el equipo elige por hábito en vez de por incertidumbre.

* Elegir Context-First para toda situación puede crear parálisis por análisis.
* Elegir Problem-First demasiado temprano puede aislar un síntoma de su contexto.
* Elegir Slice-First demasiado temprano puede producir implementación sin intención.
* Elegir la misma modalidad repetidamente puede ocultar que el contexto cambió.
* Elegir una modalidad como regla de proceso puede debilitar el juicio.

La modalidad es una guía de atención. No es un proceso fijo.

## Principio guía

Elige el énfasis de modalidad más pequeño que vuelva más segura la siguiente decisión responsable.

- Si falta entendimiento, amplía el contexto.
- Si el problema no está claro, aclara el problema.
- Si aprender requiere realidad, construye una slice pequeña.

La modalidad correcta es la que ayuda al equipo a preservar continuidad mientras avanza.
