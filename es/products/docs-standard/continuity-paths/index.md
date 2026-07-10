# Introducción

Un camino de continuidad es una forma de recorrer la documentación desde una perspectiva concreta.

No es una secuencia obligatoria de documentos.

Es una lectura narrativa que muestra cómo el conocimiento se conecta, qué documentos explican cada parada y qué profundidad documental existe en cada punto.

Por ejemplo, un equipo puede recorrer la documentación desde la perspectiva de un escenario, de un producto, de una línea de trabajo, de una capacidad, de una decisión o de una validación.

!!! principle "Principio de Continuidad"

    Un camino de continuidad debería ayudar a entender cómo una pieza de conocimiento se conecta con otros documentos, decisiones, implementación y aprendizaje.


## Perspectivas de continuidad

Los caminos de continuidad pueden comenzar desde distintas perspectivas.

Cada perspectiva responde una pregunta diferente y permite recorrer la documentación desde una intención distinta.

| Perspectiva                                               | Pregunta que ayuda a responder                         | Enfoque principal    |
| --------------------------------------------------------- | ------------------------------------------------------ | -------------------- |
| [Escenario de negocio](perspectives/business-scenario.md) | ¿Dónde estoy trabajando?                               | Procesos de negocio                  |
| [Contexto de dominio](perspectives/domain-context.md)     | ¿Qué lenguaje, reglas y límites pertenecen al negocio? | Modelado de dominio                  |
| [Proyecto de software](perspectives/software-project.md)  | ¿Qué herramientas tengo para abordar el trabajo?       | Alcance de software                 |
| [Producto al cliente](perspectives/client-product.md)     | ¿Qué puede hacer el usuario en un sistema?             | Experiencia, uso y coordinación de software |
| [Servicio consumible](perspectives/consumable-service.md) | *Qué capacidades ofrece este sistema para otros?       | Capacidades de software                 |



Una perspectiva no reemplaza a las demás.

Solo define desde dónde empieza la lectura.

## Profundidad documental

Un camino de continuidad también ayuda a ver hasta qué profundidad fue documentado un punto.

Una parada del camino puede estar apenas identificada, explicada mínimamente, ampliada o mantenida como referencia.

| Profundidad  | Significado                                                       |
| ------------ | ----------------------------------------------------------------- |
| Identificada | El conocimiento existe, pero todavía tiene poca estructura.       |
| Mínima       | Hay suficiente documentación para apoyar trabajo cercano.         |
| Ampliada     | Hay más detalle porque existe complejidad, riesgo o coordinación. |
| Referencia   | El conocimiento es estable e importante para trabajo futuro.      |

Esto permite observar la documentación generada por VSlices sin asumir que todo debe tener la misma profundidad.

Un camino puede mostrar que una parte del sistema está bien entendida, otra está en exploración y otra solo fue excluida del alcance actual.
