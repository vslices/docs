---
type: finding
state: candidate
code: FND-0002
role: foundational
evidence_level: restricted-live
title: La continuidad de conocimiento puede romperse por dispersión activa entre contextos locales

related_questions:
* RQ-001

related_studies:
* stu-002

related_observations:
* OBS-0005
* OBS-0006
* OBS-0007
* OBS-0008
* OBS-0009

related_tensions:
* TNS-0003
* TNS-0004
* TNS-0005
* TNS-0006

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework
* VSlices Tooling

confidentiality:
  level: restricted
  reason: current-professional-context
  publishable: anonymized-only

evidence:
  level: restricted-live
  artifacts_available: false
  source: current professional experience
---

# FND-0002 — La continuidad de conocimiento puede romperse por dispersión activa entre contextos locales

## Tipo

finding

## Rol

foundational

## Estado

candidate

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente principal

[Study — Dispersión de conocimiento en un ecosistema asegurador empresarial](../studies/stu-002-insurance-knowledge-dispersion.md)

## Formulación

Esta evidencia sugiere que la continuidad de conocimiento puede romperse no solo porque el conocimiento se pierda históricamente, sino también porque el conocimiento activo queda disperso entre contextos locales sin mecanismos suficientes para conectarlo transversalmente.

En este caso, el problema no es ausencia total de conocimiento.

El problema es que el conocimiento existe en productos, ramos, servicios, equipos o procesos específicos, pero no necesariamente forma una comprensión compartida del dominio como conjunto.

Dicho de forma breve:

> El conocimiento puede estar vivo localmente y, aun así, carecer de continuidad transversal.

## Observaciones que lo sostienen

* [OBS-0005 — El conocimiento puede estar activo pero disperso entre productos, ramos y servicios](../observations/obs-0005-conocimiento-activo-pero-disperso.md)
* [OBS-0006 — Conceptos similares pueden recibir nombres distintos según el contexto local](../observations/obs-0006-conceptos-similares-nombres-distintos.md)
* [OBS-0007 — La duplicación de servicios puede reflejar falta de continuidad conceptual, no solo redundancia técnica](../observations/obs-0007-duplicacion-servicios-falta-continuidad-conceptual.md)
* [OBS-0008 — La ausencia de definiciones compartidas dificulta reconocer similitudes entre procesos](../observations/obs-0008-ausencia-definiciones-compartidas-dificulta-reconocer-similitudes.md)
* [OBS-0009 — Una organización puede tener expertos locales sin una vista transversal suficiente del dominio](../observations/obs-0009-expertos-locales-sin-vista-transversal.md)

## Tensiones relacionadas

* [TNS-0003 — Autonomía local vs lenguaje compartido](../tensions/tns-0003-autonomia-local-vs-lenguaje-compartido.md)
* [TNS-0005 — Variación por ramo o producto vs modelo conceptual común](../tensions/tns-0005-variacion-ramo-producto-vs-modelo-conceptual-comun.md)
* [TNS-0006 — Conocimiento activo vs continuidad transversal](../tensions/tns-0006-conocimiento-activo-vs-continuidad-transversal.md)
* [TNS-0007 — Servicios especializados vs duplicación conceptual](../tensions/tns-0007-servicios-especializados-vs-duplicacion-conceptual.md)

## Evidencia

La evidencia disponible proviene de experiencia profesional actual y restringida en un ecosistema empresarial del dominio asegurador.

Por razones de confidencialidad, esta evidencia no incluye artifacts públicos, nombres de sistemas, servicios, APIs, flujos internos, reglas propietarias, decisiones técnicas, datos operacionales ni detalles identificables de la organización, proveedor, equipos o personas.

La evidencia puede formularse solo en términos generales:

* Se observa un ecosistema con múltiples productos, ramos, servicios y contextos operacionales.
* Se observa que existen personas, equipos y sistemas con conocimiento local activo.
* Se observa que conceptos similares pueden aparecer nombrados de forma distinta según contexto.
* Se observa que servicios diferentes pueden gestionar responsabilidades conceptualmente cercanas.
* Se observa que la ausencia de definiciones compartidas dificulta reconocer similitudes entre procesos.
* Se observa que la existencia de expertos locales no garantiza una vista transversal suficiente del dominio.
* Se observa que no siempre es evidente cuándo una diferencia representa variación legítima, duplicación accidental o separación conceptual necesaria.

Esta evidencia permite formular un finding candidato, pero no constituye validación fuerte ni generalizable.

## Interpretación

El problema observado no es pérdida de conocimiento por olvido.

La interpretación inicial es que el problema aparece cuando el conocimiento queda distribuido entre contextos locales sin suficientes mecanismos de conexión conceptual.

En este escenario, cada producto, ramo, servicio o equipo puede conservar conocimiento útil para operar su parte del dominio. Sin embargo, la organización puede tener dificultad para construir respuestas transversales:

* qué conceptos son compartidos
* qué conceptos son locales
* qué términos son equivalentes
* qué términos son variantes
* qué procesos pertenecen a una misma familia conceptual
* qué servicios representan responsabilidades similares
* qué diferencias son legítimas
* qué diferencias son accidentales
* qué decisiones deberían conectarse entre contextos

Esto produce una forma distinta de fragilidad.

No es la fragilidad de un sistema que nadie entiende.

Es la fragilidad de un ecosistema donde muchas partes son entendidas localmente, pero el conjunto no queda suficientemente conectado.

## Alcance

Este finding aplica, de forma inicial y prudente, a ecosistemas de software y dominio donde:

* existen múltiples productos, ramos, áreas o contextos locales
* el conocimiento experto está distribuido
* los conceptos similares aparecen en varios servicios o procesos
* los lenguajes locales dificultan reconocer similitudes
* la organización opera correctamente en partes locales
* la vista transversal del dominio es limitada o difícil de reconstruir
* la evolución del sistema requiere coordinar decisiones entre contextos

Este finding tiene valor principalmente fundacional y comparativo: amplía RQ-001 mostrando que la pérdida de continuidad no ocurre solamente por envejecimiento histórico, sino también por dispersión activa.

## Relación con VSlices

Este finding ayuda a ampliar el problema fundacional de VSlices Research.

VSlices no solo debería estudiar cómo evitar que el conocimiento se pierda con el tiempo.

También debería estudiar cómo evitar que el conocimiento vivo quede fragmentado entre contextos locales sin continuidad transversal.

Desde este finding, VSlices Research puede investigar si mecanismos como vocabularios de dominio, context documents, behavior documents, continuity paths, mapas conceptuales, decisiones trazables y tooling documental ayudan a conectar conocimiento local sin imponer uniformidad prematura.

Esto se conecta con la misión de VSlices de preservar continuidad entre descubrimiento de dominio, documentación, arquitectura, implementación y evolución.

Pero también agrega un matiz importante:

> preservar continuidad no significa centralizar todo el conocimiento, sino conectar conocimiento distribuido con límites explícitos.

## Relación con FND-0001

Este finding complementa a [FND-0001 — La pérdida de continuidad de conocimiento dificulta la evolución segura de sistemas de software](../findings/fnd-0001-perdida-continuidad-dificulta-evolucion-validacion.md).

FND-0001 observa una forma de ruptura de continuidad asociada a pérdida histórica, redescubrimiento y dificultad para evolucionar sistemas longevos.

FND-0002 observa una forma distinta de ruptura de continuidad asociada a dispersión activa, conocimiento local y falta de vista transversal.

Ambos findings pueden alimentar una distinción inicial:

* pérdida histórica de continuidad: el conocimiento existió, pero dejó de estar disponible, trazable o compartido
* dispersión activa de continuidad: el conocimiento existe, pero está fragmentado entre contextos locales sin conexión suficiente

Esta distinción todavía debe tratarse como candidata.

No debe convertirse en taxonomía oficial hasta observar más casos.

## Límites

Este finding no demuestra que toda dispersión de conocimiento sea negativa.

Tampoco demuestra que toda organización con expertos locales carezca de continuidad transversal.

No demuestra que centralizar definiciones sea la solución correcta.

No demuestra que todos los servicios similares sean duplicados.

No demuestra que todos los conceptos similares deban unificarse.

En dominios grandes, la distribución del conocimiento puede ser necesaria, legítima y saludable. Muchos productos, ramos o servicios necesitan lenguaje, reglas y decisiones propias.

La evidencia disponible es actual, profesional, restringida y no documentable con artifacts públicos. Por lo tanto, este finding debe tratarse como fundacional y candidato, no como validado.

## Riesgos de interpretación

* Confundir dispersión de conocimiento con ausencia de conocimiento.
* Asumir que centralizar definiciones resolvería el problema.
* Tratar toda variación local como duplicación accidental.
* Tratar todo servicio similar como redundante.
* Forzar un modelo conceptual común antes de entender diferencias reales.
* Eliminar lenguaje local que representa matices legítimos del dominio.
* Convertir un problema de continuidad transversal en una iniciativa burocrática de documentación.
* Usar este finding para justificar VSlices sin validar sus mecanismos.
* Confundir continuidad con uniformidad.
* Confundir conexión conceptual con control centralizado.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework
* VSlices Tooling

## Próxima evidencia necesaria

Para fortalecer, refinar o descartar este finding, VSlices Research necesita evidencia adicional y documentable.

Evidencia deseable:

* Casos documentables donde el conocimiento exista localmente, pero no esté conectado transversalmente.
* Casos donde expertos locales no logren formar una vista compartida del dominio completo.
* Casos donde conceptos similares aparezcan con nombres distintos en varios contextos.
* Casos donde servicios similares sean duplicación conceptual accidental.
* Casos donde servicios similares sean especializaciones legítimas.
* Casos donde un vocabulario compartido ayude a preservar continuidad sin borrar diferencias locales.
* Casos donde un vocabulario compartido introduzca rigidez o burocracia.
* Casos donde continuity paths ayuden a conectar conceptos distribuidos.
* Casos donde behavior documents permitan comparar procesos similares.
* Casos donde VSlices ayude a conectar conocimiento activo sin imponer uniformidad.
* Casos donde mecanismos de VSlices agreguen ceremonia sin mejorar continuidad.

## Estado de madurez

Este finding debe permanecer como `candidate`.

Puede alimentar RQ-001 y orientar estudios futuros, pero no debe convertirse todavía en principio oficial, patrón adoptado o decisión de producto.

Su función actual es fundacional:

> ayuda a ampliar el problema práctico que VSlices Research debe investigar, mostrando que la continuidad puede fallar por dispersión activa incluso cuando el conocimiento sigue existiendo localmente.
---

type: finding
state: candidate
code: FND-0003
role: foundational
evidence_level: restricted-live
title: La continuidad de conocimiento puede romperse cuando conocimiento crítico permanece concentrado en una persona clave durante una transición

related_questions:

* RQ-001

related_studies:

* stu-003-key-person-knowledge-transition

related_observations:

* OBS-0010
* OBS-0011
* OBS-0012
* OBS-0013
* OBS-0014

related_tensions:

* TNS-0007
* TNS-0008

affects:

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

confidentiality:
level: restricted
reason: current-professional-transition
publishable: anonymized-only

evidence:
level: restricted-live
artifacts_available: false
source: current professional experience
---------------------------------------

# FND-0003 — La continuidad de conocimiento puede romperse cuando conocimiento crítico permanece concentrado en una persona clave durante una transición

## Tipo

finding

## Rol

foundational

## Estado

candidate

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente principal

[Study — Riesgo de pérdida de conocimiento por salida de una persona clave](../studies/stu-003-key-person-knowledge-transition.md)

## Formulación

Esta evidencia sugiere que la continuidad de conocimiento puede romperse o debilitarse cuando conocimiento crítico permanece concentrado en una persona clave durante una transición, salida o cambio de rol.

En este caso, el conocimiento no está necesariamente perdido.

Tampoco está necesariamente disperso entre muchos contextos locales.

El conocimiento existe, está activo y puede ser usado durante la operación normal, pero depende demasiado de la disponibilidad de una persona específica.

Dicho de forma breve:

> El equipo puede funcionar mientras la persona clave está disponible, pero perder continuidad cuando esa disponibilidad desaparece.

## Observaciones que lo sostienen

* [OBS-0010 — El conocimiento crítico puede estar activo pero concentrado en una persona clave](../observations/obs-0010-conocimiento-critico-activo-concentrado-persona-clave.md)
* [OBS-0011 — La salida de una persona puede revelar dependencias de conocimiento ocultas durante la operación normal](../observations/obs-0011-salida-revela-dependencias-conocimiento-ocultas.md)
* [OBS-0012 — No todo conocimiento acumulado necesita transferirse con el mismo nivel de profundidad](../observations/obs-0012-conocimiento-acumulado-no-requiere-misma-profundidad.md)
* [OBS-0013 — La transferencia efectiva requiere priorizar conocimiento por riesgo, frecuencia de uso y dificultad de reconstrucción](../observations/obs-0013-transferencia-prioriza-riesgo-frecuencia-dificultad-reconstruccion.md)
* [OBS-0014 — El conocimiento técnico relevante puede estar mezclado con contexto histórico, decisiones implícitas y criterios de operación](../observations/obs-0014-conocimiento-tecnico-mezclado-contexto-decisiones-operacion.md)

## Tensiones relacionadas

* [TNS-0007 — Transferencia suficiente vs documentación exhaustiva](../tensions/tns-0007-transferencia-suficiente-vs-documentacion-exhaustiva.md)
* [TNS-0008 — Responsabilidad profesional de transferencia vs límite personal de salida](../tensions/tns-0008-responsabilidad-profesional-transferencia-vs-limite-personal-salida.md)

## Evidencia

La evidencia disponible proviene de experiencia profesional actual y restringida en un contexto de transición laboral.

Por razones de confidencialidad, esta evidencia no incluye artifacts públicos, nombres de sistemas, servicios, APIs, repositorios, flujos internos, reglas propietarias, decisiones técnicas identificables, datos operacionales ni detalles de la organización, cliente, proveedor, equipos o personas.

La evidencia puede formularse solo en términos generales:

* Se observa que una persona concentra conocimiento relevante sobre partes del sistema, dominio, operación o evolución.
* Se observa que ese conocimiento puede estar activo y ser usado para responder dudas, desbloquear decisiones o sostener continuidad durante la operación normal.
* Se observa que una posible salida o transición hace visible el riesgo de que ese conocimiento deje de estar disponible.
* Se observa que no todo el conocimiento acumulado está documentado, distribuido o convertido en artifacts compartidos.
* Se observa que no todo conocimiento acumulado requiere el mismo nivel de profundidad de transferencia.
* Se observa que la transferencia necesita priorizar conocimiento por riesgo, frecuencia de uso y dificultad de reconstrucción.
* Se observa que parte del conocimiento técnico relevante está mezclado con contexto histórico, decisiones implícitas y criterios prácticos de operación.

Esta evidencia permite formular un finding candidato, pero no constituye validación fuerte ni generalizable.

## Interpretación

El problema observado no es simplemente que una persona se vaya.

La interpretación inicial es que la salida o transición puede revelar una fragilidad previa: parte de la continuidad del equipo dependía de conocimiento concentrado en una persona específica.

Mientras esa persona está disponible, la continuidad puede parecer estable porque el equipo puede recuperar contexto mediante conversaciones, consultas informales, intervención directa o memoria personal.

Sin embargo, esa continuidad puede ser frágil si el conocimiento no está suficientemente distribuido, documentado, transferido o validado por otras personas.

En este escenario, la salida no necesariamente crea la pérdida de continuidad.

Puede revelar que la continuidad ya estaba demasiado acoplada a una disponibilidad humana específica.

## Alcance

Este finding aplica, de forma inicial y prudente, a equipos, proyectos o sistemas donde:

* una persona concentra conocimiento relevante para operación, soporte o evolución
* parte del conocimiento crítico no está documentado ni distribuido
* el equipo depende de consultas informales a una persona específica
* una salida, cambio de rol o reducción de disponibilidad puede afectar continuidad
* el conocimiento acumulado mezcla técnica, historia, decisiones y operación
* transferir todo el conocimiento acumulado sería inviable o poco usable
* se necesita priorizar qué conocimiento transferir antes de una transición

Este finding tiene valor principalmente fundacional y comparativo: amplía `RQ-001` mostrando que la pérdida de continuidad no ocurre solamente por envejecimiento histórico o dispersión activa, sino también por concentración personal durante transiciones.

## Relación con VSlices

Este finding ayuda a ampliar el problema fundacional de VSlices Research.

VSlices no solo debería estudiar cómo evitar que el conocimiento se pierda con el tiempo o quede disperso entre contextos locales.

También debería estudiar cómo evitar que conocimiento crítico quede demasiado acoplado a una persona clave, especialmente cuando esa persona cambia de rol, reduce disponibilidad o sale del equipo.

Desde este finding, VSlices Research puede investigar posteriormente si mecanismos como documentación mínima, continuity paths, notas de soporte, decision records, context documents, behavior documents, mapas de riesgo o prácticas de transferencia ayudan a preservar continuidad durante una transición.

Pero esa evaluación todavía no corresponde a este finding.

Este documento no propone una solución de VSlices.

Solo identifica un escenario donde la continuidad puede romperse.

## Relación con FND-0001 y FND-0002

Este finding complementa a:

* [FND-0001 — La pérdida de continuidad de conocimiento dificulta mantener, evolucionar y validar sistemas de software](../findings/fnd-0001-perdida-continuidad-dificulta-evolucion-validacion.md)
* [FND-0002 — La continuidad de conocimiento puede romperse por dispersión activa entre contextos locales](../findings/fnd-0002-continuidad-rota-por-dispersion-activa.md)

FND-0001 observa una forma de ruptura asociada a pérdida histórica, redescubrimiento y dificultad para evolucionar sistemas longevos.

FND-0002 observa una forma de ruptura asociada a dispersión activa, conocimiento local y falta de vista transversal.

FND-0003 observa una forma de ruptura potencial asociada a concentración personal de conocimiento durante una transición.

En conjunto, estos findings pueden alimentar una distinción inicial:

* pérdida histórica de continuidad: el conocimiento existió, pero dejó de estar disponible, trazable o compartido
* dispersión activa de continuidad: el conocimiento existe, pero está fragmentado entre contextos locales sin conexión suficiente
* concentración personal de continuidad: el conocimiento existe, pero está demasiado acoplado a una persona clave

Esta distinción todavía debe tratarse como candidata.

No debe convertirse en taxonomía oficial hasta observar más casos, revisar contra evidencia adicional y contrastar sus límites.

## Límites

Este finding no demuestra que toda salida de una persona clave produzca pérdida de continuidad.

Tampoco demuestra que toda concentración de conocimiento sea negativa.

En algunos contextos, es normal y razonable que ciertas personas concentren más conocimiento por experiencia, especialización, rol, antigüedad o participación directa en decisiones relevantes.

Este finding tampoco demuestra que todo conocimiento personal deba documentarse exhaustivamente.

No demuestra que la responsabilidad de transferencia pertenezca solo a la persona que sale.

No demuestra que la organización pueda resolver concentración de conocimiento solo con documentos.

La evidencia disponible es actual, profesional, restringida y no documentable con artifacts públicos. Por lo tanto, este finding debe tratarse como fundacional y candidato, no como validado.

## Riesgos de interpretación

* Confundir concentración de conocimiento con culpa individual.
* Asumir que la persona que sale debe compensar toda la deuda de conocimiento acumulada.
* Tratar toda salida como emergencia documental.
* Intentar transferir todo el conocimiento acumulado sin priorización.
* Confundir documentación exhaustiva con continuidad real.
* Transferir solo información técnica y omitir contexto histórico, decisional u operacional.
* Asumir que una transferencia breve siempre es suficiente.
* Ignorar que parte del conocimiento puede requerir práctica, validación o acompañamiento.
* Usar este finding para justificar VSlices sin validar sus mecanismos.
* Convertir un problema de continuidad en una exigencia de heroísmo individual.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Tooling

## Próxima evidencia necesaria

Para fortalecer, refinar o descartar este finding, VSlices Research necesita evidencia adicional y documentable.

Evidencia deseable:

* Casos documentables donde una salida o cambio de rol revele concentración de conocimiento.
* Casos donde una transferencia mínima haya preservado continuidad suficiente.
* Casos donde una transferencia insuficiente haya producido bloqueos posteriores.
* Casos donde documentación exhaustiva haya sido poco usada o poco efectiva.
* Casos donde documentación detallada haya sido necesaria por criticidad, regulación o riesgo.
* Casos donde la organización haya reducido dependencia personal antes de una salida.
* Evidencia sobre qué conocimiento debe priorizarse antes de una transición.
* Evidencia sobre cómo validar que el conocimiento fue transferido realmente.
* Evidencia sobre qué parte del conocimiento requiere documento, sesión práctica, acompañamiento o referencia breve.
* Casos donde mecanismos de VSlices ayuden a preservar continuidad durante una transición.
* Casos donde mecanismos de VSlices agreguen ceremonia sin mejorar continuidad.

## Estado de madurez

Este finding debe permanecer como `candidate`.

Puede alimentar `RQ-001` y orientar estudios futuros, pero no debe convertirse todavía en principio oficial, patrón adoptado o decisión de producto.

Su función actual es fundacional:

> ayuda a ampliar el problema práctico que VSlices Research debe investigar, mostrando que la continuidad puede fallar cuando conocimiento crítico permanece concentrado en una persona clave durante una transición.
