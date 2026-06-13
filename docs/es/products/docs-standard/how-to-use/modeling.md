# Modelado de documentos

VSlices Docs Standard trata los documentos como estructuras evolutivas que preservan conocimiento útil.

Un documento no es solo un archivo; es un contenedor con nombre para conocimiento que puede apoyar entendimiento, decisiones, implementación, validación o evolución futuros.

El objetivo del modelado de documentos es hacer que la documentación sea lo suficientemente explícita como para preservar la continuidad sin convertirla en burocracia.

## Estructura progresiva

Los documentos deben crecer progresivamente.

Un equipo no debería empezar con la versión más grande posible de un documento, y no todo conocimiento debería convertirse inmediatamente en un documento formal. VSlices Docs Standard usa cuatro niveles de progresión:

- __L0 - Nota__: captura conocimiento temprano, local, incierto o temporal antes de que el equipo sepa si merece estructura formal.
- __L1 - Documento mínimo__: captura la estructura más pequeña útil para un tipo de documento.
- __L2 - Documento ampliado__: añade detalle cuando la complejidad, el riesgo, la ambigüedad, el tamaño del equipo, la reutilización o la vida útil del sistema requieren documentación más explícita.
- __L3 - Documento de referencia__: representa conocimiento lo suficientemente estable e importante como para convertirse en una referencia mantenida para trabajo futuro.

Los niveles describen madurez y utilidad, no burocracia. Un documento solo debería avanzar cuando el conocimiento demuestre suficiente valor.

### L0 - Nota

Una nota captura conocimiento rápidamente.

Es útil cuando el equipo necesita preservar algo sin decidir todavía dónde pertenece. Ejemplos:

- __Nota de concepto__: un concepto temprano que más adelante puede formar parte del Vocabulario de dominio.
- __Nota de supuesto__: algo que el equipo cree, pero que todavía no ha validado.
- __Nota de riesgo__: una posible fuente de falla, malentendido, retrabajo o complejidad accidental.
- __Pregunta abierta__: algo que el equipo todavía necesita entender.

Una nota puede resolverse, archivarse, fusionarse en un documento o promoverse a un documento formal.

### L1 - Documento mínimo

Un documento mínimo captura la estructura más pequeña útil para un tipo de documento. Debe ser suficiente para apoyar una iteración real sin volverse pesado.

Usa este nivel cuando el equipo sabe que el conocimiento importa, pero todavía no necesita una estructura completa. Ejemplos:

- __Documento de contexto mínimo__: suficiente para explicar dónde está trabajando el equipo.
- __Documento de caso de uso mínimo__: suficiente para explicar comportamiento, consecuencia y validaciones.
- __Registro de decisión mínimo__: suficiente para explicar qué se eligió y por qué.

### L2 - Documento ampliado

Un documento ampliado añade una estructura más explícita.

Usa este nivel cuando el documento deba soportar mayor complejidad, riesgo, ambigüedad, reutilización o coordinación. Ejemplos:

- __Documento de proceso ampliado__: útil cuando importan varios roles, _workflows_, excepciones y _handoffs_.
- __Documento de capacidad ampliado__: útil cuando varios casos de uso dependen de la misma capacidad estable.
- __Registro de decisión ampliado__: útil cuando importan opciones, _tradeoffs_, riesgos y condiciones de revisión.

Un documento debería crecer porque el dominio lo requiere, no porque la plantilla lo permita.

### L3 - Documento de referencia

Un documento de referencia se mantiene como una fuente estable de verdad para trabajo futuro.

L3 no es una plantilla separada. Es un nivel de madurez que significa que el documento es lo suficientemente importante como para ser revisado, mantenido y confiado como referencia. Ejemplos:

- __Vocabulario de dominio de referencia__: lenguaje estable usado a través de varios documentos y equipos.
- __Documento de contexto de referencia__: base compartida para un scenario o work line de larga vida.
- __Documento de capacidad de referencia__: capacidad estable que influye en varios casos de uso, decisiones o áreas de implementación.

No todos los documentos deberían llegar a L3. La mayoría deberían permanecer como notas, documentos mínimos o documentos ampliados. La regla es simple:

> Todo puede comenzar como una nota. Solo el conocimiento que demuestra ser útil debería ganar más estructura.

## Ciclo de vida del documento

Un documento puede evolucionar a través de distintos estados. Los estados y significados sugeridos son:

- __draft__: todavía se está moldeando
- __active__: actualmente representa conocimiento compartido útil
- __superseded__: ha sido reemplazado por conocimiento más nuevo
- __archived__: ya no está activo, pero puede seguir siendo útil como contexto histórico

Un documento no debe tratarse como permanente solo porque exista. Cuando el sistema cambia, la documentación puede necesitar cambiar con él.

## Identidad del documento

Los documentos deben ser fáciles de referenciar. Un documento puede tener un identificador estable cuando necesite conectarse con otros documentos. Ejemplo:

- _context_._order-fulfillment_
- _process_._order-submission_
- _use-case_._create-reservation_
- _capability_._validate-payment_
- _decision_._order-validation-boundary_
- _validation_._payment-rules-feedback_

El identificador no necesita ser complejo. Solo necesita ayudar a los lectores a entender a qué se refiere el documento y cómo se conecta con otro conocimiento.

## Relaciones entre documentos

Los documentos no deberían vivir como archivos aislados. Pueden relacionarse entre sí mediante relaciones simples; las relaciones comunes incluyen:

- supports
- refines
- depends-on
- validates
- challenges
- supersedes

Ejemplos:

- Un Documento de caso de uso refina un Documento de contexto.
- Un Documento de capacidad apoya varios Documentos de caso de uso.
- Un Registro de decisión depende de una Nota de riesgo.
- Una Nota de validación valida o cuestiona una Nota de supuesto.
- Un Registro de decisión más nuevo reemplaza a un Registro de decisión anterior.

## Granularidad

Un documento debe preservar una sola pieza coherente de conocimiento.

- Si un documento intenta explicar demasiadas cosas, puede necesitar dividirse.
- Si varios documentos repiten la misma idea, puede que deban fusionarse.
- Un documento debería dividirse cuando eso mejore la claridad, la reutilización o la trazabilidad.
- Un documento no debería dividirse solo porque la estructura lo permita.

## Metadatos mínimos

Un documento puede incluir metadatos ligeros cuando sea útil.

Ejemplo:

```md
---
id: context.order-fulfillment
type: context-document
status: active
scope: order-fulfillment
related:
  - process.order-submission
  - decision.order-validation-boundary
---
```

Los metadatos deberían apoyar la navegación y la continuidad. No deberían convertirse en la parte más importante del documento.

## Principio de modelado

El modelado de documentos en VSlices Docs Standard sigue un principio: __Usar la estructura más pequeña que preserve el conocimiento del que depende el trabajo futuro__.

- Si una nota es suficiente, usa una nota.
- Si un documento mínimo es suficiente, usa el documento mínimo.
- Si el conocimiento se vuelve estable, riesgoso, reutilizado o crítico para decisiones, dale más estructura.

El propósito no es modelar la documentación perfectamente, sino preservar conocimiento deliberadamente.
