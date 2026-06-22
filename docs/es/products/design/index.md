# VSlices Design

VSlices Design ayuda a los equipos a decidir cuánto entendimiento de dominio necesitan antes de convertir conocimiento de negocio en software.

Proporciona modalidades de diseño, herramientas de razonamiento y heurísticas de modelado.

Ayuda a moverse desde material de negocio poco claro hacia decisiones de software más claras sin perder continuidad.

VSlices Design es intencionalmente independiente de VSlices Framework. No necesitas usar VSlices Framework para aplicar VSlices Design.

!!! principle "Principio de Diseño"

    Entiende el material de negocio antes de construir la estructura de software.

    La modalidad correcta no es la más sofisticada. Es la que coincide con la incertidumbre que el equipo realmente enfrenta.

## Propósito

Muchos proyectos de software comienzan desde artefactos que aparecen tarde en el razonamiento de diseño:

* historias de usuario
* pantallas
* APIs
* tablas de base de datos
* componentes técnicos
* tareas de implementación

Estos artefactos son útiles, pero no siempre son el punto de partida correcto.

!!! risk "Riesgo a evitar"

    Cuando el dominio es poco claro, fragmentado, manual, impulsado por legado u organizacionalmente complejo, partir directamente desde la implementación puede crear complejidad accidental.


VSlices Design existe para reducir ese riesgo.

Su propósito es ayudar a los equipos a elegir cuánto entendimiento, contexto, planificación y feedback necesitan antes de avanzar.


## Relación con la VSlices Suite

VSlices Design es un producto dentro de la VSlices Suite.

Se conecta con los otros productos, pero permanece independiente.

| Producto              | Relación con VSlices Design                                                                                                   |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| [VSlices Docs Standard](../docs-standard/index.md) | Proporciona estructuras documentales para preservar la intención descubierta.                                                 |
| [VSlices Method](../method/index.md)        | Define cómo aplicar Design dentro de un flujo de ingeniería.                                                                  |
| [VSlices Framework](../framework/index.md)     | Puede reflejar más adelante los conceptos resultantes como contextos, capacidades, features, flujos, errores e integraciones. |

!!! principle "Principio de Continuidad"

    El entendimiento de dominio debería mantenerse conectado con la documentación, la arquitectura y la implementación.

    La implementación debería permanecer trazable hacia la intención de negocio que la justificó.


## Principio central

!!! principle "Principio de Diseño"

    Elige la modalidad que responde a la incertidumbre real del equipo.

Lo importante no es elegir la modalidad más sofisticada.

A veces conviene:

* explorar ampliamente
* enfocarse en un problema específico
* aprender desde una pequeña vertical slice
