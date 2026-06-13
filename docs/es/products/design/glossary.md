# Glosario de VSlices Design

Este glosario define términos usados por VSlices Design.

VSlices Design se enfoca en razonamiento, modelado, incertidumbre, límites y entendimiento progresivo antes de comprometerse demasiado pronto con la arquitectura o la implementación.

Estos términos ayudan a describir cómo el trabajo de diseño puede comenzar desde distintos tipos de conocimiento disponible.

## Conceptos de diseño

- __Design modality__: una forma de abordar el trabajo de diseño según la incertidumbre actual, el conocimiento disponible y el siguiente paso más seguro.

- __Context-First__: una modalidad de diseño que comienza entendiendo el contexto de negocio, operativo, organizacional o del sistema que rodea el problema antes de acotar una solución o implementación específica.

- __Problem-First__: una modalidad de diseño que parte de una tensión, necesidad, riesgo, pregunta o fallo concreto que debe entenderse antes de decidir qué construir.

- __Slice-First__: una modalidad de diseño que parte de una pequeña slice útil de trabajo para aprender de la implementación, la validación o el uso real.

## Conceptos de apoyo

- __Modeling heuristic__: una ayuda práctica de razonamiento usada para hacer más fácil observar y discutir el conocimiento del dominio, la incertidumbre, las responsabilidades o los límites.

- __Design reasoning__: el proceso de entender por qué una estructura, límite, comportamiento, documento o dirección de implementación puede ser apropiada para el contexto actual.

- __Uncertainty__: una falta de entendimiento fiable sobre el dominio, el problema, el comportamiento, la responsabilidad, el riesgo o el resultado esperado.

- __Boundary reasoning__: el acto de usar los límites como objetos de razonamiento para identificar dónde conceptos, responsabilidades, decisiones, sistemas, actores o áreas de propiedad deberían separarse.

- __Progressive understanding__: la mejora gradual del conocimiento del dominio y del sistema mediante descubrimiento, documentación, modelado, implementación, validación y feedback.

## Relación entre las modalidades de diseño

Las modalidades de diseño describen distintos puntos de partida para el trabajo de diseño.

```text
Context-First
-> start from the surrounding situation

Problem-First
-> start from a concrete tension or need

Slice-First
-> start from a small useful implementation or validation slice
```

No son niveles de madurez ni una secuencia fija.

Un equipo puede comenzar con Context-First cuando el entorno no está claro, con Problem-First cuando una tensión específica es visible, o con Slice-First cuando construir una pequeña pieza es la forma más segura de aprender.

La parte importante es elegir la modalidad que encaja con la incertidumbre del trabajo actual.
