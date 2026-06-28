---
type: tension
state: observed
code: TNS-0005
title: Variación por ramo o producto vs modelo conceptual común

related_questions:
* RQ-001

related_studies:
* STU-002

related_observations:
* OBS-0005
* OBS-0006

related_findings:
* FND-0002

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

# TNS-0005 — Variación por ramo o producto vs modelo conceptual común

## Tipo

tension

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-002 — Dispersión de conocimiento en un ecosistema asegurador empresarial](../studies/stu-002-insurance-knowledge-dispersion.md)

## Tensión

En un ecosistema empresarial con múltiples ramos, productos y servicios, cada contexto puede necesitar representar el dominio de forma distinta.

Pero, al mismo tiempo, el ecosistema puede necesitar un modelo conceptual común que permita reconocer relaciones, similitudes, diferencias y responsabilidades compartidas.

La tensión puede formularse así:

> Necesitamos permitir variaciones legítimas por ramo o producto, pero también necesitamos un modelo conceptual común mínimo para preservar continuidad transversal.

## Fuerza A

La primera fuerza es la variación por ramo o producto.

En dominios amplios, distintos productos, ramos o contextos operacionales pueden requerir diferencias reales en lenguaje, reglas, procesos, responsabilidades y comportamiento.

Esta variación puede ser legítima porque cada contexto puede tener:

* reglas de negocio específicas
* restricciones operacionales propias
* diferencias regulatorias
* comportamientos particulares
* excepciones históricas o comerciales
* necesidades de integración distintas
* actores diferentes
* ciclos de vida propios
* criterios de validación específicos

Esta fuerza importa porque un modelo conceptual común demasiado temprano puede borrar matices reales del dominio.

Si se obliga a que todos los ramos o productos usen la misma definición, el resultado puede ser una abstracción artificial que no representa bien ningún contexto concreto.

## Fuerza B

La segunda fuerza es el modelo conceptual común.

Aunque la variación local sea necesaria, un ecosistema grande también necesita reconocer conceptos compartidos, familias de comportamiento y responsabilidades equivalentes.

Sin un modelo conceptual común mínimo, puede volverse difícil responder preguntas como:

* ¿qué conceptos aparecen en varios ramos o productos?
* ¿qué procesos pertenecen a una misma familia conceptual?
* ¿qué diferencias son esenciales y cuáles son accidentales?
* ¿qué responsabilidades deberían estar alineadas?
* ¿qué servicios resuelven problemas similares?
* ¿qué conceptos deberían tener una definición transversal?
* ¿qué conceptos deberían mantenerse separados?
* ¿qué reglas son comunes y cuáles son específicas?

Esta fuerza importa porque sin una capa conceptual compartida, el dominio puede fragmentarse en múltiples versiones locales difíciles de comparar, integrar o evolucionar.

## Por qué importa

Esta tensión importa porque la continuidad de conocimiento puede romperse tanto por exceso de variación como por exceso de unificación.

Si se permite que cada ramo o producto evolucione su propio modelo sin conexión transversal, pueden aparecer:

* conceptos duplicados
* servicios con responsabilidades similares
* reglas repetidas con pequeñas diferencias
* dificultad para comparar procesos
* dificultad para coordinar cambios
* documentación fragmentada
* dependencia de expertos locales
* pérdida de visión del dominio como conjunto

Pero si se impone un modelo conceptual común demasiado fuerte, pueden aparecer:

* abstracciones demasiado generales
* pérdida de precisión local
* reglas comunes que no aplican realmente a todos los contextos
* resistencia de equipos o áreas
* modelos que se vuelven burocráticos
* documentación transversal que no ayuda a operar
* decisiones centralizadas que ignoran diferencias legítimas

El problema no es elegir entre variación o modelo común.

El problema es determinar qué debe variar, qué debe compartirse y cómo documentar esa diferencia.

## Evidencia

La evidencia disponible corresponde a experiencia profesional actual y restringida.

Puede formularse solo en términos generales:

* Se observa un ecosistema con múltiples ramos, productos y servicios.
* Se observa que conceptos similares aparecen en más de un contexto.
* Se observa que algunos conceptos varían según producto, ramo o flujo local.
* Se observa que no siempre es evidente si una diferencia representa una regla legítima o una divergencia accidental.
* Se observa que la falta de un modelo conceptual común dificulta reconocer familias de conceptos.
* Se observa que centralizar definiciones sin comprender la variación local podría introducir rigidez conceptual.

No existen artifacts públicos disponibles dentro de VSlices Research para esta tensión.

Por razones de confidencialidad, no se documentan nombres de organizaciones, clientes, proveedores, servicios, APIs, sistemas, flujos internos, reglas propietarias, datos operacionales ni detalles identificables de equipos o personas.

## Observaciones relacionadas

* [OBS-0005 — El conocimiento puede estar activo pero disperso entre productos, ramos y servicios](../observations/obs-0005-conocimiento-activo-pero-disperso.md)
* [OBS-0006 — Conceptos similares pueden recibir nombres distintos según el contexto local](../observations/obs-0006-conceptos-similares-nombres-distintos.md)

## Tensiones relacionadas

* [TNS-0003 — Conocimiento activo vs continuidad transversal](../tensions/tns-0006-conocimiento-activo-vs-continuidad-transversal.md)
* [TNS-0004 — Autonomía local vs lenguaje compartido](../tensions/tns-0003-autonomia-local-vs-lenguaje-compartido.md)

## Posibles respuestas candidatas

* Identificar familias conceptuales en vez de imponer definiciones globales inmediatas.
* Documentar qué partes de un concepto son comunes y qué partes varían por contexto.
* Separar conceptos transversales de conceptos locales.
* Registrar variaciones por ramo o producto como diferencias explícitas, no como excepciones invisibles.
* Usar vocabularios de dominio que permitan alias, variantes y límites de validez.
* Usar context documents para explicar dónde aplica una definición.
* Usar behavior documents para comparar comportamientos observables entre variantes.
* Usar continuity paths para conectar conceptos similares sin asumir equivalencia inmediata.
* Evitar convertir toda similitud en abstracción común.
* Evitar tratar toda diferencia local como caso especial accidental.

Estas respuestas son candidatas.

No deben tratarse todavía como soluciones validadas.

## Riesgo de sobrecorrección

Si se favorece demasiado la variación por ramo o producto, cada contexto puede evolucionar con su propio modelo sin conexión suficiente con el resto del ecosistema.

Esto puede producir:

* fragmentación conceptual
* duplicación de servicios
* dificultad para reconocer procesos equivalentes
* aumento de complejidad accidental
* reglas similares implementadas de forma distinta
* documentación difícil de navegar
* pérdida de continuidad transversal

Si se favorece demasiado el modelo conceptual común, se puede intentar unificar conceptos que deberían permanecer separados.

Esto puede producir:

* modelos genéricos que no representan bien las diferencias reales
* pérdida de precisión de dominio
* abstracciones prematuras
* rigidez frente a productos nuevos
* decisiones centralizadas incorrectas
* documentación transversal que simplifica demasiado
* presión por homogeneidad artificial

La respuesta candidata no debería ser permitir variación ilimitada ni imponer un modelo único.

La respuesta probablemente está en construir un modelo conceptual común mínimo, explícitamente limitado, que permita conectar variantes sin borrar diferencias legítimas.

## Interpretación inicial

Esta tensión sugiere que preservar continuidad conceptual en dominios grandes no significa eliminar la variación.

Significa hacerla visible, nombrarla y conectarla.

Un modelo conceptual común puede ser útil si permite reconocer relaciones entre conceptos, pero se vuelve riesgoso si se transforma en una abstracción obligatoria que ignora los límites locales del dominio.

Desde VSlices Research, esta tensión puede alimentar preguntas sobre cómo representar:

* conceptos compartidos
* variantes por contexto
* límites de validez
* familias conceptuales
* relaciones entre términos locales
* comportamientos comunes y específicos
* decisiones que justifican separación o unificación

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework
* VSlices Tooling

## Límite

Esta tensión no demuestra que todo ecosistema con múltiples productos necesite un modelo conceptual común.

Tampoco demuestra que toda variación por ramo o producto sea legítima.

La tensión solo registra que, en una experiencia profesional actual y restringida, apareció una fricción entre preservar variaciones locales y construir una comprensión conceptual compartida del dominio.

Para fortalecer esta tensión, VSlices Research necesita casos documentables donde pueda compararse:

* conceptos comunes
* variantes locales
* diferencias legítimas
* duplicaciones accidentales
* decisiones de unificación
* decisiones de separación
* efectos de centralizar o no centralizar un modelo conceptual

## Próxima evidencia necesaria

* Casos documentables donde una variación por producto o ramo represente una diferencia legítima.
* Casos documentables donde una variación aparente oculte duplicación accidental.
* Ejemplos donde un modelo conceptual común ayude a preservar continuidad.
* Ejemplos donde un modelo conceptual común introduzca rigidez o abstracción prematura.
* Evidencia sobre cómo documentar límites de validez de un concepto transversal.
* Evidencia sobre cuándo conviene crear una familia conceptual en vez de una definición única.
* Observaciones sobre cómo VSlices Docs Standard podría representar conceptos comunes y variantes locales.
* Observaciones sobre cómo continuity paths podrían conectar variantes sin forzar equivalencia.
