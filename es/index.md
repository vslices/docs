---
hide:
  - navigation
---

<div class="vslices-hero">
  <img
    src="https://raw.githubusercontent.com/vslices/icons/refs/heads/main/official/icon.svg"
    alt="VSlices icon"
    class="vslices-hero__icon"
  />

  <div class="vslices-hero__content">
    <h1>VSlices</h1>
    <p>
      Una suite progresiva de ingeniería de software enfocada en preservar continuidad entre el descubrimiento del dominio, la documentación, el razonamiento de diseño, la arquitectura, la implementación, la validación y la evolución del sistema.
    </p>
  </div>
</div>

VSlices está compuesto por cuatro productos conectados:

<div class="grid cards" markdown>

-   **[VSlices Framework](products/framework/index.md)**

    Apoyo para implementar software orientado al dominio con baja ceremonia y arquitectura progresiva.

-   **[VSlices Design](products/design/index.md)**

    Razonamiento de diseño y técnicas de modelado para entender el dominio antes de implementar.

-   **[VSlices Docs Standard](products/docs-standard/index.md)**

    Estructuras de documentación viva para preservar la intención del sistema a medida que el software evoluciona.

-   **[VSlices Method](products/method/index.md)**

    Un método de continuidad que conecta descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución.

</div>

## Estado actual de madurez

VSlices se encuentra actualmente en una etapa de __beta prerelease__.

Esta documentación se comparte temprano para validar si la suite comunica sus ideas con claridad, preserva la continuidad conceptual entre sus productos y ayuda a las personas a razonar sobre ingeniería de software sin añadir ceremonia innecesaria.

La versión actual debe leerse como una instantánea fundacional, no como una especificación final del producto.

| Área | Estado actual | Qué esperar |
| --- | --- | --- |
| [VSlices Design](./products/design/index.md) | Beta prerelease | Las ideas principales de diseño, los principios y las<br/>modalidades de modelado están disponibles para<br/>comentarios tempranos.<br/><br/>Algunas técnicas pueden seguir evolucionando a medida<br/>que se validan en proyectos reales. |
| [VSlices Docs Standard](./products/docs-standard/index.md) | Beta prerelease | El modelo de documentación, los tipos de documento y<br/>los principios de continuidad están disponibles para<br/>comentarios tempranos.<br/><br/>Las plantillas y ejemplos pueden volverse más concretos<br/>con el tiempo. |
| [VSlices Method](./products/method/index.md) | Beta prerelease | El método conecta actualmente el razonamiento de<br/>diseño, la documentación y la intención de<br/>implementación.<br/><br/>Sus modelos de colaboración y continuidad están<br/>disponibles para revisión y refinamiento. |
| [VSlices Framework](./products/framework/index.md) | Experimental | La documentación de Framework está intencionalmente<br/>limitada mientras los conceptos de Design, Docs<br/>Standard y Method se revisan juntos.<br/><br/>Su modelo de implementación puede cambiar a medida<br/>que mejore el alineamiento. |
| [Alive Lab](./alive-lab/index.md) | Exploratory | Las field notes, project stories, theories y decisiones<br/>preservan el aprendizaje en curso.<br/><br/>Estos materiales pueden influir en VSlices, pero no todos<br/>son orientación oficial del producto. |

El objetivo de este prerelease no es presentar VSlices como completo. Es hacer visible el pensamiento actual, recibir comentarios y mejorar la suite antes de expandir la documentación de Framework y traducir la documentación completa al español.

## Comienza aquí

Si eres nuevo en VSlices, usa esta ruta de lectura según lo que necesites entender:

| Si quieres... | Comienza con... |
| --- | --- |
| Entender la idea central | [¿Qué es VSlices?](start-here/what-is-vslices.md) |
| Entender por qué existe VSlices | [Por qué existe VSlices](start-here/why-vslices-exists.md) |
| Entender cómo se relacionan los productos entre sí | [Vista general de la suite](start-here/suite-overview.md) |
| Explorar posibles rutas de adopción | [Rutas de adopción - WIP](start-here/adoption-paths.md) |

También puedes comenzar desde la página general de [¿Cómo empezar?](start-here/index.md).

## Productos

Los productos de VSlices pueden evolucionar independientemente, pero están pensados para preservar la misma continuidad desde distintos ángulos:

| Producto | Enfoque |
| --- | --- |
| [VSlices Method](products/method/index.md) | Conecta descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución. |
| [VSlices Design](products/design/index.md) | Ayuda a razonar sobre el dominio y dar forma al sistema antes de implementar. |
| [VSlices Docs Standard](products/docs-standard/index.md) | Preserva la intención del sistema mediante estructuras de documentación viva. |
| [VSlices Framework](products/framework/index.md) | Apoya la implementación mediante bibliotecas .NET, primitivas y patrones de desarrollo. |

Juntos ayudan a mantener alineados el entendimiento, la documentación, el diseño, la implementación, la validación y la evolución a medida que el sistema crece.

## Validación

VSlices está siendo definido y validado mediante trabajo real de diseño e implementación de software.

El [Alive Lab](alive-lab/index.md) preserva teorías, historias de proyectos, descubrimientos de modelado y observaciones de campo que dan forma a VSlices con el tiempo.

El contenido de Alive Lab debe leerse como aprendizaje en progreso. Algunas ideas pueden convertirse más adelante en orientación oficial del producto, mientras que otras pueden permanecer como material exploratorio.

## Decisiones

Las decisiones importantes de metodología, producto y documentación se registran en la [sección de Decisiones](decisions/index.md). Estos registros preservan:

* por qué se tomó una decisión
* qué tradeoffs fueron aceptados
* qué permanece incierto
* cómo VSlices evoluciona desde presión real de diseño

## Estado actual

VSlices se encuentra actualmente en una etapa fundacional temprana.

La documentación representa la primera estructura pública de la suite, no una metodología terminada ni un ecosistema completo de framework.

Algunas ideas son lo suficientemente estables para documentarse como parte de v0.1. Otras ideas permanecen experimentales y se mantienen intencionalmente dentro del [Alive Lab](alive-lab/index.md) hasta ser validadas con mayor profundidad.
