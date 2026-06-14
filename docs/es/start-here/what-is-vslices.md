# ¿Qué es VSlices?

__VSlices__ es una suite progresiva de ingeniería de software enfocada en preservar continuidad entre el descubrimiento del dominio, la documentación, la arquitectura, la implementación y la evolución del sistema.

Ayuda a los equipos a mantener el software estructuralmente cercano al dominio que representa.

VSlices no es solo un framework para organizar código. Está compuesto por cuatro productos conectados:

- __VSlices Method__
- __VSlices Design__
- __VSlices Docs Standard__
- __VSlices Framework__

Cada producto puede usarse de forma independiente, pero están diseñados para trabajar juntos.

## Idea central

Los sistemas de software a menudo se alejan del dominio que representan, y esta deriva suele aparecer cuando el descubrimiento, la documentación, la arquitectura y la implementación evolucionan como actividades separadas.

VSlices propone una dirección diferente:

> El mismo lenguaje del dominio, los límites estructurales y la intención conductual deben permanecer visibles en la documentación, la arquitectura y el código.

El objetivo no es hacer que cada proyecto siga la misma arquitectura, __sino preservar la continuidad__.

## Qué promueve VSlices

VSlices promueve:

- domain-driven design
- vertical slices
- modelado fuerte del dominio
- comportamientos explícitos
- errores esperados explícitos
- capacidades componibles
- arquitectura progresiva
- baja ceremonia

VSlices no requiere que los equipos empiecen con un gran plano arquitectónico. En cambio, anima a los equipos a introducir estructura cuando el dominio demuestra que esa estructura es necesaria.

## Qué no es VSlices

VSlices no impone:

- CQRS,
- Event Sourcing,
- Clean Architecture,
- microservices,
- ni un estilo específico de infraestructura.

Tampoco está pensado para ser:

- low-code tooling,
- automatic software generation,
- ni software de imposición arquitectónica.

VSlices debe apoyar las decisiones de ingeniería, no reemplazarlas.

## Los cuatro productos

### VSlices Method

El método conecta todo el ciclo de vida: descubrimiento, documentación, arquitectura, implementación y evolución, definiendo cómo se espera que los otros productos trabajen juntos.

### VSlices Design

Design se centra en el modelado y el razonamiento arquitectónico antes de la implementación, proporcionando conceptos, técnicas y lenguaje para entender el dominio y dar forma al sistema.

### VSlices Docs Standard

Docs Standard define estructuras de documentación que preservan la intención del sistema. El objetivo es hacer que la documentación sea parte del diseño, no un artefacto desconectado.

### VSlices Framework

Framework proporciona bibliotecas .NET, primitivas y patrones de desarrollo para implementar software orientado al dominio con baja ceremonia y arquitectura progresiva.

> VSlices Framework actualmente es experimental, y su documentación pública está intencionalmente limitada durante v0.1-beta.
