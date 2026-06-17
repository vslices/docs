# VSlices y las metodologías de desarrollo

## Propósito

Este documento explica cómo VSlices se relaciona con metodologías, prácticas y enfoques de entrega de software.

VSlices no es una metodología ágil, un framework de gestión de proyectos, una arquitectura fija ni un reemplazo de las prácticas de ingeniería existentes.

Es una suite de ingeniería de software orientada a la continuidad. Su principal preocupación es preservar la alineación entre comprensión del dominio, documentación, razonamiento de diseño, arquitectura, implementación y evolución del sistema.

## La diferencia central

La mayoría de las metodologías de desarrollo y enfoques de entrega tienen un centro de gravedad específico.

- Agile se enfoca en adaptar la entrega.
- Scrum se enfoca en organizar el trabajo en equipo.
- Extreme Programming se enfoca en la retroalimentación técnica y la calidad de ingeniería.
- Lean se enfoca en reducir desperdicio y mejorar el flujo.
- Domain-Driven Design se enfoca en comprender y modelar el dominio.

VSlices se enfoca en la continuidad entre esas preocupaciones.

Sus preguntas centrales no son solo:

* ¿Cómo entregamos software?
* ¿Cómo organizamos el código?

!!! note "Pregunta central para VSlices"

    ¿Cómo preservamos la intención del dominio, el significado arquitectónico, el conocimiento documentado y el comportamiento ejecutable a medida que el sistema evoluciona?

## Alcance

| Este documento cubre | Este documento no cubre |
| --- | --- |
| Cómo VSlices se relaciona con metodologías de desarrollo y enfoques orientados a la entrega. | Cómo VSlices se relaciona con estilos arquitectónicos o patrones de implementación. |

Enfoques arquitectónicos como Clean Architecture, Hexagonal Architecture, CQRS, Event Sourcing, microservices, modular monoliths o Vertical Slice Architecture deben discutirse por separado.

## VSlices y otras metodologías

VSlices puede compararse con distintas metodologías y enfoques de entrega. Cada comparación mantiene el mismo foco: qué optimiza el otro enfoque, cómo se relaciona con VSlices y qué agrega VSlices mediante continuidad.

=== "Agile"

    **Relación:** Altamente compatible.

    **Preocupaciones compartidas:**

    * evolución incremental
    * adaptabilidad
    * retroalimentación
    * simplicidad
    * evitar complejidad innecesaria por adelantado

    **Diferencia:** Agile se enfoca en adaptar la entrega. VSlices se enfoca en preservar continuidad mientras ocurre esa entrega.

    !!! note "Pregunta de VSlices"

        ¿Cómo respondemos al cambio sin perder el significado del sistema?

=== "Scrum"

    **Relación:** Complementaria.

    **Scrum define:**

    * sprints
    * product owners
    * scrum masters
    * sprint reviews
    * reglas de gestión del backlog

    **Diferencia:** Scrum ayuda a organizar el trabajo. VSlices ayuda a preservar el significado del trabajo.

    !!! note "Pregunta de VSlices"

        ¿Cómo preservamos continuidad entre descubrimiento de producto, documentación, arquitectura e implementación?

=== "Extreme Programming"

    **Relación:** Fuertemente alineada.

    **Preocupaciones compartidas:**

    * simplicidad
    * retroalimentación
    * mejora continua
    * calidad técnica
    * refactorización
    * prácticas de ingeniería sostenibles

    **Diferencia:** Extreme Programming se enfoca en construir software de forma segura e incremental. VSlices extiende esa preocupación hacia la continuidad entre el código y el conocimiento que justifica ese código.

    !!! note "Pregunta de VSlices"

        ¿Cómo mantenemos la calidad técnica conectada con la intención del dominio, las decisiones documentadas y la evolución arquitectónica?

=== "Lean Software Development"

    **Relación:** Fuertemente alineada.

    **Preocupaciones compartidas:**

    * reducir desperdicio
    * retrasar decisiones innecesarias
    * amplificar el aprendizaje
    * evitar la sobreproducción
    * mejorar el flujo

    **Diferencia:** Lean se enfoca en reducir desperdicio y mejorar el aprendizaje. VSlices aplica esa preocupación a la continuidad del conocimiento de software, tratando el conocimiento fragmentado, la documentación desactualizada, las decisiones poco claras y la arquitectura desvinculada de las necesidades del dominio como formas de desperdicio.

    !!! note "Pregunta de VSlices"

        ¿Cómo reducimos el desperdicio causado por conocimiento fragmentado e intención arquitectónica perdida?

=== "Domain-Driven Design"

    **Relación:** Profundamente compatible.

    **Preocupaciones compartidas:**

    * lenguaje del dominio
    * límites del dominio
    * significado de negocio
    * modelos explícitos
    * software moldeado por necesidades reales del negocio

    **Diferencia:** Domain-Driven Design ayuda a los equipos a descubrir, comprender y modelar el dominio. VSlices intenta preservar esa comprensión a lo largo de la documentación, el diseño, la arquitectura, la implementación y la evolución.

    !!! note "Pregunta de VSlices"

        ¿Cómo mantenemos alineados con el tiempo el modelo de dominio, el conocimiento documentado, la estructura arquitectónica y el comportamiento ejecutable?

=== "Waterfall"

    **Relación:** Baja alineación con Waterfall tradicional secuencial.

    **Diferencia:** Waterfall trata el descubrimiento, la documentación, el diseño, la implementación y la validación como una secuencia que ocurre en un orden fijo. VSlices los trata como fuentes evolutivas de conocimiento.

    !!! note "Pregunta de VSlices"

        ¿Qué conocimiento debe permanecer visible y evolutivo mientras el sistema cambia?

## Resumen comparativo

La siguiente tabla resume la relación principal entre cada enfoque y VSlices.

| Enfoque | Preocupación principal | Relación con VSlices |
| --- | --- | --- |
| Agile | Entrega adaptativa | Compatible; añade continuidad entre conocimiento, documentación e implementación. |
| Scrum | Coordinación del equipo | Complementario; no lo reemplaza. |
| Extreme Programming | Calidad técnica y retroalimentación | Fuertemente alineado; extiende la continuidad más allá del código. |
| Lean | Reducción de desperdicio y aprendizaje | Fuertemente alineado; trata el conocimiento fragmentado como desperdicio. |
| Domain-Driven Design | Modelado del dominio | Profundamente compatible; preserva la intención del dominio a lo largo del ciclo de vida. |
| Waterfall | Especificación y entrega secuenciales | Baja alineación; VSlices prefiere continuidad viva. |

## La posición de VSlices

VSlices no es un reemplazo universal para metodologías existentes. Es una capa de continuidad para la ingeniería de software.

Ayuda a los equipos a preguntar:

!!! note "Pregunta de continuidad"

    ¿Nuestra comprensión del dominio, documentos, decisiones, arquitectura e implementación siguen describiendo el mismo sistema?

Cuando la respuesta es no, el sistema puede seguir funcionando, pero su significado ha empezado a fragmentarse.

VSlices existe para reducir esa fragmentación.

## Conclusión

VSlices puede trabajar con equipos ágiles, equipos de ingeniería disciplinados, equipos orientados al dominio y equipos que usan distintos estilos arquitectónicos.

Su diferenciación no está en reemplazar esos enfoques. Está en preservar continuidad entre comprensión del negocio, documentación, diseño, implementación y evolución del software.

Esa continuidad es el centro de VSlices.
