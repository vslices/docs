# Modelado de documentos

VSlices Docs Standard trata los documentos como estructuras evolutivas que preservan conocimiento útil.

Un documento no es solo un archivo. Es un contenedor con nombre para conocimiento que puede apoyar entendimiento, decisiones, implementación, validación o evolución futuros.

El objetivo del modelado de documentos es hacer que la documentación sea lo suficientemente explícita como para preservar continuidad sin convertirla en burocracia.

!!! principle "Principio de Modelado"

    Usa la estructura más pequeña que preserve el conocimiento del que depende el trabajo futuro.


## Estructura progresiva

Los documentos deben crecer progresivamente.

Un equipo no debería empezar con la versión más grande posible de un documento. Tampoco todo conocimiento debería convertirse inmediatamente en un documento formal.

VSlices Docs Standard usa cuatro niveles de progresión:

| Nivel | Nombre                  | Uso                                                                                                         |
| ----- | ----------------------- | ----------------------------------------------------------------------------------------------------------- |
| [L0](#l0---nota)    | Nota                    | Captura conocimiento temprano, local, incierto o temporal antes de saber si merece estructura formal.       |
| [L1](#l1---documento-mínimo)    | Documento mínimo        | Captura la estructura más pequeña útil para un tipo de documento.                                           |
| [L2](#l2---documento-ampliado)    | Documento ampliado      | Añade detalle cuando la complejidad, el riesgo, la ambigüedad, la coordinación o la vida útil lo requieren. |
| [L3](#l3---documento-de-referencia)    | Documento de referencia | Representa conocimiento estable e importante que debe mantenerse como referencia para trabajo futuro.       |

Los niveles describen madurez y utilidad, no burocracia.

Un documento solo debería avanzar cuando el conocimiento demuestra suficiente valor.

## L0 - Nota

Una nota captura conocimiento rápidamente.

Es útil cuando el equipo necesita preservar algo sin decidir todavía dónde pertenece.

Ejemplos:

* **Nota de concepto**: un concepto temprano que más adelante puede formar parte del Vocabulario de dominio
* **Nota de supuesto**: algo que el equipo cree, pero que todavía no ha validado
* **Nota de riesgo**: una posible fuente de falla, malentendido, retrabajo o complejidad accidental
* **Pregunta abierta**: algo que el equipo todavía necesita entender

Una nota puede resolverse, archivarse, fusionarse en un documento o promoverse a un documento formal.

## L1 - Documento mínimo

Un documento mínimo captura la estructura más pequeña útil para un tipo de documento.

Debe ser suficiente para apoyar una iteración real sin volverse pesado.

Usa este nivel cuando el equipo sabe que el conocimiento importa, pero todavía no necesita una estructura completa.

Ejemplos:

* **Documento de contexto mínimo**: suficiente para explicar dónde está trabajando el equipo
* **Documento de caso de uso mínimo**: suficiente para explicar comportamiento, consecuencia y validaciones
* **Registro de decisión mínimo**: suficiente para explicar qué se eligió y por qué

## L2 - Documento ampliado

Un documento ampliado añade una estructura más explícita.

Usa este nivel cuando el documento deba soportar mayor complejidad, riesgo, ambigüedad, reutilización o coordinación.

Ejemplos:

* **Documento de proceso ampliado**: útil cuando importan varios roles, *workflows*, excepciones y *handoffs*
* **Documento de capacidad ampliado**: útil cuando varios casos de uso dependen de la misma capacidad estable
* **Registro de decisión ampliado**: útil cuando importan opciones, *tradeoffs*, riesgos y condiciones de revisión

Un documento debería crecer porque el dominio lo requiere, no porque la plantilla lo permita.

## L3 - Documento de referencia

Un documento de referencia se mantiene como una fuente estable de verdad para trabajo futuro.

L3 no es una plantilla separada. Es un nivel de madurez que significa que el documento es lo suficientemente importante como para ser revisado, mantenido y usado como referencia.

Ejemplos:

* **Vocabulario de dominio de referencia**: lenguaje estable usado a través de varios documentos y equipos
* **Documento de contexto de referencia**: base compartida para un escenario o línea de trabajo de larga vida
* **Documento de capacidad de referencia**: capacidad estable que influye en varios casos de uso, decisiones o áreas de implementación

No todos los documentos deberían llegar a L3.

La mayoría deberían permanecer como notas, documentos mínimos o documentos ampliados.

!!! principle "Principio de Progresión"

    Todo puede comenzar como una nota. Solo el conocimiento que demuestra ser útil debería ganar más estructura.


## Ciclo de vida del documento

Un documento puede evolucionar a través de distintos estados.

| Estado       | Significado                                                               |
| ------------ | ------------------------------------------------------------------------- |
| draft      | Todavía se está moldeando.                                                |
| active     | Actualmente representa conocimiento compartido útil.                      |
| superseded | Fue reemplazado por conocimiento más nuevo.                               |
| archived   | Ya no está activo, pero puede seguir siendo útil como contexto histórico. |

Un documento no debe tratarse como permanente solo porque existe.

Cuando el sistema cambia, la documentación puede necesitar cambiar con él.

## Identidad y metadatos

Los documentos deben ser fáciles de referenciar.

Un documento puede tener un identificador estable cuando necesite conectarse con otros documentos.

Ejemplos:

* context.order-fulfillment
* process.order-submission
* use-case.create-reservation
* capability.validate-payment
* decision.order-validation-boundary
* validation.payment-rules-feedback

El identificador no necesita ser complejo. Solo necesita ayudar a los lectores a entender a qué se refiere el documento y cómo se conecta con otro conocimiento.

Un documento también puede incluir metadatos ligeros cuando sea útil.

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

## Relaciones entre documentos

Los documentos no deberían vivir como archivos aislados.

Pueden relacionarse entre sí mediante relaciones simples.

| Relación     | Uso                                                          |
| ------------ | ------------------------------------------------------------ |
| supports   | Un documento apoya o da contexto a otro.                     |
| refines    | Un documento vuelve más específico el conocimiento de otro.  |
| depends-on | Un documento depende de conocimiento preservado en otro.     |
| validates  | Un documento confirma conocimiento anterior.                 |
| challenges | Un documento cuestiona o pone en duda conocimiento anterior. |
| supersedes | Un documento reemplaza conocimiento anterior.                |

Ejemplos:

* Un Documento de caso de uso refina un Documento de contexto.
* Un Documento de capacidad apoya varios Documentos de caso de uso.
* Un Registro de decisión depende de una Nota de riesgo.
* Una Nota de validación valida o cuestiona una Nota de supuesto.
* Un Registro de decisión más nuevo reemplaza a un Registro de decisión anterior.

## Granularidad

Un documento debe preservar una sola pieza coherente de conocimiento.

* Si un documento intenta explicar demasiadas cosas, puede necesitar dividirse.
* Si varios documentos repiten la misma idea, puede que deban fusionarse.
* Un documento debería dividirse cuando eso mejore la claridad, la reutilización o la trazabilidad.
* Un documento no debería dividirse solo porque la estructura lo permita.

!!! risk "Riesgo a evitar"

    Dividir documentos sin una razón de continuidad puede crear fragmentación en vez de claridad.


## Regla de modelado

El propósito no es modelar la documentación perfectamente.

El propósito es preservar conocimiento deliberadamente.

* Si una nota es suficiente, usa una nota.
* Si un documento mínimo es suficiente, usa el documento mínimo.
* Si el conocimiento se vuelve estable, riesgoso, reutilizado o crítico para decisiones, dale más estructura.

!!! principle "Principio de Modelado"

    Usa la estructura documental más pequeña que preserve el conocimiento necesario para el trabajo futuro.
