---
type: tension
state: observed
code: TNS-0011
title: Automatizar práctica actual vs descubrir necesidad real

related_questions:
* RQ-001

related_studies:
* STU-004

related_observations:
* OBS-0015
* OBS-0016
* OBS-0017
* OBS-0018
* OBS-0019

related_tensions:
* TNS-0009
* TNS-0010
* TNS-0012

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

# TNS-0011 — Automatizar práctica actual vs descubrir necesidad real

## Tipo

tension

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-004 — Riesgo de escape de conocimiento en contextos no digitalizados](../studies/stu-004-non-digitalized-knowledge-escape.md)

## Tensión

En contextos no digitalizados, una primera digitalización puede partir desde la práctica actual: lo que las personas hacen hoy, los pasos que siguen, las herramientas que usan y las formas concretas en que resuelven el trabajo.

Pero, al mismo tiempo, la práctica actual no siempre representa la necesidad real.

Puede ser una adaptación, una compensación, un hábito, una solución de emergencia, una restricción heredada o una forma local de sobrevivir a la ausencia de mejores herramientas.

La tensión puede formularse así:

> Necesitamos entender la práctica actual para construir desde la realidad, pero también necesitamos descubrir la necesidad real para no automatizar accidentalmente una solución provisional, limitada o deformada por restricciones existentes.

## Fuerza A

La primera fuerza es automatizar la práctica actual.

En un contexto no digitalizado, la práctica actual suele ser la evidencia más cercana al trabajo real.

Observarla permite reconocer:

* qué hacen las personas hoy
* qué pasos se repiten
* qué información se usa
* qué artifacts manuales existen
* qué decisiones aparecen en la operación
* qué tareas generan carga
* qué excepciones ocurren
* qué dolores concretos existen
* qué partes podrían ordenarse o automatizarse

Esta fuerza importa porque una solución que ignora la práctica real corre el riesgo de diseñar desde abstracciones demasiado lejanas.

La práctica actual permite partir desde evidencia, no solo desde intención.

## Fuerza B

La segunda fuerza es descubrir la necesidad real.

La práctica actual puede estar condicionada por limitaciones que no deberían preservarse.

Puede existir porque las personas tuvieron que adaptarse a:

* falta de software
* falta de información disponible
* herramientas manuales
* restricciones de tiempo
* acuerdos informales
* errores históricos
* procesos heredados
* coordinación difícil
* baja visibilidad de datos
* dependencia de memoria
* soluciones temporales que se volvieron permanentes

Esta fuerza importa porque automatizar una práctica sin entender la necesidad que intenta resolver puede convertir un workaround en sistema.

En vez de reducir el problema, el software podría estabilizarlo.

## Por qué importa

Esta tensión importa porque digitalizar no debería significar copiar mecánicamente la práctica actual.

La práctica actual es evidencia, pero no necesariamente destino.

Si se automatiza sin explorar la necesidad real, pueden aparecer riesgos como:

* preservar pasos innecesarios
* digitalizar workarounds
* convertir restricciones antiguas en reglas nuevas
* mantener categorías accidentales
* reforzar hábitos poco útiles
* ocultar problemas de fondo
* construir software que mejora la ejecución de una práctica que quizá debía rediseñarse
* confundir “así se hace hoy” con “así debería funcionar”

Pero si se ignora demasiado la práctica actual, también aparecen riesgos:

* diseñar una solución desconectada del contexto
* perder conocimiento situado
* subestimar restricciones reales
* imponer categorías externas
* simplificar excesivamente el dominio
* no reconocer dolores operativos concretos
* crear software que parece correcto, pero no calza con la vida real

El problema no es elegir entre práctica actual o necesidad real.

El problema es usar la práctica actual como evidencia para descubrir qué necesidad sostiene, qué parte debe preservarse y qué parte podría cambiar.

## Evidencia

La evidencia disponible es exploratoria y parcial.

Puede formularse en términos generales:

* Se observa que algunos contextos operan sin software especializado previo.
* Se observa que las personas resuelven necesidades reales mediante prácticas manuales, informales o parcialmente estructuradas.
* Se observa que esas prácticas pueden contener conocimiento relevante del dominio.
* Se observa que algunas prácticas actuales pueden existir por restricciones, ausencia de herramientas o soluciones temporales.
* Se observa que una primera digitalización puede capturar la forma actual de trabajar sin cuestionar qué necesidad la originó.
* Se observa que automatizar una práctica actual puede preservar conocimiento útil, pero también puede congelar adaptaciones accidentales.
* Se observa que descubrir la necesidad real requiere mirar más allá de los pasos visibles.

La evidencia disponible todavía no constituye validación fuerte.

Debe tratarse como observación exploratoria dentro de VSlices Research.

## Observaciones relacionadas

* [OBS-0015 — En contextos no digitalizados, el conocimiento relevante puede estar embebido en prácticas cotidianas y no existir como artifact explícito](../observations/obs-0015-conocimiento-embebido-practicas-cotidianas.md)
* [OBS-0016 — El levantamiento inicial puede capturar procedimientos visibles, pero omitir criterios tácitos usados para decidir](../observations/obs-0016-levantamiento-captura-procedimientos-visibles-omite-criterios-tacitos.md)
* [OBS-0017 — Digitalizar un proceso no explorado puede congelar una interpretación parcial del dominio](../observations/obs-0017-digitalizar-proceso-no-explorado-congela-interpretacion-parcial.md)
* [OBS-0018 — La ausencia de software previo no implica ausencia de conocimiento estructurado](../observations/obs-0018-ausencia-software-previo-no-implica-ausencia-conocimiento-estructurado.md)
* [OBS-0019 — El conocimiento puede escaparse cuando se modela solo lo que las personas dicen hacer y no lo que realmente hacen](../observations/obs-0019-conocimiento-escapa-modelar-dicho-no-practica-real.md)

## Tensiones relacionadas

* [TNS-0009 — Rapidez de digitalización vs profundidad de descubrimiento](../tensions/tns-0009-rapidez-digitalizacion-vs-profundidad-descubrimiento.md)
* [TNS-0010 — Procedimiento visible vs criterio tácito](../tensions/tns-0010-procedimiento-visible-vs-criterio-tacito.md)
* [TNS-0012 — Formalizar temprano vs mantener ambigüedad exploratoria](../tensions/tns-0012-formalizar-temprano-vs-mantener-ambiguedad-exploratoria.md)

## Posibles respuestas candidatas

* Observar la práctica actual sin asumir que debe preservarse completa.
* Preguntar qué necesidad intenta resolver cada paso.
* Distinguir entre práctica esencial, workaround y hábito accidental.
* Identificar restricciones que dieron forma a la práctica actual.
* Separar necesidad del mecanismo usado actualmente para resolverla.
* Evitar automatizar pasos antes de entender su propósito.
* Mantener hipótesis explícitas sobre qué partes de la práctica deberían cambiar.
* Validar con casos reales si la práctica actual representa la necesidad.
* Usar la primera digitalización para descubrir qué partes del proceso pueden simplificarse.
* Revisar después del uso real qué partes fueron preservadas innecesariamente.

Estas respuestas son candidatas.

No deben tratarse todavía como soluciones validadas.

## Riesgo de sobrecorrección

Si se favorece demasiado la automatización de la práctica actual, el sistema puede digitalizar restricciones y hábitos sin cuestionarlos.

Esto puede producir:

* automatización de workarounds
* preservación de pasos innecesarios
* rigidez operativa
* falsa mejora por solo acelerar lo existente
* pérdida de oportunidad de rediseño
* software que hereda problemas del proceso manual
* confusión entre práctica observada y necesidad real

Si se favorece demasiado el descubrimiento de la necesidad real ignorando la práctica actual, el equipo puede diseñar una solución idealizada.

Esto puede producir:

* pérdida de conocimiento situado
* baja adopción
* falta de calce con restricciones reales
* omisión de criterios prácticos
* diseño excesivamente abstracto
* soluciones que no reducen el dolor cotidiano
* desconexión entre modelo y operación

La respuesta candidata no debería ser copiar la práctica actual ni reemplazarla desde una teoría externa.

La respuesta probablemente está en observar la práctica actual como evidencia, pero usarla para descubrir la necesidad que la sostiene.

## Interpretación inicial

Esta tensión sugiere que la práctica actual debe ser tratada como una fuente de conocimiento, no como una especificación definitiva.

Desde VSlices Research, esto refuerza una idea importante:

> digitalizar una práctica no explorada puede mejorar la operación, pero también puede preservar restricciones que el software tenía oportunidad de cuestionar.

Preservar continuidad no significa mantener todo igual.

Puede significar conservar el conocimiento relevante mientras se revisan las formas accidentales que surgieron por falta de herramientas, visibilidad o coordinación.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Límite

Esta tensión no demuestra que la práctica actual sea incorrecta.

Tampoco demuestra que toda digitalización deba rediseñar el proceso.

En muchos casos, la práctica actual puede ser una respuesta madura, situada y útil al contexto real.

La tensión solo registra que, en contextos no digitalizados, existe una fricción entre automatizar la forma actual de trabajar y descubrir la necesidad real que esa práctica intenta resolver.

Para fortalecer esta tensión, VSlices Research necesita casos documentables donde pueda compararse:

* práctica actual
* necesidad subyacente
* restricciones que moldearon la práctica
* pasos preservados
* pasos eliminados
* pasos rediseñados
* impacto de automatizar directamente
* impacto de descubrir la necesidad antes de automatizar
* cambios posteriores al uso real

## Próxima evidencia necesaria

* Casos documentables donde automatizar la práctica actual haya entregado valor suficiente.
* Casos donde automatizar la práctica actual haya preservado workarounds innecesarios.
* Casos donde descubrir la necesidad real haya permitido simplificar el proceso.
* Casos donde rediseñar sin respetar la práctica actual haya producido una solución desconectada.
* Evidencia sobre cómo distinguir práctica esencial de workaround.
* Evidencia sobre cómo documentar la necesidad detrás de una práctica.
* Observaciones sobre cómo validar si una práctica actual debe preservarse, cambiarse o eliminarse.
* Casos donde una primera digitalización revele qué partes del proceso actual eran accidentales.
