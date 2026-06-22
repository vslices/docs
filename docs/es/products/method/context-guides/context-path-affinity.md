# Caminos de continuidad en VSlices Method

VSlices Method usa los caminos de continuidad para ayudar a decidir cómo abordar un contexto real antes de elegir documentos, técnicas o estructuras de implementación.

Los caminos de continuidad son definidos por VSlices Docs Standard.

VSlices Method no redefine esos caminos.

Los usa como una herramienta de trabajo para reconocer qué continuidad necesita preservarse durante descubrimiento, documentación, diseño, implementación o evolución.

!!! principle "Principio de Continuidad"

    Parte desde la continuidad que necesita preservarse, no desde el documento que podría escribirse.


## Por qué Method necesita esta idea

Sin caminos de continuidad, es fácil tratar la documentación como una lista de documentos por completar.

VSlices Method intenta evitar eso.

La pregunta inicial no debería ser "*Qué documento falta?*", sino: "**¿Qué continuidad necesitamos entender y preservar?**".

Después de responder esa pregunta, Docs Standard ayuda a identificar qué documentos pueden apoyar ese recorrido.

## Caminos disponibles

VSlices Docs Standard define cinco caminos principales de continuidad:

| Camino               | Pregunta que ayuda a responder                                   |
| -------------------- | ---------------------------------------------------------------- |
| [Escenario de negocio](../../docs-standard/continuity-paths/perspectives/business-scenario.md) | ¿Dónde ocurre el trabajo y por qué importa?                      |
| [Contexto de dominio](../../docs-standard/continuity-paths/perspectives/domain-context.md)  | ¿Qué lenguaje, reglas, límites y significados deben preservarse? |
| [Proyecto de software](../../docs-standard/continuity-paths/perspectives/software-project.md) | ¿Qué iniciativa técnica está abordando el trabajo?               |
| [Producto al cliente](../../docs-standard/continuity-paths/perspectives/client-product.md)  | ¿Qué comportamiento visible entrega valor a usuarios o clientes? |
| [Servicio consumible](../../docs-standard/continuity-paths/perspectives/consumable-service.md)  | ¿Qué capacidades ofrece o consume el sistema?                    |

Method no asume que todos los caminos deban recorrerse en cada iteración.

Un trabajo puede tener un camino principal y uno o más caminos secundarios.

## Afinidad contexto-camino

Un contexto tiene afinidad con un camino cuando ese camino explica mejor la continuidad que está en riesgo.

La afinidad contexto-camino ayuda a decidir desde dónde empezar.

| Contexto observado                                                            | Camino con mayor afinidad |
| ----------------------------------------------------------------------------- | ------------------------- |
| El equipo necesita entender cómo ocurre el trabajo hoy                        | Escenario de negocio      |
| El equipo necesita aclarar lenguaje, reglas, límites o significados           | Contexto de dominio       |
| El equipo necesita entrar, modificar o estructurar una iniciativa de software | Proyecto de software      |
| El equipo necesita definir comportamiento visible para usuarios o clientes    | Producto al cliente       |
| El equipo necesita exponer, consumir o coordinar capacidades entre sistemas   | Servicio consumible       |

!!! risk "Riesgo de checklist"

    Si todos los caminos parecen obligatorios, la afinidad se perdió. Los caminos ayudan a reducir ruido, no a agregar ceremonia.


## Caminos principales y secundarios

El camino principal representa la continuidad más importante para el trabajo actual.

Los caminos secundarios aportan contexto, precisión o soporte.

No deberían convertir una iteración pequeña en una exploración completa del sistema.

| Tipo de camino | Uso                                                               |
| -------------- | ----------------------------------------------------------------- |
| Principal      | Explica la continuidad que no podemos perder                      |
| Secundario     | Apoya la comprensión del camino principal                         |
| Futuro         | Puede ser relevante después, pero no necesita profundizarse ahora |

## Uso durante una iteración

Al iniciar una iteración, Method puede usar los caminos de continuidad de esta forma:

1. Observar el contexto real

    Antes de documentar, entender qué situación estamos enfrentando.

2. Identificar la continuidad en riesgo

    Determinar qué conocimiento sería costoso perder, malinterpretar o separar de la implementación.

3. Reconocer el camino con mayor afinidad

    Elegir el camino que mejor explica el trabajo actual.

4. Identificar documentos útiles

    Usar Docs Standard para decidir qué documentos pueden apoyar ese camino.

5. Aplicar afinidad documento-etapa

    Decidir qué documentos conviene trabajar ahora y cuáles pueden esperar.

6. Implementar preservando continuidad

    Mantener conectadas intención, lenguaje, comportamiento, decisiones y estructura técnica.

## Resultado esperado

Usar caminos de continuidad dentro de Method debería ayudar a responder:

* qué continuidad importa ahora
* desde qué perspectiva conviene entender el trabajo
* qué documentos pueden apoyar ese recorrido
* qué caminos pueden esperar
* qué complejidad todavía no necesitamos introducir

Method no usa los caminos para imponer una ruta universal.

Los usa para mantener foco.
