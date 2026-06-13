# Flujo de iteración de diseño

VSlices Design usa un flujo de iteración recurrente:

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

Este flujo es compartido por todas las modalidades de VSlices Design; las etapas siempre son las mismas en todas las modalidades, pero cambia el énfasis.

- Algunas situaciones requieren más comprensión antes de planificar.
- Algunas situaciones requieren una base contextual más sólida antes de construir.
- Algunas situaciones requieren un feedback de implementación más rápido.

Por eso VSlices Design usa modalidades; no reemplazan el flujo de iteración, solo cambian cuánta atención recibe cada etapa.

## Relación con las pirámides

El flujo de iteración usa las dos metáforas explicadas en `understanding.md`:

- pirámide invertida
- pirámide de construcción

Cada etapa del flujo de iteración puede entenderse mediante esas metáforas.

| Stage | Main metaphor | Purpose |
| --- | --- | --- |
| Understanding | Inverted pyramid | Extract domain knowledge |
| Contextualizing | Construction pyramid base | Build the base scenario |
| Planning | Construction pyramid middle | Decide the intended improvement |
| Building | Construction pyramid height | Implement, validate, and deliver value |

El flujo es cíclico.

Después de Building, el equipo vuelve a Understanding porque cada cambio entregado modifica el contexto y crea nuevo conocimiento.

## 1. Understanding

Understanding es la etapa donde el equipo extrae conocimiento del dominio.

El equipo explora el contexto de negocio escuchando a expertos del dominio, observando el trabajo existente, identificando vocabulario, descubriendo conceptos y detectando flows relevantes.

Esta etapa está relacionada con la pirámide invertida, donde el negocio se trata como una superficie amplia de conocimiento de dominio. Y para entender un objetivo específico, el equipo debe quitar los granos de arena que lo cubren. Quitar granos significa entenderlos.

El equipo pregunta:

- ¿Qué conceptos aparecen repetidamente?
- ¿Quién participa en esta parte del negocio?
- ¿Qué lenguaje usan los expertos del dominio?
- ¿Qué flows ya existen?
- ¿Qué problemas son visibles?
- ¿Qué supuestos estamos haciendo?
- ¿Qué seguimos sin entender?

El objetivo no es modelarlo todo. Es entender lo suficiente para continuar con mejores preguntas.

### Artefactos de apoyo comunes

- glossary
- concept notes
- domain interview notes
- actor list
- open questions
- assumption list
- early flow sketches

### Riesgo principal evitado

Diseñar artefactos antes de entender el mundo al que pertenecen.

## 2. Contextualizing

Contextualizing es la etapa donde el equipo organiza el conocimiento descubierto en una base visible del escenario.

Esta etapa está relacionada con la base de la pirámide de construcción, donde el equipo toma la arena extraída durante Understanding y empieza a colocarla en el sitio de construcción.

El objetivo es hacer comprensible el contexto actual, y puede incluir:

- áreas o departamentos relevantes
- actores y responsabilidades
- flows actuales
- sistemas actuales
- puntos de dolor actuales
- límites actuales
- lenguaje de negocio relevante
- relaciones entre conceptos

Contextualizing no define la solución final; su propósito es hacer visible la situación actual lo suficiente como para apoyar mejores decisiones.

El equipo pregunta:

- ¿Cuál es el escenario actual?
- ¿Cómo se mueve el trabajo hoy?
- ¿Qué áreas, actores o sistemas participan?
- ¿Qué flows rodean el objetivo?
- ¿Qué conceptos son fundamentales?
- ¿Qué límites están empezando a aparecer?
- ¿Qué debe preservarse como entendimiento compartido?

Una base sólida hace que las decisiones posteriores sean más seguras. Sin suficiente base contextual, los artefactos posteriores pueden parecer precisos pero seguir siendo inestables.

### Artefactos de apoyo comunes

- current scenario notes
- flow sketches
- swimlane diagrams
- responsibility map
- context map
- concept relationship notes
- pain point list
- boundary notes

### Riesgo principal evitado

Tratar un problema, use case o feature como algo aislado cuando en realidad pertenece a un contexto más amplio.

## 3. Planning

Planning es la etapa donde el equipo decide cómo debería mejorar la situación actual.

El equipo usa la base contextual para identificar qué parte del negocio debería cambiar y por qué. Esta etapa cambia la mentalidad:

> ¿Qué está pasando? -> ¿Qué debería mejorar?

Planning se enfoca en:

- business impact
- feasibility
- risk
- scope
- tradeoffs
- affected flows
- possible improvements

El equipo pregunta:

- ¿Qué problemas vale la pena resolver ahora?
- ¿Qué mejora crea valor de negocio significativo?
- ¿Qué flows adyacentes podrían verse afectados?
- ¿Qué riesgos o mitigaciones existen?
- ¿Qué debe permanecer fuera de la iteración actual?
- ¿Cómo se vería el escenario mejorado?
- ¿Qué use cases, processes, capabilities o services pueden ser necesarios?

El resultado de Planning debe ser lo suficientemente preciso para guiar la implementación sin fingir que ya se conocen todos los detalles futuros.

### Artefactos de apoyo comunes

- improvement proposal
- target scenario notes
- scope notes
- tradeoff notes
- risk notes
- decision notes
- affected flow list
- use case sketches
- target process sketches

### Riesgo principal evitado

Resolver el problema técnico más atractivo en lugar del problema de negocio más relevante.

## 4. Building

Building es la etapa donde la mejora planificada se vuelve real. Esto incluye desarrollo, integración, validación, entrega y feedback.

En esta etapa, los artefactos de diseño se traducen en decisiones de implementación. El equipo puede definir o implementar:

- features
- flows
- capabilities
- domain types
- integrations
- services
- expected errors
- deployment changes
- operational adjustments

Building no está separado de Understanding. Prueba el entendimiento acumulado hasta ese momento.

Cuando el equipo construye, descubre si las etapas anteriores fueron lo suficientemente claras, incompletas o incorrectas.

El resultado de Building produce valor de negocio, pero también produce nuevo conocimiento.

Ese nuevo conocimiento se convierte en material para la siguiente iteración.

El equipo pregunta:

- ¿Qué debe implementarse ahora?
- ¿Qué supuestos se están probando?
- ¿Qué artefactos de diseño están guiando la implementación?
- ¿Qué nuevas restricciones aparecieron durante el desarrollo?
- ¿Qué cambió después de la entrega?
- ¿Qué aprendió el equipo?
- ¿Qué debería explorarse después?

### Artefactos de apoyo comunes

- feature notes
- implementation notes
- validation notes
- delivery notes
- feedback notes
- technical decision notes
- discovered constraint notes
- next-iteration notes

### Riesgo principal evitado

Tratar la implementación como el final del aprendizaje.

## Volver a Understanding

La iteración no termina después de Building; de hecho, vuelve a Understanding.

Cada mejora entregada cambia el contexto de negocio.

- Una nueva feature puede crear nuevos workflows.
- Un nuevo workflow puede revelar nuevas responsabilidades.
- Una nueva responsabilidad puede exponer nuevos riesgos.
- Un nuevo riesgo puede requerir nueva planificación.
- Un nuevo comportamiento en producción puede desafiar supuestos previos.

Por eso VSlices Design trata la iteración como un bucle.

```text
Understanding -> Contextualizing -> Planning -> Building -> Understanding
```

El equipo no vuelve al principio porque falló. Vuelve porque el dominio ha evolucionado.

## Modalidades y énfasis de etapa

Todas las modalidades de VSlices Design usan el mismo flujo de iteración; cambian el énfasis.

> Context-First da más peso a Understanding y Contextualizing.
> Problem-First da más peso a Planning manteniendo suficiente Understanding y Contextualizing alrededor del problema.
> Slice-First da más peso a Building para que el equipo pueda aprender rápido de una pequeña implementación vertical.

La modalidad debe encajar con el tipo de incertidumbre y contexto que el equipo está enfrentando.

| Modality | Main emphasis | Useful when |
| --- | --- | --- |
| Context-First | Understanding and Contextualizing | The domain is unclear, broad, fragmented, or organizationally complex |
| Problem-First | Planning with enough context | A clear problem exists, but its surrounding context still matters |
| Slice-First | Building and feedback | The team can learn faster from a small working slice |

## Preparación para construir

Building puede comenzar cuando el equipo tiene suficiente claridad para tomar decisiones de implementación sin depender solo de supuestos.

Esto no significa que cada detalle deba conocerse; solo significa que el equipo puede explicar:

- qué se está mejorando
- por qué importa
- qué contexto respalda la decisión
- qué conceptos están involucrados
- qué flows o responsabilidades se ven afectados
- cuál es el resultado previsto
- qué incertidumbre permanece

Una feature no debería aparecer como una decisión aislada. Debería ser el resultado visible de un camino que comenzó desde una comprensión más amplia.

## Regla de complejidad

El flujo de iteración debe seguir siendo progresivo; el equipo no debería crear todos los artefactos posibles en cada iteración.

El nivel de detalle debería crecer solo cuando ayude a:

- preservar el entendimiento
- reducir el riesgo
- aclarar decisiones
- guiar la implementación
- proteger la intención del negocio

Los dominios pequeños pueden necesitar solo notas ligeras y diagramas simples. Los dominios complejos pueden requerir análisis, modelado y documentación más profundos.

El flujo debe adaptarse al dominio. El dominio nunca debe ser forzado a adaptarse al flujo. VSlices Design no es un embudo burocrático.

Es una forma de asegurar que el software concreto esté respaldado por suficiente comprensión contextual. El equipo debe moverse deliberadamente; puede ser lento o rápido, pero debe ser deliberado.

## Aclaraciones

### Sobre los artefactos

Los artefactos de apoyo son ayudas opcionales. No son documentos obligatorios.

Un equipo debe crearlos solo cuando ayuden a preservar el entendimiento, reducir el riesgo, aclarar decisiones o guiar la implementación.

### Sobre el cambio de modalidad

Un equipo puede cambiar de modalidad entre iteraciones.

Empezar con Context-First no obliga al equipo a permanecer en Context-First para siempre.

A medida que la incertidumbre cambia, la modalidad también puede cambiar.
