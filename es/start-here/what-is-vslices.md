# ¿Qué es VSlices?

__VSlices__ es una suite progresiva de ingeniería de software enfocada en preservar continuidad entre el descubrimiento del dominio, la documentación, el razonamiento de diseño, la arquitectura, la implementación, la validación y la evolución del sistema.

Ayuda a los equipos a mantener el software estructuralmente cercano al dominio que representa.

VSlices no es solo un framework para organizar código. Está compuesto por cuatro productos conectados:

- __[VSlices Method](../products/method/index.md)__: conecta descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución.
- __[VSlices Design](../products/design/index.md)__: aporta razonamiento de diseño y técnicas de modelado.
- __[VSlices Docs Standard](../products/docs-standard/index.md)__: define estructuras de documentación viva.
- __[VSlices Framework](../products/framework/index.md)__: ofrece apoyo para la implementación.

Cada producto puede usarse de forma independiente, pero están diseñados para trabajar juntos.

## Idea central

Los sistemas de software a menudo se alejan del dominio que representan. Esta deriva suele aparecer cuando el descubrimiento, la documentación, el diseño, la arquitectura y la implementación evolucionan como actividades separadas.

!!! principle "Principio de continuidad"

    El mismo lenguaje del dominio, los límites estructurales y la intención conductual deberían permanecer visibles en la documentación, la arquitectura y el código.

El objetivo no es hacer que cada proyecto siga la misma arquitectura, __sino preservar continuidad__.

## Qué promueve VSlices

VSlices promueve prácticas que mantienen visible la intención del dominio a medida que el sistema crece:

| Área | Qué enfatiza VSlices |
| --- | --- |
| Entendimiento del dominio | domain-driven design y modelado fuerte del dominio |
| Estructura del sistema | vertical slices, capacidades componibles y arquitectura progresiva |
| Claridad del comportamiento | comportamientos explícitos y errores esperados explícitos |
| Estilo de adopción | baja ceremonia y estructura introducida solo cuando el dominio la necesita |

VSlices no requiere que los equipos empiecen con un gran plano arquitectónico. En cambio, anima a introducir estructura cuando el dominio demuestra que esa estructura es necesaria.

## Qué no es VSlices

VSlices no impone una arquitectura específica ni reemplaza el criterio de ingeniería.

| VSlices no impone... | Qué significa |
| --- | --- |
| CQRS | Los equipos pueden usarlo cuando el dominio o la complejidad lo justifican, pero VSlices no lo exige. |
| Event Sourcing | El historial de eventos no se asume como estrategia predeterminada de persistencia o modelado. |
| Clean Architecture | Las decisiones de capas deberían emerger de las necesidades del sistema, no de una plantilla obligatoria. |
| microservices | El despliegue y los límites de servicios son decisiones arquitectónicas, no valores predeterminados de VSlices. |
| un estilo específico de infraestructura | Las decisiones de infraestructura deberían apoyar al dominio en vez de definir la arquitectura desde el inicio. |

VSlices tampoco es:

* una herramienta low-code
* un generador automatico de software
* software de imposición arquitectónica

VSlices debe apoyar las decisiones de ingeniería, no reemplazarlas.

## Los cuatro productos

VSlices está compuesto por cuatro productos que preservan continuidad desde distintos ángulos:

| Producto | Enfoque |
| --- | --- |
| [VSlices Method](../products/method/index.md) | Conecta descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución a lo largo del ciclo de vida del software. |
| [VSlices Design](../products/design/index.md) | Proporciona conceptos, técnicas y lenguaje para razonar sobre el dominio y dar forma al sistema antes de implementar. |
| [VSlices Docs Standard](../products/docs-standard/index.md) | Define estructuras de documentación viva que preservan la intención del sistema y mantienen la documentación conectada al diseño. |
| [VSlices Framework](../products/framework/index.md) | Proporciona bibliotecas .NET, primitivas y patrones de desarrollo para implementar software orientado al dominio con baja ceremonia y arquitectura progresiva. |

{% include-markdown "shared/experimental/vslices-framework-v0.1beta.md" %}
