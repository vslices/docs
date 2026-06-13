# Selección de modalidad

Selección de modalidad (_Modality Selection_ en ingles) explica cómo elegir una modalidad de _VSlices Design_ para la iteración actual.

El objetivo no es elegir la mejor modalidad en general. Es elegir la modalidad que ayuda al equipo a reducir la incertidumbre que actualmente amenaza la continuidad.

## Idea central

Elige la modalidad según la incertidumbre que más importa ahora. La pregunta no es:

```text
¿Qué modalidad preferimos?
```

La mejor pregunta es:

```text
¿Qué tipo de incertidumbre haría insegura la siguiente decisión?
```

_VSlices Method_ usa las modalidades definidas por _VSlices Design_:

* **Context-First**, cuando el equipo necesita un entendimiento más amplio antes de decidir qué construir.
* **Problem-First**, cuando existe un problema claro, pero sus causas, impacto o límites necesitan clarificación.
* **Slice-First**, cuando el equipo puede aprender más rápido construyendo una vertical slice pequeña y reversible.

Method no redefine estas modalidades. Ayuda a decidir cuál debería guiar el trabajo actual.

## Context-First

Usa Context-First cuando el equipo todavía no puede explicar el escenario de forma segura. Esto puede ocurrir cuando:

* el dominio es nuevo o se entiende poco
* el trabajo es mayormente manual o implícito
* varios actores interpretan el mismo proceso de formas distintas
* el lenguaje es inestable o ambiguo
* los límites del workflow no están claros
* el equipo todavía no sabe qué problema importa más

Context-First ayuda a evitar construir software alrededor de una realidad mal entendida.

El principal riesgo es el análisis sin movimiento. Usa Context-First solo hasta que el equipo tenga suficiente contexto para tomar una siguiente decisión más segura.

## Problem-First

Usa Problem-First cuando hay un problema visible, pero el equipo todavía no lo entiende lo suficiente como para resolverlo responsablemente. Esto puede ocurrir cuando:

* los usuarios reportan un dolor repetido
* un workflow tiene un cuello de botella conocido
* una feature existente no logra apoyar el trabajo real
* el impacto de negocio es visible, pero la causa no está clara
* se están proponiendo múltiples soluciones antes de entender el problema
* el problema puede cruzar varios workflows o responsabilidades

Problem-First ayuda a evitar resolver síntomas. El principal riesgo es la optimización local.

Usa Problem-First hasta que el equipo pueda explicar el problema, su contexto y la mejora esperada.

## Slice-First

Usa Slice-First cuando el equipo puede aprender de forma más segura construyendo una pequeña pieza de comportamiento. Esto puede ocurrir cuando:

* el contexto se entiende lo suficiente como para actuar
* el riesgo es acotado y reversible
* el equipo necesita feedback desde el uso real
* la implementación revelará restricciones útiles
* una vertical slice pequeña puede validar un supuesto
* más análisis no mejoraría significativamente la siguiente decisión

Slice-First ayuda a evitar diseñar demasiado antes de que la realidad pueda enseñar al equipo. El principal riesgo es la implementación sin entendimiento.

Usa Slice-First solo cuando la slice sea lo suficientemente pequeña para aprender de ella sin ocultar incertidumbre importante.

## Señales de selección

Una selección útil normalmente comienza nombrando la incertidumbre dominante.

| Señal actual                                                          | Comienza con      | Por qué                                                                                   |
| --------------------------------------------------------------------- | ----------------- | ----------------------------------------------------------------------------------------- |
| El equipo no entiende el contexto circundante.                        | **[Context-First](../../design/modalities/context-first/index.md)** | La siguiente decisión necesita un entendimiento más amplio antes de elegir qué construir. |
| El equipo entiende el área, pero no el problema.                      | **[Problem-First](../../design/modalities/problem-first/index.md)** | La siguiente decisión necesita claridad del problema antes de elegir una solución.        |
| El equipo entiende lo suficiente como para aprender mediante entrega. | **[Slice-First](../../design/modalities/slice-first/index.md)**   | La siguiente decisión puede hacerse más segura validando una _vertical slice_ pequeña.      |

La modalidad seleccionada debería reducir incertidumbre. No debería convertirse en la identidad de la iteración.

Un equipo puede comenzar con una modalidad y luego moverse a otra cuando el tipo de incertidumbre cambia.

## Errores comunes

La selección de modalidad puede fallar cuando el equipo elige según hábito en vez de incertidumbre.

* Elegir _Context-First_ para cada situación puede crear parálisis por análisis.
* Elegir _Problem-First_ demasiado pronto puede aislar un síntoma de su contexto.
* Elegir _Slice-First_ demasiado pronto puede producir implementación sin intención.
* Elegir repetidamente la misma modalidad puede ocultar que el contexto cambió.
* Elegir una modalidad como regla de proceso puede debilitar el juicio.

La modalidad es una guía de atención. No es un proceso fijo.

## Principio guía

Elige el menor énfasis de modalidad que haga más segura la siguiente decisión responsable.

* Si falta entendimiento, amplía el contexto.
* Si el problema no está claro, clarifica el problema.
* Si aprender requiere realidad, construye una slice pequeña.

La modalidad correcta es la que ayuda al equipo a preservar continuidad mientras avanza.
