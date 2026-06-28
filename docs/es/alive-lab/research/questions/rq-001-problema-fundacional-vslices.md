# RQ-001 — Problema fundacional de VSlices Research

## Pregunta

¿Qué problema práctico de la ingeniería de software dio origen a VSlices, y cómo puede transformarse ese problema en una línea de investigación aplicada sin perder su raíz práctica?

## Estado

candidate

## Origen

VSlices nació primero como un proyecto de software y como una respuesta práctica a problemas observados en ingeniería de software, antes de ser formulado como objeto de investigación.

La suite se define como una iniciativa enfocada en preservar continuidad entre descubrimiento de dominio, documentación, arquitectura, implementación y evolución.

Esta pregunta existe para reconstruir ese problema fundacional sin convertir retrospectivamente a VSlices en una teoría cerrada desde su origen.

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

## Hipótesis inicial

VSlices surge desde la hipótesis práctica de que preservar continuidad entre dominio, documentación, arquitectura, implementación y evolución puede reducir fragmentación conceptual y mejorar la trazabilidad de decisiones en proyectos de software.

Esta hipótesis no debe tratarse todavía como validada.

Su función inicial es orientar investigación aplicada sobre cuándo la continuidad se pierde, qué consecuencias produce y qué mecanismos podrían ayudar a preservarla sin introducir burocracia innecesaria.

## Qué busca observar esta pregunta

Esta pregunta busca reconstruir el problema práctico que hizo necesario a VSlices antes de estudiar mecanismos específicos como continuity paths, documentación mínima o coordinación entre líneas paralelas.

Busca responder, de forma progresiva:

* dónde se rompe la continuidad en proyectos de software
* qué tipos de conocimiento se pierden durante la evolución de un sistema
* qué consecuencias produce esa pérdida
* qué mecanismos de VSlices intentan responder a ese problema
* qué parte de VSlices nació como respuesta práctica
* qué parte sigue siendo intuición no validada
* qué límites tiene la hipótesis de continuidad

## Preguntas derivadas

* ¿Dónde se rompe normalmente la continuidad en un proyecto de software?
* ¿Qué evidencia práctica originó la necesidad de VSlices?
* ¿Qué tipos de conocimiento se pierden primero: dominio, flujo, arquitectura, decisiones, comportamiento o implementación?
* ¿Qué ocurre cuando un sistema sigue funcionando, pero ya no existe comprensión compartida sobre lo que hace?
* ¿Qué partes de VSlices fueron respuesta directa a ese problema?
* ¿Qué partes pueden ser intuición no validada todavía?
* ¿Qué mecanismos actuales de VSlices intentan preservar continuidad?
* ¿Qué límites tiene esta hipótesis?

## Relación con otras preguntas

RQ-001 funciona como pregunta raíz.

De ella derivan preguntas más específicas:

* [RQ-001: continuidad entre líneas paralelas de trabajo](rq-001-continuidad-entre-lineas-paralelas.md)
* [RQ-002: documentación mínima para preservar continuidad sin burocracia](rq-002-documentacion-mínima.md)
* [RQ-003: continuity paths como mecanismo de preservación conceptual](rq-003-continuity-paths.md)

## Evidencia inicial disponible

* Definición de VSlices como suite enfocada en continuidad entre dominio, documentación, arquitectura, implementación y evolución.
* Regla de evolución de producto: las ideas deben surgir desde problemas reales y evidencia antes de convertirse en parte oficial de la suite.
* Alive Lab existe como espacio para validar ideas antes de formalizarlas como parte de VSlices.
* Experiencia profesional retrospectiva y restringida en sistemas empresariales longevos donde la pérdida de continuidad de conocimiento dificultó la comprensión, renovación y evolución segura del software.
* Observación general de que un sistema puede seguir funcionando operativamente mientras se pierde conocimiento compartido sobre dominio, flujos, decisiones e intención original.
* Observación general de que renovar un sistema legacy puede requerir reconstruir conocimiento antes de intervenir técnicamente.

## Evidencia retrospectiva restringida

La formulación inicial de esta pregunta está influenciada por experiencia profesional previa en sistemas empresariales longevos, donde se observó que la pérdida de continuidad entre conocimiento de dominio, flujos operacionales, decisiones del sistema y software existente puede dificultar la renovación segura de una plataforma.

Por razones de confidencialidad, esta evidencia no se documenta como caso de estudio detallado ni incluye información interna, propietaria, operacional o identificable de la organización.

La evidencia se usa únicamente para formular el problema general de investigación:

> sistemas que siguen funcionando pueden perder conocimiento compartido sobre qué hacen, por qué lo hacen, cómo se conectan sus flujos y qué necesidades originales siguen cumpliendo.

Esta experiencia no valida por sí sola a VSlices.

Sí ayuda a justificar que el problema de pérdida de continuidad existe como preocupación práctica y merece ser investigado mediante casos observables, documentables y permitidos dentro de Alive Lab.

## Evidencia no documentable

Por límites éticos, profesionales y de confidencialidad, no deben documentarse detalles internos de organizaciones, sistemas, flujos, módulos, decisiones técnicas, procesos operacionales o información propietaria observados durante experiencia profesional previa.

Esta evidencia puede inspirar preguntas, hipótesis o findings fundacionales, pero no debe usarse como validación fuerte ni como caso de estudio detallado.

## Evidencia faltante

* Casos documentables y permitidos donde la continuidad se haya roto.
* Ejemplos públicos o propios donde pueda describirse el problema sin restricciones de confidencialidad.
* Ejemplos donde VSlices haya ayudado a preservar continuidad.
* Ejemplos donde VSlices haya agregado ceremonia sin suficiente valor.
* Comparación entre proyectos con y sin mecanismos explícitos de continuidad.
* Observación de casos actuales en Alive Lab donde VSlices intente preservar continuidad desde etapas tempranas.
* Evidencia sobre qué tipos de conocimiento se pierden primero durante la evolución de un sistema.
* Evidencia sobre qué mecanismos ayudan realmente a recuperar o preservar continuidad.

## Riesgos metodológicos

* Convertir el origen de VSlices en relato mítico.
* Asumir que toda fragmentación se resuelve con VSlices.
* Confundir intuiciones fundacionales con hallazgos validados.
* Usar experiencia retrospectiva restringida como si fuera evidencia formal completa.
* Confundir pérdida de documentación con pérdida de continuidad completa.
* Asumir que más documentación resolvería automáticamente el problema.
* Adoptar mecanismos antes de probarlos en Alive Lab.
* Diseñar mecanismos demasiado pesados para prevenir un problema real pero variable.

## Límite actual

Esta pregunta no demuestra que VSlices resuelve la fragmentación de conocimiento en proyectos de software.

Solo establece el problema fundacional que VSlices Research debe investigar.

La evidencia retrospectiva disponible permite formular el problema, pero no validarlo de forma general.

Para avanzar, esta pregunta necesita casos documentables, observaciones actuales y estudios dentro de Alive Lab que permitan distinguir entre intuición fundacional, evidencia observada, findings locales y posibles decisiones de producto.
