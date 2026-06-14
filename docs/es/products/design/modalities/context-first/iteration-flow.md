# Flujo de iteración en Context-First

_Context-First_ da más atención a Understanding y Contextualizing.

| Etapa           | Énfasis           | Objetivo                                                                             |
| --------------- | ----------------- | ------------------------------------------------------------------------------------ |
| Understanding   | Alto              | Descubrir suficiente conocimiento de dominio para entender el área<br/>de negocio.       |
| Contextualizing | Alto              | Construir un escenario base amplio de flujos actuales, actores,<br/>conceptos y límites. |
| Planning        | Medio             | Seleccionar la mejora más valiosa respaldada por la base contextual.                 |
| Building        | Medio<br/>(_posterior_) | Implementar la mejora sin perder trazabilidad hacia el contexto<br/>descubierto.         |

Las etapas tempranas son intencionalmente más fuertes porque _Context-First_ asume que un contexto débil crea decisiones de implementación inestables.

# Understanding en _Context-First_

## Objetivo

El objetivo de Understanding es excavar suficiente conocimiento de dominio para saber de qué está compuesta el área de negocio.

El equipo escucha a expertos de dominio, observa el trabajo existente, identifica vocabulario recurrente, descubre conceptos, detecta actores y captura supuestos.

Esta etapa se relaciona con la pirámide invertida: el equipo retira los granos de arena que cubren el área explorada, y retirar granos significa entenderlos.

Entonces, el equipo pregunta:

* ¿Qué conceptos aparecen repetidamente?
* ¿Quién participa en esta área de negocio?
* ¿Qué lenguaje usan los expertos de dominio?
* ¿Qué flujos ya existen?
* ¿Qué problemas son visibles?
* ¿Qué supuestos estamos haciendo?
* ¿Qué partes del dominio siguen siendo poco claras?
* ¿Qué conceptos parecen fundacionales?
* ¿Qué historias son repetidas por distintas personas?

El objetivo no es modelar todo el negocio. Es entender lo suficiente para continuar con mejores preguntas.

## Artefactos comunes de apoyo

* glosario
* notas de conceptos
* notas de entrevistas de dominio
* lista de actores
* lista de áreas o departamentos
* preguntas abiertas
* lista de supuestos
* bocetos tempranos de flujo
* notas de historias recurrentes

## Riesgo principal evitado

Diseñar artefactos de *software* antes de entender el mundo al que pertenecen.

# Contextualizing en _Context-First_

## Objetivo

El objetivo de Contextualizing es organizar el conocimiento descubierto en un escenario base amplio.

El equipo toma la arena extraída durante Understanding y empieza a colocarla en la pirámide de construcción. Esta etapa vuelve visible el contexto actual; puede describir:

* áreas o departamentos relevantes
* actores y responsabilidades
* flujos actuales
* sistemas actuales
* puntos de dolor actuales
* límites actuales
* conceptos importantes
* relaciones entre conceptos
* *handoffs* entre participantes
* flujos adyacentes

Contextualizing no define la solución final. Su propósito es hacer visible la situación actual lo suficiente para apoyar mejores decisiones. Entonces, el equipo pregunta:

* ¿Cuál es el escenario actual?
* ¿Cómo se mueve el trabajo hoy?
* ¿Qué áreas, actores, sistemas o participantes externos están involucrados?
* ¿Qué flujos rodean el objetivo?
* ¿Qué responsabilidades son explícitas?
* ¿Qué responsabilidades son implícitas?
* ¿Qué límites están empezando a aparecer?
* ¿Qué flujos adyacentes podrían verse afectados?
* ¿Qué debería preservarse como entendimiento compartido?

Una base contextual fuerte vuelve más seguras las decisiones posteriores. Sin suficiente base, los artefactos posteriores pueden parecer precisos, pero seguir siendo inestables.

## Artefactos comunes de apoyo

* notas del escenario actual
* bocetos de flujo
* diagramas de carriles
* mapa de responsabilidades
* mapa de contexto
* notas de relaciones entre conceptos
* lista de puntos de dolor
* notas de límites
* notas de áreas afectadas
* notas de procesos actuales

## Riesgo principal evitado

Tratar un problema, caso de uso o *feature* como algo aislado cuando en realidad pertenece a un contexto operacional más amplio.

# Planning en _Context-First_

## Objetivo

El objetivo de Planning es decidir qué mejora debería perseguirse desde la base contextual.

El equipo usa el contexto descubierto para evaluar qué debería cambiar, por qué debería cambiar y qué impacto puede tener ese cambio. Planning cambia la mentalidad:

> ¿Qué está pasando? -> ¿Qué debería mejorar?

En _Context-First_, Planning debería estar respaldado por suficiente entendimiento alrededor para evitar optimización local.

El equipo pregunta:

* ¿Qué problemas vale la pena resolver ahora?
* ¿Qué mejora crea valor de negocio significativo?
* ¿Qué mejora es factible en el contexto actual?
* ¿Qué flujos adyacentes podrían verse afectados?
* ¿Qué riesgos o mitigaciones existen?
* ¿Qué partes deberían quedar fuera de la iteración actual?
* ¿Cómo se vería el escenario mejorado?
* ¿Qué casos de uso, procesos, capacidades o servicios podrían necesitarse?
* ¿Qué supuestos todavía necesitan validación?

La mejora preferida no siempre es la más interesante técnicamente. Es la mejora que entrega valor de negocio significativo sin introducir complejidad desproporcionada.

## Artefactos comunes de apoyo

* propuesta de mejora
* notas del escenario objetivo
* notas de alcance
* notas de *tradeoff*
* notas de riesgo
* notas de decisión
* lista de flujos afectados
* bocetos de casos de uso
* bocetos de proceso objetivo
* notas de mitigación
* notas de fuera de alcance

## Riesgo principal evitado

Resolver el problema técnico más atractivo en vez del problema de negocio más relevante.

# Building en _Context-First_

## Objetivo

El objetivo de Building es implementar la mejora planificada preservando continuidad con el contexto descubierto. Building incluye desarrollo, integración, validación, entrega y *feedback*.

En esta etapa, los artefactos de diseño se vuelven decisiones de implementación. El equipo puede definir o implementar:

* *features*
* flujos
* capacidades
* tipos de dominio
* integraciones
* servicios
* errores esperados
* cambios de despliegue
* ajustes operacionales

En _Context-First_, Building debería permanecer conectado con la base construida en etapas anteriores.

Una *feature* no debería aparecer como una decisión de implementación aislada. Debería ser trazable hacia:

* concepto de negocio
* flujo
* responsabilidad
* punto de dolor
* mejora objetivo
* límite descubierto

Building también prueba el entendimiento acumulado hasta ahora. Cuando el equipo construye, descubre si las etapas anteriores fueron suficientemente claras, incompletas o incorrectas.

El resultado de Building produce valor de negocio, pero también produce nuevo conocimiento. Ese nuevo conocimiento se vuelve material para la siguiente iteración.

El equipo pregunta:

* ¿Qué necesita implementarse ahora?
* ¿Qué supuestos se están probando?
* ¿Qué artefactos de diseño están guiando la implementación?
* ¿Qué conceptos o flujos sostienen esta *feature*?
* ¿Qué nuevas restricciones aparecieron durante el desarrollo?
* ¿Qué cambió después de la entrega?
* ¿Qué aprendió el equipo?
* ¿Qué debería explorarse después?

## Artefactos comunes de apoyo

* notas de *feature*
* notas de implementación
* notas de validación
* notas de entrega
* notas de *feedback*
* notas de decisión técnica
* notas de restricciones descubiertas
* notas de siguiente iteración
* notas de trazabilidad
* notas de aprendizaje en producción

## Riesgo principal evitado

Tratar la implementación como el final del aprendizaje.
