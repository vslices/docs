# RQ-001 — Problema fundacional de VSlices Research

## Pregunta

¿Qué problema práctico de la ingeniería de software dio origen a VSlices, y cómo puede transformarse ese problema en una línea de investigación aplicada sobre continuidad de conocimiento sin perder su raíz práctica?

## Estado

candidate

## Origen

VSlices nació primero como un proyecto de software y como una respuesta práctica a problemas observados en ingeniería de software, antes de ser formulado como objeto de investigación.

La suite se define como una iniciativa enfocada en preservar continuidad entre descubrimiento de dominio, documentación, arquitectura, implementación y evolución.

Esta pregunta existe para reconstruir ese problema fundacional sin convertir retrospectivamente a VSlices en una teoría cerrada desde su origen.

Después de los primeros studies de VSlices Research, esta pregunta se refina para observar no solo pérdida de continuidad en sistemas existentes, sino también ruptura, debilitamiento, dispersión, concentración o escape de conocimiento en distintos momentos del ciclo de vida de un dominio o sistema.

## Problema observado

En proyectos de software, es común que el conocimiento se fragmente entre lo que se descubre del dominio, lo que se documenta, lo que se diseña, lo que se implementa y lo que posteriormente evoluciona.

Esta fragmentación puede producir:

* pérdida de intención arquitectónica
* documentación desconectada del código
* decisiones difíciles de rastrear
* lenguaje de dominio inconsistente
* flujos de negocio comprendidos solo de forma parcial
* dificultad para validar necesidades de auditoría o cumplimiento
* arquitectura que deja de reflejar el problema original
* miedo a modificar sistemas que siguen operando, pero ya no son comprendidos suficientemente

Sin embargo, la evidencia inicial sugiere que la pérdida de continuidad no ocurre solo en sistemas legacy o durante mantenimiento posterior.

La continuidad de conocimiento también puede verse comprometida cuando:

* el conocimiento existió, pero se perdió históricamente o dejó de estar disponible de forma suficiente
* el conocimiento existe y está activo, pero permanece disperso entre contextos locales
* el conocimiento existe y está activo, pero permanece concentrado en una persona clave
* el conocimiento existe en la práctica, pero se escapa antes o durante una digitalización inicial

Por lo tanto, el problema fundacional no es solamente la pérdida de documentación o la degradación de sistemas antiguos.

El problema más amplio es cómo preservar continuidad de conocimiento entre práctica, dominio, decisiones, documentación, arquitectura, implementación, operación, evolución y transición.

## Hipótesis inicial

VSlices surge desde la hipótesis práctica de que preservar continuidad entre dominio, documentación, arquitectura, implementación y evolución puede reducir fragmentación conceptual y mejorar la trazabilidad de decisiones en proyectos de software.

Esta hipótesis no debe tratarse todavía como validada.

Su función inicial es orientar investigación aplicada sobre cuándo la continuidad se pierde, se debilita, se dispersa, se concentra o se escapa, qué consecuencias produce y qué mecanismos podrían ayudar a preservarla sin introducir burocracia innecesaria.

Después de los primeros studies, la hipótesis puede formularse de manera más precisa:

> Si la continuidad de conocimiento se rompe en distintos momentos del ciclo de vida de un dominio o sistema, entonces VSlices Research debe estudiar no solo cómo preservar documentación, sino cómo preservar relaciones entre conocimiento práctico, decisiones, comportamiento, arquitectura, implementación y evolución.

Esta formulación sigue siendo candidata.

No demuestra todavía que VSlices resuelva el problema.

## Qué busca observar esta pregunta

Esta pregunta busca reconstruir el problema práctico que hizo necesario a VSlices antes de estudiar mecanismos específicos como continuity paths, documentación mínima, behavior documents, context documents, tooling documental o coordinación entre líneas paralelas.

Busca responder, de forma progresiva:

* dónde se rompe la continuidad en proyectos de software
* dónde puede escaparse la continuidad antes de que exista software
* qué tipos de conocimiento se pierden, dispersan, concentran u omiten
* qué consecuencias produce esa pérdida, dispersión, concentración u omisión
* qué mecanismos de VSlices intentan responder a ese problema
* qué parte de VSlices nació como respuesta práctica
* qué parte sigue siendo intuición no validada
* qué límites tiene la hipótesis de continuidad

También busca observar si distintos escenarios de ruptura requieren respuestas distintas.

Por ejemplo:

* sistemas legacy pueden requerir reconstrucción de conocimiento perdido
* ecosistemas activos pueden requerir continuidad transversal
* transiciones de personas clave pueden requerir transferencia suficiente
* contextos no digitalizados pueden requerir descubrimiento progresivo antes de formalizar

## Preguntas derivadas

* ¿Dónde se rompe normalmente la continuidad en un proyecto de software?
* ¿Dónde puede escaparse la continuidad antes de que exista software?
* ¿Qué evidencia práctica originó la necesidad de VSlices?
* ¿Qué tipos de conocimiento se pierden primero: dominio, flujo, arquitectura, decisiones, comportamiento, operación o implementación?
* ¿Qué ocurre cuando un sistema sigue funcionando, pero ya no existe comprensión compartida sobre lo que hace?
* ¿Qué ocurre cuando el conocimiento está activo, pero disperso entre productos, equipos, servicios o contextos locales?
* ¿Qué ocurre cuando el conocimiento crítico está activo, pero concentrado en una persona clave?
* ¿Qué ocurre cuando un contexto no digitalizado contiene conocimiento tácito que no alcanza a ser explorado antes de digitalizar?
* ¿Qué partes de VSlices fueron respuesta directa a estos problemas?
* ¿Qué partes pueden ser intuición no validada todavía?
* ¿Qué mecanismos actuales de VSlices intentan preservar continuidad?
* ¿Qué límites tiene esta hipótesis?
* ¿Qué señales permiten distinguir pérdida histórica, dispersión activa, concentración personal y escape inicial de continuidad?
* ¿Qué mecanismos ayudan en un escenario, pero podrían agregar ceremonia innecesaria en otro?

## Studies relacionados

* [STU-001 — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem.md)
* [STU-002 — Dispersión de conocimiento en un ecosistema asegurador empresarial](../studies/stu-002-insurance-knowledge-dispersion.md)
* [STU-003 — Riesgo de pérdida de conocimiento por salida de una persona clave](../studies/stu-003-key-person-knowledge-transition.md)
* [STU-004 — Riesgo de escape de conocimiento en contextos no digitalizados](../studies/stu-004-non-digitalized-knowledge-escape.md)

## Findings relacionados

* [FND-0001 — La pérdida de continuidad de conocimiento dificulta mantener, evolucionar y validar sistemas de software](../findings/fnd-0001-perdida-continuidad-dificulta-evolucion-validacion.md)
* [FND-0002 — La continuidad de conocimiento puede romperse por dispersión activa entre contextos locales](../findings/fnd-0002-continuidad-rota-por-dispersion-activa.md)
* [FND-0003 — La continuidad de conocimiento puede romperse cuando conocimiento crítico permanece concentrado en una persona clave durante una transición](../findings/fnd-0003-continuidad-rota-por-concentracion-persona-clave.md)
* [FND-0004 — La continuidad de conocimiento puede romperse antes de existir software cuando el conocimiento tácito de un contexto no digitalizado no es explorado suficientemente](../findings/fnd-0004-continuidad-rota-antes-software-conocimiento-tacito-no-explorado.md)

## Síntesis inicial relacionada

La primera síntesis candidata de esta pregunta es:

* [SYN-0001 — Escenarios iniciales de ruptura o escape de continuidad de conocimiento](../synthesis/syn-0001-escenarios-iniciales-ruptura-escape-continuidad-conocimiento.md)

Esta síntesis propone que la continuidad de conocimiento puede verse comprometida en al menos cuatro escenarios iniciales:

* pérdida histórica de continuidad
* dispersión activa de continuidad
* concentración personal de continuidad
* escape inicial de continuidad

Esta distinción todavía es candidata.

No debe tratarse como taxonomía oficial, principio adoptado ni decisión de producto.

## Evidencia inicial disponible

* Definición de VSlices como suite enfocada en continuidad entre dominio, documentación, arquitectura, implementación y evolución.
* Regla de evolución de producto: las ideas deben surgir desde problemas reales y evidencia antes de convertirse en parte oficial de la suite.
* Alive Lab existe como espacio para validar ideas antes de formalizarlas como parte de VSlices.
* Experiencia profesional retrospectiva y restringida en sistemas empresariales longevos donde la pérdida de continuidad de conocimiento dificultó la comprensión, renovación y evolución segura del software.
* Experiencia profesional restringida y actual donde el conocimiento permanece activo, pero puede estar disperso entre productos, líneas de negocio, servicios o contextos locales.
* Experiencia profesional restringida y actual donde conocimiento crítico puede permanecer concentrado en una persona clave durante una transición.
* Observaciones exploratorias en contextos no digitalizados donde conocimiento tácito puede existir en la práctica, pero escaparse durante una digitalización inicial.
* Observación general de que un sistema puede seguir funcionando operativamente mientras se pierde conocimiento compartido sobre dominio, flujos, decisiones e intención original.
* Observación general de que renovar un sistema legacy puede requerir reconstruir conocimiento antes de intervenir técnicamente.
* Observación general de que conocimiento activo no garantiza continuidad transversal.
* Observación general de que conocimiento disponible en una persona no garantiza continuidad distribuida.
* Observación general de que ausencia de software previo no implica ausencia de conocimiento estructurado.

## Evidencia retrospectiva restringida

La formulación inicial de esta pregunta está influenciada por experiencia profesional previa en sistemas empresariales longevos, donde se observó que la pérdida de continuidad entre conocimiento de dominio, flujos operacionales, decisiones del sistema y software existente puede dificultar la renovación segura de una plataforma.

Por razones de confidencialidad, esta evidencia no se documenta con información interna, propietaria, operacional o identificable de la organización.

La evidencia se usa únicamente para formular el problema general de investigación:

> sistemas que siguen funcionando pueden perder conocimiento compartido sobre qué hacen, por qué lo hacen, cómo se conectan sus flujos y qué necesidades originales siguen cumpliendo.

Esta experiencia no valida por sí sola a VSlices.

Sí ayuda a justificar que el problema de pérdida de continuidad existe como preocupación práctica y merece ser investigado mediante casos observables, documentables y permitidos dentro de Alive Lab.

## Evidencia restringida actual

La pregunta también se apoya en experiencias profesionales actuales con límites de confidencialidad, donde se observan riesgos de continuidad asociados a:

* conocimiento activo pero disperso entre contextos locales
* conceptos similares con nombres diferentes según el contexto
* servicios o soluciones especializadas que pueden ocultar duplicación conceptual
* conocimiento crítico concentrado en una persona clave
* riesgo de pérdida de continuidad durante transición, salida o cambio de rol

Por razones éticas y profesionales, estas experiencias no deben documentarse con detalles identificables de organizaciones, sistemas, servicios, flujos, decisiones internas, equipos o personas.

Pueden usarse para formular observaciones, tensiones y findings candidatos, pero no deben tratarse como validación fuerte o generalizable.

## Evidencia exploratoria desde contextos no digitalizados

La pregunta también se apoya en observaciones exploratorias sobre contextos donde no existe software especializado previo o donde la digitalización todavía no ha ocurrido de forma suficiente.

En estos casos, se observa que el conocimiento puede existir en:

* prácticas cotidianas
* criterios tácitos
* memoria operativa
* acuerdos informales
* objetos físicos
* espacios de trabajo
* clasificación local
* diferencias entre lo que se dice hacer y lo que realmente se hace

Esta evidencia permite ampliar RQ-001 para incluir escenarios donde la continuidad puede escaparse antes de que exista software.

No demuestra que toda digitalización inicial pierda conocimiento.

No demuestra que todo conocimiento tácito deba explicitarse.

Solo justifica investigar cómo una primera digitalización puede capturar, omitir o congelar conocimiento del dominio.

## Evidencia no documentable

Por límites éticos, profesionales y de confidencialidad, no deben documentarse detalles internos de organizaciones, sistemas, flujos, módulos, decisiones técnicas, procesos operacionales o información propietaria observados durante experiencia profesional previa o actual.

Esta evidencia puede inspirar preguntas, hipótesis, observations, tensions o findings fundacionales, pero no debe usarse como validación fuerte ni como caso de estudio detallado cuando no exista autorización o forma segura de anonimización.

## Evidencia faltante

* Casos documentables y permitidos donde la continuidad se haya roto.
* Casos documentables donde la continuidad se haya preservado de forma suficiente.
* Ejemplos públicos o propios donde pueda describirse el problema sin restricciones de confidencialidad.
* Ejemplos donde VSlices haya ayudado a preservar continuidad.
* Ejemplos donde VSlices haya agregado ceremonia sin suficiente valor.
* Comparación entre proyectos con y sin mecanismos explícitos de continuidad.
* Observación de casos actuales en Alive Lab donde VSlices intente preservar continuidad desde etapas tempranas.
* Evidencia sobre qué tipos de conocimiento se pierden primero durante la evolución de un sistema.
* Evidencia sobre qué tipos de conocimiento se dispersan entre contextos activos.
* Evidencia sobre qué conocimiento se concentra en personas clave y cómo se transfiere de forma suficiente.
* Evidencia sobre qué conocimiento tácito se escapa durante digitalización inicial.
* Evidencia sobre qué mecanismos ayudan realmente a recuperar o preservar continuidad.
* Evidencia sobre qué mecanismos ayudan en un escenario, pero agregan ruido en otro.
* Evidencia sobre cómo validar que la continuidad fue preservada, no solo documentada.

## Riesgos metodológicos

* Convertir el origen de VSlices en relato mítico.
* Asumir que toda fragmentación se resuelve con VSlices.
* Confundir intuiciones fundacionales con hallazgos validados.
* Usar experiencia retrospectiva restringida como si fuera evidencia formal completa.
* Usar experiencia actual restringida como si fuera evidencia generalizable.
* Confundir pérdida de documentación con pérdida de continuidad completa.
* Asumir que más documentación resolvería automáticamente el problema.
* Convertir la síntesis inicial en taxonomía oficial demasiado pronto.
* Tratar pérdida histórica, dispersión activa, concentración personal y escape inicial como categorías cerradas.
* Ignorar que los escenarios pueden solaparse.
* Adoptar mecanismos antes de probarlos en Alive Lab.
* Diseñar mecanismos demasiado pesados para prevenir un problema real pero variable.
* Usar RQ-001 para justificar VSlices antes de validar sus mecanismos.
* Confundir preservar continuidad con preservar todo conocimiento, toda práctica o toda decisión.

## Límite actual

Esta pregunta no demuestra que VSlices resuelve la fragmentación, pérdida, dispersión, concentración o escape de conocimiento en proyectos de software.

Solo establece el problema fundacional que VSlices Research debe investigar.

La evidencia disponible permite formular una primera explicación candidata sobre escenarios de ruptura o escape de continuidad, pero no validarla de forma general.

La síntesis `SYN-0001` ayuda a ordenar los primeros cuatro escenarios observados, pero todavía debe permanecer como candidata.

Para avanzar, esta pregunta necesita nuevos casos documentables, observaciones actuales y estudios dentro de Alive Lab que permitan distinguir entre intuición fundacional, evidencia observada, findings locales, synthesis candidatas y posibles decisiones de producto.
