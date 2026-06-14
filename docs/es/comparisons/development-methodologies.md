# VSlices y las metodologías de desarrollo

## Propósito

Este documento explica cómo se relaciona VSlices con otras metodologías, prácticas y enfoques arquitectónicos de desarrollo de software.

VSlices no es principalmente:

* una metodología ágil
* un framework de gestión de proyectos
* una arquitectura fija
* un reemplazo de las prácticas de ingeniería existentes

VSlices es una suite de ingeniería de software orientada a la continuidad. Su principal preocupación es preservar la alineación entre:

* comprensión del dominio
* documentación
* razonamiento de diseño
* arquitectura
* implementación
* evolución del sistema

## La diferencia central

La mayoría de las metodologías de desarrollo y enfoques de entrega tienen un centro de gravedad específico.

- Agile se enfoca en adaptar la entrega.
- Scrum se enfoca en organizar el trabajo en equipo.
- Extreme Programming se enfoca en la retroalimentación técnica y la calidad de ingeniería.
- Lean se enfoca en reducir desperdicio y mejorar el flujo.
- Domain-Driven Design se enfoca en comprender y modelar el dominio.

VSlices se enfoca en la continuidad. Las preguntas centrales no son solo:

> ¿Cómo entregamos software?
>
> ¿Cómo organizamos el código?

La pregunta central es:

> ¿Cómo preservamos la intención del dominio, el significado arquitectónico, el conocimiento documentado y el comportamiento ejecutable a medida que el sistema evoluciona?

## Alcance

Este documento compara VSlices con metodologías de desarrollo y enfoques orientados a la entrega.

No compara VSlices con estilos arquitectónicos ni patrones de implementación.

Enfoques arquitectónicos como Clean Architecture, Hexagonal Architecture, CQRS, Event Sourcing, microservices, modular monoliths o Vertical Slice Architecture deben discutirse por separado.

## VSlices y Agile

VSlices es altamente compatible con los principios de Agile. Ambos valoran:

* evolución incremental
* adaptabilidad
* retroalimentación
* simplicidad
* evitar complejidad innecesaria por adelantado

Sin embargo, Agile aborda principalmente cómo los equipos se adaptan y entregan valor con el tiempo.

VSlices aborda cómo el conocimiento, las decisiones, los límites, los comportamientos y la implementación permanecen conectados mientras ocurre esa entrega.

Mientras Agile pregunta: _¿Cómo respondemos al cambio?_, VSlices pregunta: _¿Cómo respondemos al cambio sin perder el significado del sistema?_.

## VSlices y Scrum

Scrum proporciona una estructura para la coordinación del equipo mediante roles, eventos, artefactos e iteraciones.

Y VSlices no intenta reemplazar Scrum, porque no define:

* sprints
* product owners
* scrum masters
* sprint reviews
* reglas de gestión del backlog

Un equipo que usa Scrum todavía podría usar VSlices para preservar la continuidad entre descubrimiento de producto, documentación, arquitectura e implementación.

Scrum ayuda a organizar el trabajo. VSlices ayuda a preservar el significado del trabajo.

## VSlices y Extreme Programming

VSlices está fuertemente alineado con Extreme Programming. Ambos valoran:

* simplicidad
* retroalimentación
* mejora continua
* calidad técnica
* refactorización
* prácticas de ingeniería sostenibles

Extreme Programming se enfoca profundamente en cómo el software se construye de forma segura e incremental. VSlices extiende esta preocupación hacia la continuidad entre el código y el conocimiento que justifica el código.

Mientras XP pregunta: _¿Cómo construimos software con alta calidad técnica y retroalimentación rápida?_, VSlices pregunta: _¿Cómo mantenemos esa calidad técnica conectada con la intención del dominio, las decisiones documentadas y la evolución arquitectónica?_.

## VSlices y Lean Software Development

VSlices está altamente alineado con el pensamiento Lean. Ambos se preocupan por:

* reducir desperdicio
* retrasar decisiones innecesarias
* amplificar el aprendizaje
* evitar la sobreproducción
* mejorar el flujo

VSlices aplica este pensamiento a la continuidad del conocimiento de software. Desde la perspectiva de VSlices, las abstracciones innecesarias, la documentación desactualizada, los tickets desconectados, las decisiones poco claras y la arquitectura desvinculada de las necesidades del dominio son formas de desperdicio.

Mientras Lean pregunta: _¿Cómo reducimos desperdicio y mejoramos el aprendizaje?_, VSlices pregunta: _¿Cómo reducimos el desperdicio causado por el conocimiento fragmentado y la intención arquitectónica perdida?_.

## VSlices y Domain-Driven Design

VSlices es profundamente compatible con Domain-Driven Design. Ambos se preocupan por:

* lenguaje del dominio
* límites del dominio
* significado de negocio
* modelos explícitos
* software moldeado por necesidades reales del negocio

Domain-Driven Design ayuda a los equipos a descubrir, comprender y modelar el dominio. VSlices intenta preservar esa comprensión a lo largo de la documentación, el diseño, la arquitectura, la implementación y la evolución.

Mientras DDD pregunta: _¿Cómo modelamos el software en torno al dominio?_, VSlices pregunta: ¿Cómo mantenemos alineados con el tiempo el modelo de dominio, el conocimiento documentado, la estructura arquitectónica y el comportamiento ejecutable?

## VSlices y Waterfall

VSlices no está alineado con Waterfall tradicional como modelo secuencial de ciclo de vida. VSlices no asume que el descubrimiento, la documentación, el diseño, la implementación y la validación ocurren una sola vez en un orden fijo.

Sin embargo, VSlices no rechaza la documentación ni el pensamiento por adelantado. El problema no es la documentación. Es tratar la documentación como conocimiento congelado.

VSlices prefiere documentación viva que evoluciona con la implementación y preserva el significado arquitectónico a lo largo del tiempo.

Waterfall suele preguntar: _¿Qué debería especificarse antes de que comience la implementación?_, VSlices pregunta: _¿Qué conocimiento debe seguir siendo visible y evolutivo mientras el sistema cambia?_.

## Resumen comparativo

| Enfoque | Preocupación principal | Relación con VSlices |
| --- | --- | --- |
| Agile | Entrega adaptativa | Compatible; añade continuidad entre conocimiento, documentación e implementación |
| Scrum | Coordinación del equipo | Complementario; no lo reemplaza |
| Extreme Programming | Calidad técnica y retroalimentación | Fuertemente alineado; extiende la continuidad más allá del código |
| Lean | Reducción de desperdicio y aprendizaje | Fuertemente alineado; trata el conocimiento fragmentado como desperdicio |
| Domain-Driven Design | Modelado del dominio | Profundamente compatible; preserva la intención del dominio a lo largo del ciclo de vida |
| Waterfall | Especificación y entrega secuenciales | Baja alineación; VSlices prefiere continuidad viva |

## La posición de VSlices

VSlices no es un reemplazo universal para metodologías existentes. Es una capa de continuidad para la ingeniería de software. Ayuda a los equipos a preguntar:

> ¿Nuestra comprensión del dominio, documentos, decisiones, arquitectura e implementación siguen describiendo el mismo sistema?

Cuando la respuesta es no, el sistema puede seguir funcionando, pero su significado ha empezado a fragmentarse.

VSlices existe para reducir esa fragmentación.

## Conclusión

VSlices puede trabajar con equipos ágiles, equipos de ingeniería disciplinados, equipos orientados al dominio y equipos que usan distintos estilos arquitectónicos.

Su diferenciación no está en reemplazar esos enfoques. Está en preservar la continuidad entre ellos.

VSlices se ocupa de lo que a menudo se pierde entre:

* comprender el negocio
* documentar el sistema
* diseñar la solución
* implementar el comportamiento
* y evolucionar el software con el tiempo

Esa continuidad es el centro de VSlices.
