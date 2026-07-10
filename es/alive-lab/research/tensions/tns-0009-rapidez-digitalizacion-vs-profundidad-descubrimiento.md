---
type: tension
state: observed
code: TNS-0009
title: Rapidez de digitalización vs profundidad de descubrimiento

related_questions:
* RQ-001

related_studies:
* STU-004

related_observations:
* OBS-0015
* OBS-0016
* OBS-0017
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

# TNS-0009 — Rapidez de digitalización vs profundidad de descubrimiento

## Tipo

tension

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-004 — Riesgo de escape de conocimiento en contextos no digitalizados](../studies/stu-004-non-digitalized-knowledge-escape.md)

## Tensión

En contextos no digitalizados, puede existir presión por digitalizar rápido para resolver una necesidad práctica, ordenar información, automatizar trabajo o reducir carga operativa.

Pero, al mismo tiempo, una digitalización demasiado rápida puede capturar solo la parte visible del proceso y dejar escapar conocimiento relevante que todavía no ha sido descubierto, observado o explicitado.

La tensión puede formularse así:

> Necesitamos avanzar rápido hacia una solución digital útil, pero también necesitamos descubrir suficiente conocimiento del dominio para no congelar una interpretación parcial de la práctica real.

## Fuerza A

La primera fuerza es la rapidez de digitalización.

En contextos no digitalizados, digitalizar rápido puede ser necesario porque el trabajo actual puede depender de memoria, esfuerzo manual, repetición, coordinación informal o artifacts frágiles.

La rapidez puede importar porque permite:

* reducir carga operativa
* ordenar información dispersa
* evitar olvidos frecuentes
* disminuir trabajo manual repetitivo
* hacer visible información antes escondida
* entregar valor temprano
* validar una primera forma de solución
* aprender desde el uso real
* evitar que el proceso de análisis bloquee la mejora práctica

Esta fuerza importa porque no todo contexto necesita una investigación extensa antes de recibir una mejora inicial.

A veces una solución pequeña, imperfecta y útil permite observar mejor el dominio que una fase larga de análisis previo.

## Fuerza B

La segunda fuerza es la profundidad de descubrimiento.

Aunque digitalizar rápido puede entregar valor, también puede producir una representación demasiado superficial del dominio si el proceso no explora prácticas reales, criterios tácitos, excepciones y decisiones situadas.

La profundidad de descubrimiento importa porque permite reconocer:

* qué conocimiento no está escrito
* qué criterios se usan realmente para decidir
* qué excepciones aparecen en la práctica
* qué diferencias existen entre procedimiento declarado y trabajo real
* qué categorías iniciales podrían ser insuficientes
* qué decisiones no deberían automatizarse todavía
* qué partes del proceso requieren observación antes de formalización
* qué ambigüedades deben mantenerse abiertas por un tiempo

Esta fuerza importa porque una digitalización inicial puede convertirse rápidamente en estructura dominante.

Si esa estructura nace desde una comprensión incompleta, puede congelar errores, omitir criterios relevantes o volver invisible parte del conocimiento cotidiano.

## Por qué importa

Esta tensión importa porque el inicio de una digitalización es un momento de alto riesgo conceptual.

Cuando todavía no existe software, las primeras decisiones de estructura, categorías, campos, flujos y automatización pueden parecer simples o provisorias, pero pueden influir en cómo el dominio será entendido después.

Si se prioriza solo la rapidez, pueden aparecer riesgos como:

* capturar solo procedimientos visibles
* ignorar criterios tácitos
* automatizar excepciones mal entendidas
* modelar categorías demasiado tempranas
* convertir una solución inicial en verdad operacional
* ocultar diferencias entre lo que se dice hacer y lo que realmente se hace
* reducir el dominio a lo que era fácil de digitalizar

Si se prioriza solo la profundidad de descubrimiento, también aparecen riesgos:

* parálisis por análisis
* retraso de mejoras concretas
* exploración excesiva para problemas pequeños
* documentación previa que envejece antes de usarse
* pérdida de motivación por falta de resultados
* dificultad para validar con uso real
* formalización investigativa sin impacto práctico

El problema no es elegir entre rapidez o profundidad.

El problema es decidir cuánta exploración es suficiente para avanzar sin perder conocimiento relevante.

## Evidencia

La evidencia disponible es exploratoria y parcial.

Puede formularse en términos generales:

* Se observa que algunos contextos operan sin software especializado previo.
* Se observa que parte del conocimiento relevante puede estar embebido en prácticas cotidianas.
* Se observa que las personas pueden describir procedimientos visibles sin explicitar todos los criterios usados en la práctica.
* Se observa que ciertas excepciones o decisiones solo aparecen durante la ejecución real.
* Se observa que una primera solución digital puede capturar categorías visibles, pero omitir matices del uso real.
* Se observa que digitalizar demasiado rápido puede congelar una interpretación parcial del dominio.
* Se observa que explorar demasiado antes de construir también puede retrasar aprendizaje útil desde el uso real.

La evidencia disponible todavía no constituye validación fuerte.

Debe tratarse como observación exploratoria dentro de VSlices Research.

## Observaciones relacionadas

* [OBS-0015 — En contextos no digitalizados, el conocimiento relevante puede estar embebido en prácticas cotidianas y no existir como artifact explícito](../observations/obs-0015-conocimiento-embebido-practicas-cotidianas.md)
* [OBS-0016 — El levantamiento inicial puede capturar procedimientos visibles, pero omitir criterios tácitos usados para decidir](../observations/obs-0016-levantamiento-captura-procedimientos-visibles-omite-criterios-tacitos.md)
* [OBS-0017 — Digitalizar un proceso no explorado puede congelar una interpretación parcial del dominio](../observations/obs-0017-digitalizar-proceso-no-explorado-congela-interpretacion-parcial.md)
* [OBS-0019 — El conocimiento puede escaparse cuando se modela solo lo que las personas dicen hacer y no lo que realmente hacen](../observations/obs-0019-conocimiento-escapa-modelar-dicho-no-practica-real.md)

## Posibles respuestas candidatas

* Digitalizar por slices pequeños y revisables.
* Mantener explícitas las hipótesis de dominio de la primera solución.
* Distinguir entre estructura provisional y modelo estable.
* Observar la práctica real antes de formalizar decisiones críticas.
* Capturar criterios tácitos cuando afectan decisiones relevantes.
* Evitar automatizar excepciones antes de entenderlas.
* Usar la primera digitalización como instrumento de aprendizaje, no como cierre del dominio.
* Registrar dudas y límites de la comprensión inicial.
* Validar categorías iniciales con uso real.
* Permitir que el modelo evolucione después de observar casos concretos.

Estas respuestas son candidatas.

No deben tratarse todavía como soluciones validadas.

## Riesgo de sobrecorrección

Si se favorece demasiado la rapidez de digitalización, el sistema puede nacer desde una comprensión insuficiente del dominio.

Esto puede producir:

* pérdida de conocimiento tácito
* categorías prematuras
* automatización de supuestos incorrectos
* software que representa solo el procedimiento visible
* omisión de excepciones relevantes
* dificultad para corregir el modelo después
* falsa sensación de que el proceso ya fue entendido

Si se favorece demasiado la profundidad de descubrimiento, el equipo puede retrasar innecesariamente una mejora útil.

Esto puede producir:

* análisis excesivo
* documentación sin validación práctica
* falta de entrega temprana
* cansancio de quienes participan en el descubrimiento
* dificultad para aprender desde casos reales
* pérdida de oportunidad de reducir dolor inmediato

La respuesta candidata no debería ser digitalizar sin descubrir ni descubrir indefinidamente antes de digitalizar.

La respuesta probablemente está en digitalizar de forma progresiva, manteniendo abiertas las preguntas de dominio que todavía no han sido suficientemente observadas.

## Interpretación inicial

Esta tensión sugiere que la digitalización inicial debería tratarse como un proceso de aprendizaje, no solo como conversión de procedimientos manuales en software.

En contextos no digitalizados, la primera solución puede ayudar a descubrir el dominio, pero también puede ocultarlo si se vuelve demasiado rígida demasiado pronto.

Desde VSlices Research, esto refuerza una idea importante:

> la continuidad puede escaparse al inicio si la necesidad de avanzar rápido impide descubrir el conocimiento que aún vive en la práctica.

Preservar continuidad en esta etapa puede requerir mantener una relación explícita entre:

* lo que se observó
* lo que se asumió
* lo que se decidió digitalizar
* lo que quedó pendiente de descubrir
* lo que debe revisarse después del uso real

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Límite

Esta tensión no demuestra que digitalizar rápido sea incorrecto.

Tampoco demuestra que siempre se necesite un descubrimiento profundo antes de construir software.

En algunos contextos, una digitalización rápida puede ser la mejor forma de reducir dolor inmediato y generar evidencia para aprender.

La tensión solo registra que, en contextos no digitalizados, existe una fricción entre avanzar rápido hacia una solución y descubrir suficiente conocimiento para evitar que la digitalización inicial omita elementos relevantes del dominio.

Para fortalecer esta tensión, VSlices Research necesita casos documentables donde pueda compararse:

* velocidad de digitalización
* profundidad de descubrimiento
* conocimiento capturado
* conocimiento omitido
* supuestos iniciales
* ajustes posteriores al uso real
* costo de formalizar temprano
* costo de explorar demasiado antes de construir

## Próxima evidencia necesaria

* Casos documentables donde digitalizar rápido haya entregado valor temprano.
* Casos documentables donde digitalizar rápido haya omitido conocimiento relevante.
* Casos donde descubrimiento adicional haya evitado errores de modelado.
* Casos donde exploración excesiva haya retrasado innecesariamente valor práctico.
* Evidencia sobre qué señales indican que se puede digitalizar con seguridad.
* Evidencia sobre qué señales indican que todavía falta descubrimiento.
* Observaciones sobre cómo validar hipótesis de dominio después de una primera digitalización.
* Observaciones sobre cómo documentar supuestos iniciales sin convertir el proceso en burocracia.
* Casos donde la digitalización progresiva preserve continuidad sin frenar aprendizaje.
