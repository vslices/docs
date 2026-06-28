---
type: tension
state: observed
code: TNS-0002
title: Renovar software vs reconstruir conocimiento perdido

related_questions:
* RQ-001

related_studies:
* STU-001

related_observations:
* OBS-0001
* OBS-0002

related_findings:
* FND-0001

affects:
* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework

confidentiality:
  level: restricted
  reason: professional-experience
  publishable: anonymized-only

evidence:
  level: restricted-retrospective
  artifacts_available: false
  source: professional experience
---

# TNS-0002 — Renovar software vs reconstruir conocimiento perdido

## Tipo

tension

## Estado

observed

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

## Caso o fuente

[STU-001 — Pérdida de continuidad en un ecosistema legacy empresarial](../studies/stu-001-legacy-ecosystem-knowledge-loss.md)

## Tensión

Una iniciativa de renovación de software puede parecer, inicialmente, un problema técnico de modernización, reemplazo o reimplementación.

Sin embargo, cuando se ha perdido continuidad de conocimiento, renovar el software requiere primero reconstruir parte del conocimiento de dominio, flujos, decisiones y comportamiento que el sistema existente ya no expresa de forma clara.

La tensión puede formularse así:

> Necesitamos renovar el software para mejorar su mantenibilidad y evolución, pero también necesitamos reconstruir conocimiento perdido antes de intervenirlo con seguridad.

## Fuerza A

La primera fuerza es la necesidad de renovación técnica.

Un sistema legacy puede necesitar renovación por razones como:

* dificultad para mantenerlo
* tecnologías antiguas
* baja capacidad de evolución
* dependencia de conocimiento local
* arquitectura difícil de modificar
* problemas de integración
* falta de trazabilidad
* riesgo operacional o de auditoría
* separación entre necesidades actuales y comportamiento existente

Desde esta fuerza, la renovación aparece como una respuesta razonable.

El sistema necesita cambiar porque su forma actual limita la capacidad de la organización para evolucionar.

## Fuerza B

La segunda fuerza es la necesidad de reconstruir conocimiento perdido.

Antes de renovar, puede ser necesario comprender:

* qué hace realmente el sistema
* qué procesos sostiene
* qué flujos conecta
* qué reglas de negocio implementa
* qué decisiones históricas siguen siendo válidas
* qué comportamientos son intencionales y cuáles son accidentales
* qué partes del negocio cambiaron desde que el sistema fue construido
* qué necesidades actuales no están bien representadas
* qué riesgos aparecen al reemplazar o modificar una parte

Desde esta fuerza, renovar sin reconstruir conocimiento puede ser peligroso.

La organización podría reemplazar código sin entender suficientemente el dominio que ese código sostiene.

## Por qué importa

Esta tensión importa porque una renovación técnica puede fracasar si se trata el software existente como una fuente suficiente de verdad.

Cuando la continuidad de conocimiento se perdió, el código, la documentación existente y la operación diaria pueden entregar solo fragmentos parciales del sistema.

En ese contexto, renovar software implica también redescubrir:

* dominio
* flujos reales
* decisiones
* dependencias
* comportamientos esperados
* excepciones operacionales
* restricciones de auditoría o cumplimiento
* diferencias entre operación actual y diseño histórico

Si esta reconstrucción no ocurre, la renovación puede reproducir errores antiguos, eliminar comportamientos necesarios, ignorar reglas implícitas o construir una nueva solución desconectada del negocio real.

## Evidencia

La evidencia disponible corresponde a experiencia profesional retrospectiva y restringida.

Puede formularse solo en términos generales:

* Se observó un ecosistema empresarial legacy que requería renovación.
* Se observó que el sistema existente no podía ser reemplazado de forma segura sin reconstruir flujos y conocimiento de negocio.
* Se observó que parte del conocimiento necesario para renovar no estaba disponible de forma explícita, actualizada y compartida.
* Se observó que el negocio había evolucionado y que el software no podía tratarse automáticamente como representación completa del dominio actual.
* Se observó que la renovación requería distinguir entre comportamiento vigente, comportamiento heredado, conocimiento implícito y necesidades actuales.

No existen artifacts públicos disponibles dentro de VSlices Research para esta tensión.

Por razones de confidencialidad, no se documentan nombres, flujos internos, módulos, arquitectura, reglas de negocio, datos operacionales ni detalles identificables de la organización.

## Posibles respuestas candidatas

* Tratar la renovación como una combinación de modernización técnica y redescubrimiento de dominio.
* Levantar flujos antes de definir una estrategia de reemplazo.
* Identificar qué conocimiento está explícito, implícito, perdido o desactualizado.
* Diferenciar comportamiento vigente de comportamiento heredado.
* Registrar decisiones reconstruidas durante la renovación.
* Usar documentación viva para conectar dominio, comportamiento, decisiones y estructura.
* Introducir mecanismos de continuidad desde el inicio de la renovación.
* Diseñar slices de renovación que preserven trazabilidad entre problema, flujo, decisión e implementación.

Estas respuestas son candidatas.

No deben tratarse todavía como soluciones validadas.

## Riesgo de sobrecorrección

Si se favorece demasiado la fuerza de renovación técnica, el equipo puede avanzar rápidamente hacia reescritura, migración o reemplazo sin entender suficientemente el sistema que está interviniendo.

Esto puede producir:

* pérdida de comportamientos necesarios
* reimplementación incompleta de reglas de negocio
* decisiones técnicas desconectadas del dominio actual
* errores en flujos críticos
* falsa sensación de avance
* reemplazo de un sistema incomprendido por otro sistema mal alineado

Si se favorece demasiado la fuerza de reconstrucción de conocimiento, el equipo puede intentar comprender todo antes de actuar.

Esto puede producir:

* parálisis por análisis
* levantamientos demasiado extensos
* documentación pesada
* retraso de mejoras concretas
* dificultad para priorizar qué conocimiento importa realmente
* costo excesivo antes de entregar valor

La respuesta candidata no debería ser renovar sin entender ni entender todo antes de renovar.

La respuesta probablemente está en reconstruir el conocimiento mínimo necesario para renovar de forma segura, por slices trazables y con límites explícitos.

## Interpretación inicial

Esta tensión sugiere que la renovación de software no siempre empieza en el código.

En sistemas donde se perdió continuidad, la renovación puede comenzar con una pregunta anterior:

> ¿Qué conocimiento necesitamos recuperar para intervenir este sistema sin romper su continuidad con el dominio actual?

Desde VSlices Research, esta tensión refuerza la necesidad de estudiar cómo preservar continuidad entre:

* descubrimiento de dominio
* documentación
* decisiones
* arquitectura
* implementación
* evolución

También ayuda a evitar una confusión importante: modernizar tecnología no necesariamente moderniza conocimiento.

## Puede afectar a

* VSlices Research
* VSlices Method
* VSlices Docs Standard
* VSlices Design
* VSlices Framework

## Límite

Esta tensión no demuestra que toda renovación de software requiera un levantamiento completo de dominio.

Tampoco demuestra que toda reescritura sea incorrecta, ni que todo sistema legacy esté desconectado del negocio actual.

La tensión solo registra que, en una experiencia profesional retrospectiva y restringida, renovar software apareció acoplado a la necesidad de reconstruir conocimiento perdido.

Para fortalecer esta tensión, VSlices Research necesita observar casos documentables donde pueda compararse:

* motivación técnica de renovación
* conocimiento disponible antes de renovar
* conocimiento reconstruido durante la renovación
* riesgos detectados por falta de continuidad
* decisiones tomadas para preservar continuidad
* resultados de renovar con o sin mecanismos explícitos de trazabilidad

## Próxima evidencia necesaria

* Casos documentables donde una renovación técnica haya requerido redescubrir dominio.
* Casos donde renovar desde código existente haya sido insuficiente.
* Casos donde levantar flujos antes de renovar haya reducido riesgo.
* Casos donde levantar demasiado conocimiento haya introducido burocracia o retraso.
* Evidencia de qué conocimiento mínimo fue suficiente para avanzar con seguridad.
* Observaciones en Alive Lab sobre cómo VSlices puede preservar continuidad durante evolución o reemplazo progresivo.
* Comparación entre renovación técnica pura y renovación guiada por continuidad de conocimiento.
