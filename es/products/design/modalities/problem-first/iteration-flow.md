# Énfasis de etapas en Problem-First

_Problem-First_ da más atención a Planning mientras mantiene suficiente Understanding y Contextualizing alrededor del problema.

| Etapa           | Énfasis      | Objetivo                                                                      |
| --------------- | ------------ | ----------------------------------------------------------------------------- |
| Understanding   | Medio        | Entender el problema y los conceptos de dominio directamente<br/>alrededor de él. |
| Contextualizing | Medio        | Ubicar el problema dentro de su flujo y responsabilidades<br/>circundantes.       |
| Planning        | Alto         | Definir la mejora más efectiva y hacer explícitos los riesgos.                |
| Building        | Medio / Alto | Implementar la mejora y validar si el problema realmente fue<br/>reducido.        |

_Problem-First_ no requiere la base más amplia posible.

Requiere una base suficientemente amplia para sostener la mejora seleccionada.

# Understanding en _Problem-First_

## Objetivo

El objetivo de Understanding es aclarar el problema antes de intentar resolverlo.

El equipo parte desde un punto de dolor, solicitud, falla, oportunidad o limitación conocida. Luego explora los conceptos de dominio directamente alrededor de ese problema.

Esta etapa se relaciona con la pirámide invertida, pero la excavación es enfocada: el equipo no intenta remover cada grano de arena alrededor del negocio. Está removiendo los granos que cubren el problema.

Entonces, el equipo pregunta:

* ¿Qué problema estamos intentando resolver?
* ¿Quién experimenta este problema?
* ¿Cuándo aparece el problema?
* ¿Qué lenguaje usan las personas para describirlo?
* ¿Qué conceptos están directamente involucrados?
* ¿Qué comportamiento actual produce o expone el problema?
* ¿Qué supuestos estamos haciendo sobre la causa?
* ¿Este problema es síntoma de algo más profundo?
* ¿Qué pasaría si no hiciéramos nada?

El objetivo no es modelar completamente el dominio. Es entender el problema con suficiente claridad para evitar resolver algo incorrecto.

## Artefactos comunes de apoyo

* declaración del problema
* notas de entrevistas de dominio
* glosario
* notas de conceptos
* lista de actores
* notas de evidencia del problema
* lista de supuestos
* preguntas abiertas
* bocetos tempranos de flujo

## Riesgo principal evitado

Resolver un problema vagamente entendido porque al principio parecía obvio.

# Contextualizing en _Problem-First_

## Objetivo

El objetivo de Contextualizing es ubicar el problema dentro de su contexto de negocio circundante.

El equipo organiza el conocimiento descubierto en un escenario base enfocado. Este escenario debería explicar dónde aparece el problema, quiénes son afectados, qué ocurre actualmente y qué flujos circundantes pueden importar. Después de eso, el equipo puede preguntar:

* ¿Dónde aparece el problema en el flujo actual?
* ¿Qué actores, áreas, sistemas o responsabilidades están involucrados?
* ¿Qué ocurre antes de que aparezca el problema?
* ¿Qué ocurre después de que aparece el problema?
* ¿Qué flujos adyacentes podrían verse afectados por un cambio?
* ¿Qué reglas, excepciones o dependencias dan forma al problema?
* ¿Qué partes del contexto son relevantes ahora?
* ¿Qué partes pueden permanecer fuera de la iteración actual?

Contextualizing en _Problem-First_ debería ser más estrecho que en Context-First. El equipo debería evitar expandir la investigación salvo que el contexto circundante cambie la decisión.

El objetivo no es entender todo, sino entender lo suficiente alrededor del problema.

## Artefactos comunes de apoyo

* notas del escenario actual
* boceto de flujo enfocado
* diagrama de carriles
* mapa de responsabilidades
* lista de puntos de dolor
* notas de áreas afectadas
* notas de relaciones entre conceptos
* notas de límites
* notas de comportamiento actual

## Riesgo principal evitado

Tratar el problema como algo aislado cuando en realidad es causado o restringido por flujos circundantes.

# Planning en _Problem-First_

## Objetivo

El objetivo de Planning es definir la mejora más efectiva para el problema.

Esta es la etapa más importante en _Problem-First_.

El equipo usa el contexto enfocado para decidir qué debería cambiar, por qué debería cambiar, cuánto debería cambiar y qué riesgos puede introducir el cambio. Planning cambia la mentalidad:

> ¿Cuál es el problema? -> ¿Qué mejora deberíamos hacer ahora?

El equipo pregunta:

* ¿Cuál es el problema real que estamos resolviendo?
* ¿Qué resultado probaría que el problema mejoró?
* ¿Qué mejora crea valor de negocio significativo?
* ¿Qué solución es factible en el contexto actual?
* ¿Qué opciones están disponibles?
* ¿Qué opción es más simple?
* ¿Qué opción crea menos complejidad accidental?
* ¿Qué flujos adyacentes podrían verse afectados?
* ¿Qué riesgos o mitigaciones existen?
* ¿Qué debería permanecer fuera de la iteración actual?
* ¿Qué supuestos todavía necesitan validación?
* ¿Qué modos de falla deberíamos esperar?
* ¿Qué *tradeoffs* estamos aceptando?

_Problem-First_ no debería saltar del problema a la solución demasiado rápido.

El problema puede estar claro, pero la solución todavía necesita juicio de diseño. La mejora preferida es la que reduce el problema de forma efectiva sin crear complejidad desproporcionada en otro lugar.

## Artefactos comunes de apoyo

* propuesta de mejora
* notas del escenario objetivo
* notas de alcance
* notas de *tradeoff*
* notas de riesgo
* notas de mitigación
* notas de decisión
* lista de flujos afectados
* bocetos de casos de uso
* bocetos de proceso objetivo
* notas de resultado esperado
* notas de fuera de alcance

## Riesgo principal evitado

Elegir la primera solución atractiva en vez de la mejora más apropiada.

## Foco de riesgo

Planning en _Problem-First_ debería identificar riesgos explícitamente.

Esto es importante porque la modalidad evita intencionalmente la exploración amplia del dominio. Por eso, el equipo debería hacer visibles:

* riesgos causados por contexto limitado
* riesgos causados por flujos adyacentes afectados
* riesgos causados por reglas de negocio implícitas
* riesgos causados por propiedad poco clara
* riesgos causados por restricciones técnicas
* riesgos causados por cambiar comportamiento de usuarios
* riesgos causados por resolver un síntoma en vez de una causa

El equipo no necesita eliminar todos los riesgos. Pero debería saber qué riesgos está aceptando antes de que Building empiece.

# Building en _Problem-First_

## Objetivo

El objetivo de Building es implementar la mejora seleccionada y validar si realmente reduce el problema. Building incluye desarrollo, integración, validación, entrega y *feedback*.

En esta etapa, la mejora planificada se vuelve real. El equipo puede definir o implementar:

* *features*
* flujos
* capacidades
* tipos de dominio
* integraciones
* servicios
* errores esperados
* cambios de despliegue
* ajustes operacionales

En _Problem-First_, Building debería permanecer conectado al problema original.

Una *feature* debería ser trazable hacia:

* la declaración del problema
* los actores afectados
* el flujo relevante
* la mejora seleccionada
* el resultado esperado
* los riesgos aceptados
* o el comportamiento objetivo

Building también prueba si el equipo entendió correctamente el problema.

Cuando el equipo construye, descubre si la mejora planificada fue suficientemente clara, demasiado estrecha, demasiado amplia, incompleta o incorrecta.

El resultado de Building produce valor de negocio, pero también produce nuevo conocimiento. Ese nuevo conocimiento se vuelve material para la siguiente iteración. Después de eso, el equipo pregunta:

* ¿Qué necesita implementarse ahora?
* ¿Qué problema reduce esta implementación?
* ¿Qué supuestos se están probando?
* ¿Qué riesgos aceptados necesitan atención?
* ¿Qué artefactos de diseño están guiando la implementación?
* ¿Qué comportamiento prueba que la mejora funcionó?
* ¿Qué nuevas restricciones aparecieron durante el desarrollo?
* ¿Qué cambió después de la entrega?
* ¿El problema realmente mejoró?
* ¿Qué debería explorarse después?

## Artefactos comunes de apoyo

* notas de *feature*
* notas de implementación
* notas de validación
* notas de entrega
* notas de *feedback*
* notas de decisión técnica
* notas de restricciones descubiertas
* notas de riesgos aceptados
* notas de validación de resultado
* notas de siguiente iteración

## Riesgo principal evitado

Entregar una solución técnicamente correcta sin validar si el problema mejoró.

## Foco de riesgo

Building en _Problem-First_ debería mantener visibles los riesgos durante la implementación.

Esto no significa ralentizar el desarrollo con ceremonia innecesaria. Significa asegurarse de que el equipo no olvide los riesgos aceptados durante Planning.

El equipo debería observar:

* desviación de la implementación respecto del problema original
* nueva complejidad introducida por la solución
* nuevos casos límite descubiertos durante el desarrollo
* conflictos con flujos adyacentes
* validación faltante del resultado esperado
* reglas ocultas que aparecen solo durante la implementación
* atajos técnicos que debilitan la mejora
* *feedback* que revela que el problema fue malentendido

Si Building revela que el problema fue malentendido, la iteración debería volver a Understanding.

Eso no es fracaso, es aprendizaje.
