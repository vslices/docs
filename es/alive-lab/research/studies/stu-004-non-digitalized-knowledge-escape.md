---
type: study
state: observed
mode: retrospective
code: STU-004
case: non-digitalized-knowledge-escape
title: Riesgo de escape de conocimiento en contextos no digitalizados

related_questions:
* RQ-001

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

restrictions:
* no personal household details if used from domestic cases
* no private routines unless intentionally anonymized
* no sensitive operational details
* no identifiable people
* no assumptions presented as validated findings

evidence:
  level: exploratory-observed
  artifacts_available: partial
  source: practical observation and Alive Lab cases
-------------------------------------------------

# Study — Riesgo de escape de conocimiento en contextos no digitalizados

## Tipo

study

## Estado

observed

## Caso

Contexto no digitalizado — riesgo de escape de conocimiento durante descubrimiento y digitalización inicial

## Modo de observación

retrospective

## Preguntas relacionadas

* [RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Contexto

Este study registra un escenario distinto a los casos donde ya existe software o donde ya existe una organización con conocimiento distribuido alrededor de sistemas activos.

En contextos no digitalizados, el conocimiento relevante todavía puede vivir en prácticas cotidianas, conversaciones, memoria operativa, rutinas manuales, criterios tácitos, excepciones informales, acuerdos locales, hojas sueltas, mensajes, documentos parciales o experiencia acumulada de las personas que ejecutan el trabajo.

El problema observado no es que el conocimiento esté perdido.

Tampoco es necesariamente que esté disperso entre sistemas existentes.

El problema es que parte del conocimiento todavía no ha sido explorado, explicitado, modelado ni convertido en artifact compartido.

Cuando se inicia una digitalización, existe el riesgo de que solo una parte visible del dominio sea capturada. Otra parte puede escaparse porque no aparece en entrevistas iniciales, no está escrita, parece demasiado obvia para quienes la ejecutan, o solo se revela cuando ocurre una excepción real.

La digitalización inicial puede transformar una comprensión parcial del dominio en software, dejando fuera conocimiento relevante que seguía existiendo en la práctica.

## Problema observado

En un contexto no digitalizado, la ausencia de software previo no implica ausencia de conocimiento.

El conocimiento puede estar presente, pero no necesariamente en forma de documentos, modelos, reglas explícitas o procesos formalizados.

Puede existir como:

* criterio práctico
* memoria de casos anteriores
* hábitos de operación
* excepciones conocidas por experiencia
* secuencias de trabajo no escritas
* prioridades implícitas
* formas locales de clasificar información
* acuerdos entre personas
* señales usadas para decidir
* diferencias entre lo que se dice hacer y lo que realmente se hace
* restricciones materiales, temporales o sociales del contexto
* conocimiento distribuido en objetos, espacios, herramientas o rutinas

El riesgo aparece cuando un proceso de digitalización intenta capturar el dominio únicamente desde procedimientos declarados, necesidades visibles o categorías iniciales.

En ese caso, el software puede nacer representando una versión demasiado limpia, parcial o prematuramente formalizada del contexto real.

## Alcance del estudio

Este study observa el riesgo de escape de conocimiento durante la digitalización inicial de contextos que no cuentan con software previo suficientemente estructurado.

El foco está en entender cómo puede perderse continuidad antes de que exista un sistema digital, cuando el conocimiento del dominio no alcanza a ser descubierto o preservado durante las primeras decisiones de modelado.

El study busca observar:

* qué conocimiento existe antes de digitalizar
* qué conocimiento está explícito
* qué conocimiento permanece tácito
* qué prácticas reales no aparecen en descripciones iniciales
* qué criterios se usan para decidir en la práctica
* qué excepciones aparecen solo durante el uso real
* qué categorías iniciales pueden congelar una interpretación parcial
* qué conocimiento puede escaparse durante el levantamiento
* qué riesgos aparecen al automatizar antes de comprender suficiente

Este study no busca proponer todavía cómo VSlices debería resolver el problema.

El objetivo inicial es registrar el escenario de pérdida o escape de continuidad.

## Fuera de alcance

Este study no busca documentar exhaustivamente un dominio no digitalizado completo.

Tampoco busca evaluar la calidad de las personas, prácticas o rutinas existentes.

No documenta:

* datos personales sensibles
* detalles privados de hogares o personas
* flujos internos identificables sin anonimización
* reglas confidenciales de organizaciones
* información operacional no autorizada
* nombres de personas involucradas
* casos privados que no deban convertirse en evidencia
* interpretaciones no observadas como si fueran findings

El objetivo no es convertir toda práctica humana en software.

El objetivo es observar cómo parte del conocimiento puede escaparse cuando todavía no ha sido explorado, explicitado o conectado.

## Evidencia disponible

La evidencia disponible corresponde a observaciones prácticas y exploratorias en contextos donde la digitalización aparece como una intención inicial, no como una evolución de software existente.

La evidencia puede formularse en términos generales:

* Se observa que ciertos contextos operan sin software especializado previo.
* Se observa que la operación puede depender de rutinas, memoria, criterios y acuerdos tácitos.
* Se observa que las personas pueden describir procedimientos visibles, pero no siempre explicitar criterios usados para decidir.
* Se observa que ciertas excepciones solo aparecen durante la ejecución real.
* Se observa que una primera estructura digital puede capturar categorías visibles, pero omitir matices del uso real.
* Se observa que digitalizar temprano puede congelar una interpretación inicial del dominio.
* Se observa que el conocimiento puede escaparse no porque haya desaparecido, sino porque nunca fue capturado.

La evidencia disponible es parcial y exploratoria.

Por esta razón, debe tratarse como evidencia inicial, no como validación fuerte.

## Observaciones candidatas producidas

* [OBS-0015 — En contextos no digitalizados, el conocimiento relevante puede estar embebido en prácticas cotidianas y no existir como artifact explícito.](../observations/obs-0015-conocimiento-embebido-practicas-cotidianas.md)
* [OBS-0016 — El levantamiento inicial puede capturar procedimientos visibles, pero omitir criterios tácitos usados para decidir.](../observations/obs-0016-levantamiento-captura-procedimientos-visibles-omite-criterios-tacitos.md)
* [OBS-0017 — Digitalizar un proceso no explorado puede congelar una interpretación parcial del dominio.](../observations/obs-0017-digitalizar-proceso-no-explorado-congela-interpretacion-parcial.md)
* [OBS-0018 — La ausencia de software previo no implica ausencia de conocimiento estructurado.](../observations/obs-0018-ausencia-software-previo-no-implica-ausencia-conocimiento-estructurado.md)
* [OBS-0019 — El conocimiento puede escaparse cuando se modela solo lo que las personas dicen hacer y no lo que realmente hacen.](../observations/obs-0019-conocimiento-escapa-modelar-dicho-no-practica-real.md)

## Tensiones candidatas producidas

* [TNS-0009 — Rapidez de digitalización vs profundidad de descubrimiento.](../tensions/tns-0009-rapidez-digitalizacion-vs-profundidad-descubrimiento.md)
* [TNS-0010 — Procedimiento visible vs criterio tácito.](../tensions/tns-0010-procedimiento-visible-vs-criterio-tacito.md)
* [TNS-0011 — Automatizar práctica actual vs descubrir necesidad real.](../tensions/tns-0011-automatizar-practica-actual-vs-descubrir-necesidad-real.md)
* [TNS-0012 — Formalizar temprano vs mantener ambigüedad exploratoria.](../tensions/tns-0012-formalizar-temprano-vs-mantener-ambiguedad-exploratoria.md)

## Finding candidato producido

* [FND-0004 — La continuidad de conocimiento puede romperse antes de existir software cuando el conocimiento tácito de un contexto no digitalizado no es explorado suficientemente.](../findings/fnd-0004-continuidad-rota-antes-software-conocimiento-tacito-no-explorado.md)

## Interpretación inicial

Esta experiencia sugiere que la continuidad de conocimiento puede romperse antes de que exista un sistema de software.

En este escenario, el problema no aparece después de años de evolución, ni por dispersión entre servicios, ni por concentración en una persona clave.

El problema aparece durante el descubrimiento inicial.

El conocimiento existe en la práctica, pero puede no llegar al software porque no fue observado, preguntado, contrastado, modelado o preservado.

Esto permite distinguir una cuarta forma inicial de ruptura o escape de continuidad:

* pérdida histórica de continuidad: el conocimiento existió, pero dejó de estar disponible, trazable o compartido
* dispersión activa de continuidad: el conocimiento existe, pero está fragmentado entre contextos locales sin conexión suficiente
* concentración personal de continuidad: el conocimiento existe, pero está demasiado acoplado a una persona clave
* escape inicial de continuidad: el conocimiento existe en la práctica, pero no alcanza a ser descubierto o preservado durante la digitalización inicial

Esta distinción debe tratarse todavía como candidata.

No debe convertirse en taxonomía oficial hasta contar con más evidencia, revisión y contraste entre casos.

## Relación con VSlices Research

Este study ayuda a ampliar el problema fundacional de VSlices Research.

Hasta ahora, los estudios iniciales observan escenarios donde existe o existió software:

* sistemas legacy con conocimiento perdido
* sistemas activos con conocimiento disperso
* sistemas en transición con conocimiento concentrado

Este study agrega un escenario previo:

> contextos donde todavía no existe software especializado, pero sí existe conocimiento práctico que puede escaparse si no se descubre suficientemente antes o durante la digitalización.

Desde este study, VSlices Research puede observar cómo se preserva o pierde continuidad entre práctica real, descubrimiento del dominio, primeras categorías documentales, decisiones de modelado y eventual implementación.

La pregunta no es todavía cómo VSlices debería abordar el problema.

La pregunta inicial es:

> ¿Qué conocimiento puede escaparse antes de que el software exista?

## Relación con estudios anteriores

Este study complementa a:

* [Study — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem.md)
* [Study — Dispersión de conocimiento en un ecosistema asegurador empresarial](../studies/stu-002-insurance-knowledge-dispersion.md)
* [Study — Riesgo de pérdida de conocimiento por salida de una persona clave](../studies/stu-003-key-person-knowledge-transition.md)

STU-001 observa una ruptura de continuidad asociada a pérdida histórica y necesidad de redescubrimiento.

STU-002 observa una ruptura de continuidad asociada a conocimiento activo pero disperso entre contextos locales.

STU-003 observa una ruptura potencial asociada a conocimiento activo pero concentrado en una persona clave durante una transición.

STU-004 observa una ruptura potencial anterior al software, asociada a conocimiento práctico que no alcanza a ser descubierto o preservado durante la digitalización inicial.

En conjunto, estos estudios podrían alimentar una síntesis futura sobre escenarios iniciales de pérdida, debilitamiento o escape de continuidad de conocimiento.

Esa síntesis todavía no debe escribirse como conclusión estable.

## Límites

Este study tiene límites importantes:

* Es exploratorio.
* No está basado todavía en un estudio formal diseñado desde el inicio.
* Puede apoyarse en observaciones prácticas, pero requiere evidencia más concreta.
* No demuestra que toda digitalización inicial pierda conocimiento.
* No demuestra que todo conocimiento tácito deba ser explicitado.
* No demuestra que digitalizar temprano sea necesariamente incorrecto.
* No demuestra que una exploración profunda siempre sea mejor que una intervención rápida.
* No valida todavía qué mecanismos permitirían capturar conocimiento sin introducir burocracia.
* No valida todavía que VSlices resuelva este tipo de escape de conocimiento.

Su valor principal es fundacional y comparativo: permite observar una forma distinta de riesgo de continuidad, basada en conocimiento no explorado antes o durante la digitalización inicial.

## Notas de confidencialidad

Este study puede documentarse como evidencia exploratoria y anonimizada.

Si se usa un caso doméstico, organizacional o profesional como fuente, no deben incluirse detalles personales, privados, sensibles, propietarios o identificables que no sean necesarios para formular el problema general.

La experiencia puede usarse para formular preguntas, hipótesis, observaciones, tensiones y findings fundacionales, pero no debe presentarse como validación formal mientras no exista evidencia suficiente.

Su función es abrir investigación, no cerrar conclusiones.

## Próxima evidencia necesaria

Para fortalecer esta línea de investigación, VSlices Research necesita observar y formalizar evidencia adicional.

Evidencia futura deseable:

* casos donde un proceso no digitalizado haya sido digitalizado por primera vez
* ejemplos donde la digitalización inicial omitió criterios tácitos relevantes
* ejemplos donde se capturó solo el procedimiento visible, pero no las decisiones reales
* ejemplos donde una primera categoría digital congeló una interpretación parcial del dominio
* casos donde observar la práctica real reveló conocimiento que no aparecía en entrevistas
* casos donde mantener ambigüedad exploratoria ayudó a evitar formalización prematura
* casos donde explorar demasiado retrasó innecesariamente la entrega de valor
* evidencia sobre qué conocimiento tácito debe explicitarse y cuál puede permanecer situado
* evidencia sobre cómo distinguir práctica actual, necesidad real y oportunidad de automatización
* observaciones sobre cómo documentar descubrimiento inicial sin convertirlo en burocracia
