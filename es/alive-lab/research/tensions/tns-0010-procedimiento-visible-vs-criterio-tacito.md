---
type: tension
state: observed
code: TNS-0010
title: Procedimiento visible vs criterio tácito

related_questions:
* RQ-001

related_studies:
* STU-004

related_observations:
* OBS-0015
* OBS-0016
* OBS-0019

related_findings:
* FND-0004

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

confidentiality:
  level: internal
  reason: exploratory-case
  publishable: anonymized-only

evidence:
  level: exploratory-observed
  artifacts_available: partial
  source: practical observation and Alive Lab cases
-------------------------------------------------

# TNS-0010 — Procedimiento visible vs criterio tácito

## Tipo

tension

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-004 — Riesgo de escape de conocimiento en contextos no digitalizados](../studies/stu-004-non-digitalized-knowledge-escape.md)

## Tensión

En contextos no digitalizados, el descubrimiento inicial puede capturar el procedimiento visible: los pasos que las personas dicen realizar, las acciones que parecen repetirse y la secuencia general del trabajo.

Pero, al mismo tiempo, parte importante del conocimiento puede estar en criterios tácitos: cómo se decide, cuándo se hace una excepción, qué señales importan, qué se prioriza, qué se omite y qué ajustes ocurren durante la práctica real.

La tensión puede formularse así:

> Necesitamos capturar el procedimiento visible para comenzar a entender el trabajo, pero también necesitamos descubrir los criterios tácitos que explican cómo ese procedimiento se adapta, interpreta y ejecuta realmente.

## Fuerza A

La primera fuerza es el procedimiento visible.

Cuando se intenta digitalizar un contexto no digitalizado, el procedimiento visible suele ser el punto de entrada más accesible.

Permite identificar:

* qué pasos parecen existir
* qué información se usa
* qué acciones se repiten
* qué personas participan
* qué resultados se esperan
* qué artifacts manuales existen
* qué partes del trabajo podrían ordenarse o automatizarse
* qué secuencia general sostiene la operación

Esta fuerza importa porque sin una primera comprensión del procedimiento, el descubrimiento puede volverse demasiado abstracto.

El procedimiento visible ayuda a iniciar conversación, ordenar observaciones y construir una primera representación del trabajo.

## Fuerza B

La segunda fuerza es el criterio tácito.

El procedimiento visible puede no explicar suficientemente cómo se decide en la práctica.

Las personas pueden adaptar el trabajo según criterios que no siempre están escritos o verbalizados inicialmente.

Estos criterios pueden incluir:

* cuándo priorizar un caso sobre otro
* cuándo saltarse un paso
* cuándo pedir confirmación
* cuándo revisar una fuente adicional
* cuándo una excepción es aceptable
* cuándo una señal indica riesgo
* cuándo una clasificación local aplica
* cuándo un dato aparentemente menor cambia la decisión
* cuándo una regla declarada no se sigue exactamente
* cuándo el contexto material, temporal o social modifica la acción

Esta fuerza importa porque digitalizar solo el procedimiento visible puede producir software que reproduce pasos, pero no captura la inteligencia práctica que permite ejecutarlos correctamente.

## Por qué importa

Esta tensión importa porque muchas digitalizaciones iniciales pueden confundir procedimiento con conocimiento suficiente.

Un procedimiento puede decir qué se hace, pero no siempre explicar cómo se decide.

Si el descubrimiento observa solo el procedimiento visible, pueden aparecer riesgos como:

* automatizar pasos sin comprender criterios
* omitir excepciones frecuentes
* capturar una versión idealizada del trabajo
* construir reglas demasiado rígidas
* perder señales usadas por las personas para decidir
* digitalizar lo declarado, pero no lo practicado
* crear software que funciona para casos simples, pero falla ante variaciones reales

Pero si se intenta capturar todo criterio tácito antes de avanzar, también aparecen riesgos:

* análisis excesivo
* dificultad para distinguir criterio relevante de hábito accidental
* retraso de una solución útil
* sobreformalización de decisiones situadas
* pérdida de aprendizaje desde el uso real
* intento de explicitar conocimiento que quizá puede permanecer situado temporalmente

El problema no es elegir entre procedimiento visible o criterio tácito.

El problema es reconocer qué criterios tácitos son necesarios para que la primera digitalización no represente mal el dominio.

## Evidencia

La evidencia disponible es exploratoria y parcial.

Puede formularse en términos generales:

* Se observa que algunos contextos no digitalizados operan mediante prácticas cotidianas no completamente documentadas.
* Se observa que las personas pueden describir procedimientos visibles sin explicitar todos los criterios usados para decidir.
* Se observa que parte del conocimiento relevante aparece durante la ejecución real, no necesariamente durante una descripción inicial.
* Se observa que algunas excepciones, prioridades o ajustes cotidianos pueden no aparecer como reglas formales.
* Se observa que digitalizar solo los pasos visibles puede omitir conocimiento necesario para interpretar correctamente el trabajo.
* Se observa que no todo criterio tácito necesita ser formalizado de inmediato, pero algunos criterios sí pueden ser críticos para preservar continuidad.

La evidencia disponible todavía no constituye validación fuerte.

Debe tratarse como observación exploratoria dentro de VSlices Research.

## Observaciones relacionadas

* [OBS-0015 — En contextos no digitalizados, el conocimiento relevante puede estar embebido en prácticas cotidianas y no existir como artifact explícito](../observations/obs-0015-conocimiento-embebido-practicas-cotidianas.md)
* [OBS-0016 — El levantamiento inicial puede capturar procedimientos visibles, pero omitir criterios tácitos usados para decidir](../observations/obs-0016-levantamiento-captura-procedimientos-visibles-omite-criterios-tacitos.md)
* [OBS-0019 — El conocimiento puede escaparse cuando se modela solo lo que las personas dicen hacer y no lo que realmente hacen](../observations/obs-0019-conocimiento-escapa-modelar-dicho-no-practica-real.md)

## Tensiones relacionadas

* [TNS-0009 — Rapidez de digitalización vs profundidad de descubrimiento](../tensions/tns-0009-rapidez-digitalizacion-vs-profundidad-descubrimiento.md)
* [TNS-0012 — Formalizar temprano vs mantener ambigüedad exploratoria](../tensions/tns-0012-formalizar-temprano-vs-mantener-ambiguedad-exploratoria.md)

## Posibles respuestas candidatas

* Usar el procedimiento visible como punto de partida, no como representación completa del dominio.
* Observar la práctica real además de escuchar descripciones del proceso.
* Preguntar por excepciones, decisiones difíciles y casos ambiguos.
* Registrar criterios tácitos cuando afectan decisiones relevantes.
* Diferenciar entre pasos del proceso y criterios de decisión.
* Marcar criterios no confirmados como hipótesis, no como reglas.
* Evitar automatizar decisiones tácitas antes de observar suficientes casos.
* Validar el procedimiento capturado contra situaciones reales.
* Mantener abiertas preguntas de dominio cuando el criterio todavía no está claro.
* Usar primeras soluciones digitales como instrumentos para descubrir criterios faltantes.

Estas respuestas son candidatas.

No deben tratarse todavía como soluciones validadas.

## Riesgo de sobrecorrección

Si se favorece demasiado el procedimiento visible, la digitalización puede reproducir una versión superficial del trabajo.

Esto puede producir:

* reglas incompletas
* software rígido
* omisión de excepciones relevantes
* pérdida de criterio operativo
* decisiones automatizadas con supuestos débiles
* falsa sensación de comprensión
* necesidad de corregir el modelo después de fallas reales

Si se favorece demasiado el criterio tácito, el descubrimiento puede intentar capturar demasiados matices antes de construir algo útil.

Esto puede producir:

* levantamientos extensos
* dificultad para avanzar
* documentación difícil de usar
* exceso de excepciones prematuras
* confusión entre criterio crítico y preferencia local
* demora en validar con uso real

La respuesta candidata no debería ser digitalizar solo pasos visibles ni intentar formalizar todo criterio tácito desde el inicio.

La respuesta probablemente está en identificar qué criterios tácitos afectan continuidad, riesgo o comportamiento relevante.

## Interpretación inicial

Esta tensión sugiere que el conocimiento de un contexto no digitalizado no está solo en los pasos del proceso.

También está en los criterios que permiten interpretar cuándo, cómo y por qué esos pasos cambian.

Desde VSlices Research, esto refuerza una idea importante:

> un procedimiento visible puede ser una entrada al descubrimiento, pero no necesariamente una explicación suficiente del dominio.

Preservar continuidad durante la digitalización inicial puede requerir conectar:

* acciones observables
* criterios de decisión
* excepciones recurrentes
* señales contextuales
* supuestos iniciales
* ambigüedades pendientes
* decisiones que todavía no deben formalizarse

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Límite

Esta tensión no demuestra que todo procedimiento visible sea insuficiente.

Tampoco demuestra que todo criterio tácito deba descubrirse o documentarse antes de digitalizar.

En algunos casos, el procedimiento visible puede ser suficiente para una primera solución útil, especialmente si el riesgo es bajo, el proceso es simple o la digitalización se plantea como aprendizaje progresivo.

La tensión solo registra que, en contextos no digitalizados, existe una fricción entre capturar pasos visibles y descubrir criterios tácitos que pueden ser necesarios para representar correctamente el dominio.

Para fortalecer esta tensión, VSlices Research necesita casos documentables donde pueda compararse:

* procedimiento declarado
* práctica real observada
* criterios tácitos identificados
* criterios omitidos
* impacto de omitir criterios
* decisiones automatizadas
* correcciones posteriores al modelo inicial
* utilidad de mantener criterios como hipótesis antes de formalizarlos

## Próxima evidencia necesaria

* Casos documentables donde el procedimiento visible haya sido suficiente para una primera digitalización.
* Casos documentables donde el procedimiento visible haya omitido criterios relevantes.
* Ejemplos donde observar la práctica revele criterios no declarados.
* Ejemplos donde formalizar criterios demasiado pronto haya generado rigidez.
* Evidencia sobre cómo distinguir criterios críticos de hábitos accesorios.
* Evidencia sobre cómo validar criterios tácitos antes de automatizarlos.
* Observaciones sobre cómo documentar criterios como hipótesis de dominio.
* Casos donde una primera solución digital ayude a descubrir criterios faltantes.
