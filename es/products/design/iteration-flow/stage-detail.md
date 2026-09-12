# Flujo de iteración de diseño

## 1. Understanding

Understanding es la etapa donde el equipo extrae conocimiento de dominio.

El equipo explora el contexto de negocio escuchando a expertos de dominio, observando trabajo existente, identificando vocabulario, descubriendo conceptos y detectando flujos relevantes.

Esta etapa se relaciona con la pirámide invertida, donde el negocio se trata como una superficie amplia de conocimiento de dominio. Para entender un objetivo específico, el equipo debe retirar los granos de arena que lo cubren. Retirar granos significa entenderlos.

El equipo pregunta:

* ¿Qué conceptos aparecen repetidamente?
* ¿Quién participa en esta parte del negocio?
* ¿Qué lenguaje usan los expertos de dominio?
* ¿Qué flujos ya existen?
* ¿Qué problemas son visibles?
* ¿Qué supuestos estamos haciendo?
* ¿Qué seguimos sin entender?

El objetivo no es modelar todo. Es entender lo suficiente para continuar con mejores preguntas.

### Artefactos comunes de apoyo

* glosario
* notas de conceptos
* notas de entrevistas de dominio
* lista de actores
* preguntas abiertas
* lista de supuestos
* bocetos tempranos de flujo

### Riesgo principal evitado

Diseñar artefactos antes de entender el mundo al que pertenecen.

## 2. Contextualizing

Contextualizing es la etapa donde el equipo organiza el conocimiento descubierto en un escenario base visible.

Esta etapa se relaciona con la base de la pirámide de construcción, donde el equipo toma la arena extraída durante Understanding y empieza a colocarla en el sitio de construcción.

El objetivo es hacer entendible el contexto actual, y puede incluir:

* áreas o departamentos relevantes
* actores y responsabilidades
* flujos actuales
* sistemas actuales
* puntos de dolor actuales
* límites actuales
* lenguaje de negocio relevante
* relaciones entre conceptos

Contextualizing no define la solución final. Su propósito es hacer visible la situación actual lo suficiente para apoyar mejores decisiones.

El equipo pregunta:

* ¿Cuál es el escenario actual?
* ¿Cómo se mueve el trabajo hoy?
* ¿Qué áreas, actores o sistemas participan?
* ¿Qué flujos rodean el objetivo?
* ¿Qué conceptos son fundacionales?
* ¿Qué límites están empezando a aparecer?
* ¿Qué debería preservarse como entendimiento compartido?

Una base fuerte hace que las decisiones posteriores sean más seguras. Sin suficiente base contextual, los artefactos posteriores pueden parecer precisos, pero seguir siendo inestables.

### Artefactos comunes de apoyo

* notas del escenario actual
* bocetos de flujo
* diagramas de carriles
* mapa de responsabilidades
* mapa de contexto
* notas de relaciones entre conceptos
* lista de puntos de dolor
* notas de límites

### Riesgo principal evitado

Tratar un problema, caso de uso o *feature* como algo aislado cuando en realidad pertenece a un contexto mayor.

## 3. Planning

Planning es la etapa donde el equipo decide cómo debería mejorar la situación actual.

El equipo usa la base contextual para identificar qué parte del negocio debería cambiar y por qué. Esta etapa cambia la mentalidad:

> ¿Qué está pasando? -> ¿Qué debería mejorar?

Planning se enfoca en:

* impacto de negocio
* factibilidad
* riesgo
* alcance
* *tradeoffs*
* flujos afectados
* posibles mejoras

El equipo pregunta:

* ¿Qué problemas vale la pena resolver ahora?
* ¿Qué mejora crea valor de negocio significativo?
* ¿Qué flujos adyacentes podrían verse afectados?
* ¿Qué riesgos o mitigaciones existen?
* ¿Qué debería permanecer fuera de la iteración actual?
* ¿Cómo se vería el escenario mejorado?
* ¿Qué casos de uso, procesos, capacidades o servicios podrían necesitarse?

El resultado de Planning debería ser lo suficientemente preciso para guiar la implementación sin pretender que cada detalle futuro ya es conocido.

### Artefactos comunes de apoyo

* propuesta de mejora
* notas del escenario objetivo
* notas de alcance
* notas de *tradeoff*
* notas de riesgo
* notas de decisión
* lista de flujos afectados
* bocetos de casos de uso
* bocetos de proceso objetivo

### Riesgo principal evitado

Resolver el problema técnico más atractivo en vez del problema de negocio más relevante.

## 4. Building

Building es la etapa donde la mejora planificada se vuelve real. Esto incluye desarrollo, integración, validación, entrega y *feedback*.

En esta etapa, los artefactos de diseño se traducen en decisiones de implementación. El equipo puede definir o implementar:

* *features*
* flujos
* capacidades
* tipos de dominio
* integraciones
* servicios
* errores esperados
* cambios de despliegue
* ajustes operacionales

Building no está separado del entendimiento. Prueba el entendimiento acumulado hasta ahora.

Cuando el equipo construye, descubre si las etapas anteriores fueron suficientemente claras, incompletas o incorrectas.

El resultado de Building produce valor de negocio, pero también produce nuevo conocimiento.

Ese nuevo conocimiento se vuelve material para la siguiente iteración.

El equipo pregunta:

* ¿Qué necesita implementarse ahora?
* ¿Qué supuestos se están probando?
* ¿Qué artefactos de diseño están guiando la implementación?
* ¿Qué nuevas restricciones aparecieron durante el desarrollo?
* ¿Qué cambió después de la entrega?
* ¿Qué aprendió el equipo?
* ¿Qué debería explorarse después?

### Artefactos comunes de apoyo

* notas de *feature*
* notas de implementación
* notas de validación
* notas de entrega
* notas de *feedback*
* notas de decisión técnica
* notas de restricciones descubiertas
* notas de siguiente iteración

### Riesgo principal evitado

Tratar la implementación como el final del aprendizaje.

## Volver a Understanding

La iteración no termina después de Building; de hecho, vuelve a Understanding.

Cada mejora entregada cambia el contexto de negocio.

* Una nueva *feature* puede crear nuevos *workflows*.
* Un nuevo *workflow* puede revelar nuevas responsabilidades.
* Una nueva responsabilidad puede exponer nuevos riesgos.
* Un nuevo riesgo puede requerir nueva planificación.
* Un nuevo comportamiento en producción puede desafiar supuestos previos.

Por eso VSlices Design trata la iteración como un ciclo.

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

El equipo no vuelve al inicio porque falló. Vuelve porque el dominio evolucionó.
