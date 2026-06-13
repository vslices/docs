# VSlices

__VSlices__ es una suite progresiva de ingeniería de software enfocada en preservar continuidad entre el descubrimiento del dominio, la documentación, el razonamiento de diseño, la arquitectura, la implementación y la evolución del sistema.

Está compuesta por:

* __VSlices Framework__, para apoyar la implementación.
* __VSlices Design__, para el razonamiento de diseño y las técnicas de modelado.
* __VSlices Docs Standard__, para estructuras de documentación viva.
* __VSlices Method__, para conectar descubrimiento, documentación, diseño, arquitectura e implementación.

VSlices existe para reducir complejidad accidental y preservar la intención arquitectónica a medida que un sistema evoluciona.

## Estado actual de madurez

VSlices se encuentra actualmente en una etapa de __beta prerelease__.

Esta documentación se comparte temprano para validar si la suite comunica sus ideas con claridad, preserva la continuidad conceptual entre sus productos y ayuda a las personas a razonar sobre ingeniería de software sin añadir ceremonia innecesaria.

La versión actual debe leerse como una instantánea fundacional, no como una especificación final del producto.

| Área | Estado actual | Qué esperar |
| --- | --- | --- |
| VSlices Design | Beta prerelease | Las ideas principales de diseño, los principios y las modalidades de modelado están disponibles para comentarios tempranos. Algunas técnicas pueden seguir evolucionando a medida que se validan en proyectos reales. |
| VSlices Docs Standard | Beta prerelease | El modelo de documentación, los tipos de documento y los principios de continuidad están disponibles para comentarios tempranos. Las plantillas y ejemplos pueden volverse más concretos con el tiempo. |
| VSlices Method | Beta prerelease | El método conecta actualmente el razonamiento de diseño, la documentación y la intención de implementación. Sus modelos de colaboración y continuidad están disponibles para revisión y refinamiento. |
| VSlices Framework | Experimental | La documentación de Framework está intencionalmente limitada mientras los conceptos de Design, Docs Standard y Method se revisan juntos. Su modelo de implementación puede cambiar a medida que mejore el alineamiento. |
| Alive Lab | Exploratory | Las field notes, project stories, theories y decisiones preservan el aprendizaje en curso. Estos materiales pueden influir en VSlices, pero no todos son orientación oficial del producto. |

El objetivo de este prerelease no es presentar VSlices como completo. Es hacer visible el pensamiento actual, recibir comentarios y mejorar la suite antes de expandir la documentación de Framework y traducir la documentación completa al español.

## Comienza aquí

Si eres nuevo en VSlices, comienza con estas páginas:

* [¿Cómo empezar?](start-here/index.md)
* [¿Qué es VSlices?](start-here/what-is-vslices.md)
* [Por qué existe VSlices](start-here/why-vslices-exists.md)
* [Vista general de la suite](start-here/suite-overview.md)
* [Rutas de adopción - WIP](start-here/adoption-paths.md)

Si solo quieres entender la idea central, comienza con [¿Qué es VSlices?](start-here/what-is-vslices.md).

Si quieres entender por qué existe VSlices, lee [Por qué existe VSlices](start-here/why-vslices-exists.md).

Si quieres entender cómo se relacionan los productos entre sí, lee [Vista general de la suite](start-here/suite-overview.md).

## Productos

VSlices se documenta como una suite de productos conectados:

* [VSlices Framework](products/framework/index.md) explica las bases orientadas a la implementación.
* [VSlices Design](products/design/index.md) explica cómo razonamos sobre diseño de software.
* [VSlices Docs Standard](products/docs-standard/index.md) explica cómo preservamos conocimiento mediante documentación.
* [VSlices Method](products/method/index.md) explica cómo los productos se conectan a lo largo del ciclo de vida del software.

Cada producto puede evolucionar independientemente, pero todos comparten el mismo objetivo: preservar continuidad entre entender, documentar, diseñar, construir y evolucionar software.

## Validación

VSlices está siendo definido y validado mediante trabajo real de diseño e implementación de software.

El [Alive Lab](alive-lab/index.md) preserva teorías, historias de proyectos, descubrimientos de modelado y observaciones de campo que dan forma a VSlices con el tiempo.

## Decisiones

Las decisiones importantes de metodología, producto y documentación se registran en la [sección de Decisions](decisions/index.md). Estos registros preservan:

* por qué se tomó una decisión
* qué tradeoffs fueron aceptados
* qué permanece incierto
* cómo VSlices evoluciona desde presión real de diseño

## Estado actual

VSlices se encuentra actualmente en una etapa fundacional temprana.

La documentación representa la primera estructura pública de la suite, no una metodología terminada ni un ecosistema completo de framework.

Algunas ideas son lo suficientemente estables para documentarse como parte de v0.1. Otras ideas permanecen experimentales y se mantienen intencionalmente dentro del Alive Lab hasta ser validadas con mayor profundidad.
