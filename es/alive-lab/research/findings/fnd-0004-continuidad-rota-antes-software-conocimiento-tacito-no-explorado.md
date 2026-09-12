---
type: finding
state: candidate
code: FND-0004
role: foundational
evidence_level: exploratory-observed
title: La continuidad de conocimiento puede romperse antes de existir software cuando el conocimiento tácito de un contexto no digitalizado no es explorado suficientemente

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
* TNS-0011
* TNS-0012

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

# FND-0004 — La continuidad de conocimiento puede romperse antes de existir software cuando el conocimiento tácito de un contexto no digitalizado no es explorado suficientemente

## Tipo

finding

## Rol

foundational

## Estado

candidate

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-004 — Riesgo de escape de conocimiento en contextos no digitalizados](../studies/stu-004-non-digitalized-knowledge-escape.md)

## Formulación

Esta evidencia sugiere que la continuidad de conocimiento puede romperse antes de que exista software, cuando el conocimiento tácito de un contexto no digitalizado no es explorado suficientemente durante el descubrimiento inicial.

En este escenario, el conocimiento no está perdido históricamente.

Tampoco está necesariamente disperso entre sistemas, servicios, equipos o áreas.

Tampoco depende solamente de una persona clave en transición.

El conocimiento existe en la práctica cotidiana, pero puede no estar suficientemente explicitado, observado, modelado o preservado cuando se inicia una digitalización.

Dicho de forma breve:

> La continuidad puede escaparse antes de que el software exista, cuando la digitalización captura solo una parte visible del dominio y deja fuera conocimiento tácito relevante.

## Observaciones que lo sostienen

* [OBS-0015 — En contextos no digitalizados, el conocimiento relevante puede estar embebido en prácticas cotidianas y no existir como artifact explícito](../observations/obs-0015-conocimiento-embebido-practicas-cotidianas.md)
* [OBS-0016 — El levantamiento inicial puede capturar procedimientos visibles, pero omitir criterios tácitos usados para decidir](../observations/obs-0016-levantamiento-captura-procedimientos-visibles-omite-criterios-tacitos.md)
* [OBS-0017 — Digitalizar un proceso no explorado puede congelar una interpretación parcial del dominio](../observations/obs-0017-digitalizar-proceso-no-explorado-congela-interpretacion-parcial.md)
* [OBS-0018 — La ausencia de software previo no implica ausencia de conocimiento estructurado](../observations/obs-0018-ausencia-software-previo-no-implica-ausencia-conocimiento-estructurado.md)
* [OBS-0019 — El conocimiento puede escaparse cuando se modela solo lo que las personas dicen hacer y no lo que realmente hacen](../observations/obs-0019-conocimiento-escapa-modelar-dicho-no-practica-real.md)

## Tensiones relacionadas

* [TNS-0009 — Rapidez de digitalización vs profundidad de descubrimiento](../tensions/tns-0009-rapidez-digitalizacion-vs-profundidad-descubrimiento.md)
* [TNS-0010 — Procedimiento visible vs criterio tácito](../tensions/tns-0010-procedimiento-visible-vs-criterio-tacito.md)
* [TNS-0011 — Automatizar práctica actual vs descubrir necesidad real](../tensions/tns-0011-automatizar-practica-actual-vs-descubrir-necesidad-real.md)
* [TNS-0012 — Formalizar temprano vs mantener ambigüedad exploratoria](../tensions/tns-0012-formalizar-temprano-vs-mantener-ambiguedad-exploratoria.md)

## Evidencia

La evidencia disponible proviene de observaciones prácticas y exploratorias en contextos donde no existe software especializado previo o donde la digitalización todavía no ha ocurrido de forma suficiente.

La evidencia puede formularse en términos generales:

* Se observa que algunos contextos operan sin software especializado previo.
* Se observa que la ausencia de software no implica ausencia de conocimiento estructurado.
* Se observa que parte del conocimiento relevante puede estar embebido en prácticas cotidianas.
* Se observa que las personas pueden describir procedimientos visibles sin explicitar todos los criterios usados para decidir.
* Se observa que algunas diferencias entre lo declarado y lo practicado solo aparecen durante la ejecución real.
* Se observa que una primera digitalización puede capturar categorías visibles, pero omitir conocimiento tácito relevante.
* Se observa que formalizar temprano puede ayudar a construir, pero también puede congelar una interpretación parcial del dominio.
* Se observa que automatizar la práctica actual puede preservar conocimiento útil, pero también puede estabilizar restricciones o workarounds que deberían revisarse.

Esta evidencia permite formular un finding candidato, pero no constituye validación fuerte ni generalizable.

## Interpretación

El problema observado no es simplemente que no exista software.

La interpretación inicial es que, antes de la digitalización, el conocimiento puede existir en formas no documentales, no técnicas y no formalizadas.

Puede estar situado en:

* prácticas cotidianas
* criterios tácitos
* decisiones locales
* excepciones conocidas
* rutinas manuales
* categorías usadas por las personas
* lenguaje cotidiano
* memoria operativa
* objetos físicos
* espacios de trabajo
* acuerdos informales
* diferencias entre lo que se declara y lo que se hace

Cuando una digitalización inicial captura solo procedimientos visibles, campos evidentes o necesidades declaradas, puede dejar fuera conocimiento necesario para entender correctamente el dominio.

En ese escenario, el conocimiento no desaparece después de construir software.

Se escapa antes o durante la primera traducción del dominio hacia artifacts, modelos o estructuras digitales.

## Alcance

Este finding aplica, de forma inicial y prudente, a contextos donde:

* no existe software especializado previo
* la operación depende de prácticas manuales o informales
* parte del conocimiento relevante no está documentado
* las personas usan criterios prácticos no siempre verbalizados
* la primera digitalización define categorías, campos o flujos iniciales
* el descubrimiento se basa principalmente en procedimientos declarados
* existen diferencias posibles entre práctica actual y necesidad real
* existe riesgo de formalizar demasiado temprano una comprensión parcial

Este finding tiene valor principalmente fundacional y comparativo: amplía `RQ-001` mostrando que la continuidad no solo puede romperse después de que el software existe, sino también antes, cuando el conocimiento del dominio no alcanza a ser descubierto suficientemente.

## Relación con VSlices

Este finding ayuda a ampliar el problema fundacional de VSlices Research.

VSlices no solo debería estudiar continuidad en sistemas legacy, ecosistemas activos o transiciones de personas clave.

También debería estudiar cómo se preserva o se pierde continuidad durante la digitalización inicial de contextos no digitalizados.

Desde este finding, VSlices Research puede investigar posteriormente si mecanismos como discovery progresivo, documentation slices, context documents, continuity paths, notas de supuestos, registros de incertidumbre, behavior documents o validación por uso real ayudan a evitar que el conocimiento tácito se escape durante la primera digitalización.

Pero esa evaluación todavía no corresponde a este finding.

Este documento no propone una solución de VSlices.

Solo identifica un escenario donde la continuidad puede romperse o debilitarse antes de que el software exista.

## Relación con FND-0001, FND-0002 y FND-0003

Este finding complementa a:

* [FND-0001 — La pérdida de continuidad de conocimiento dificulta mantener, evolucionar y validar sistemas de software](../findings/fnd-0001-perdida-continuidad-dificulta-evolucion-validacion.md)
* [FND-0002 — La continuidad de conocimiento puede romperse por dispersión activa entre contextos locales](../findings/fnd-0002-continuidad-rota-por-dispersion-activa.md)
* [FND-0003 — La continuidad de conocimiento puede romperse cuando conocimiento crítico permanece concentrado en una persona clave durante una transición](../findings/fnd-0003-continuidad-rota-por-concentracion-persona-clave.md)

FND-0001 observa una forma de ruptura asociada a pérdida histórica, redescubrimiento y dificultad para evolucionar sistemas longevos.

FND-0002 observa una forma de ruptura asociada a dispersión activa, conocimiento local y falta de vista transversal.

FND-0003 observa una forma de ruptura potencial asociada a concentración personal de conocimiento durante una transición.

FND-0004 observa una forma de ruptura o escape anterior al software, asociada a conocimiento tácito no suficientemente explorado durante la digitalización inicial.

En conjunto, estos findings pueden alimentar una distinción inicial:

* pérdida histórica de continuidad: el conocimiento existió, pero dejó de estar disponible, trazable o compartido
* dispersión activa de continuidad: el conocimiento existe, pero está fragmentado entre contextos locales sin conexión suficiente
* concentración personal de continuidad: el conocimiento existe, pero está demasiado acoplado a una persona clave
* escape inicial de continuidad: el conocimiento existe en la práctica, pero no alcanza a ser descubierto o preservado durante la digitalización inicial

Esta distinción todavía debe tratarse como candidata.

No debe convertirse en taxonomía oficial hasta observar más casos, revisar contra evidencia adicional y contrastar sus límites.

## Límites

Este finding no demuestra que toda digitalización inicial produzca escape de conocimiento.

Tampoco demuestra que todo conocimiento tácito deba explicitarse, documentarse o digitalizarse.

En algunos contextos, una digitalización rápida y simple puede ser suficiente para reducir dolor inmediato y aprender desde el uso real.

Este finding tampoco demuestra que la práctica actual deba preservarse completa.

Parte de la práctica actual puede ser valiosa, pero otra parte puede ser accidental, ineficiente, heredada o producto de restricciones que el software podría ayudar a superar.

La evidencia disponible es exploratoria, parcial y no necesariamente documentable con artifacts públicos. Por lo tanto, este finding debe tratarse como fundacional y candidato, no como validado.

## Riesgos de interpretación

* Asumir que todo contexto no digitalizado es caótico o inmaduro.
* Confundir ausencia de software con ausencia de conocimiento.
* Tratar la primera entrevista como representación completa del dominio.
* Modelar solo lo que las personas dicen hacer y no contrastarlo con la práctica real.
* Automatizar workarounds sin descubrir la necesidad que los originó.
* Convertir categorías iniciales en estructura permanente demasiado pronto.
* Intentar capturar todo conocimiento tácito antes de construir algo útil.
* Usar el finding para justificar análisis indefinido.
* Usar el finding para afirmar que VSlices resuelve este problema sin validación.
* Confundir descubrimiento suficiente con documentación exhaustiva.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Próxima evidencia necesaria

Para fortalecer, refinar o descartar este finding, VSlices Research necesita evidencia adicional y documentable.

Evidencia deseable:

* Casos documentables donde se digitalice por primera vez un contexto no digitalizado.
* Casos donde la primera digitalización capture conocimiento tácito relevante.
* Casos donde la primera digitalización omita conocimiento tácito relevante.
* Casos donde observar la práctica revele conocimiento que no aparece en entrevistas iniciales.
* Casos donde una categoría inicial congele una interpretación parcial del dominio.
* Casos donde una formalización provisional permita avanzar sin cerrar preguntas.
* Casos donde automatizar la práctica actual preserve workarounds innecesarios.
* Casos donde descubrir la necesidad real permita simplificar la solución.
* Evidencia sobre cómo distinguir conocimiento tácito crítico de conocimiento situado que puede permanecer implícito.
* Evidencia sobre cómo validar que una primera digitalización preservó suficiente continuidad.
* Casos donde mecanismos de VSlices ayuden a explorar conocimiento tácito sin introducir burocracia.
* Casos donde mecanismos de VSlices agreguen ceremonia sin mejorar descubrimiento ni continuidad.

## Estado de madurez

Este finding debe permanecer como `candidate`.

Puede alimentar `RQ-001` y orientar estudios futuros, pero no debe convertirse todavía en principio oficial, patrón adoptado o decisión de producto.

Su función actual es fundacional:

> ayuda a ampliar el problema práctico que VSlices Research debe investigar, mostrando que la continuidad puede romperse antes de existir software cuando conocimiento tácito de un contexto no digitalizado no es explorado suficientemente.
