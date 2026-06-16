# Metodología aplicada en la iteración 0

*Cómo Domus Orbis usó VSlices Method en su iteración 0*

## Propósito

Este documento explica cómo se aplicó VSlices Method dentro de la iteración 0 de Domus Orbis.

No busca definir una regla universal para todos los proyectos. Busca mostrar cómo un caso real seleccionó fases, documentos y *artifacts* según su alcance.

El inicio de Domus Orbis fue un caso especialmente útil porque el problema inicial no era principalmente técnico. La dificultad estaba en preservar continuidad entre una necesidad doméstica real, una solución pequeña y una posible evolución futura.

## Enfoque general

La metodología aplicada siguió una secuencia simple:

{% include-markdown "shared/simple-design-iteration-flow.md" %}

Cada fase produjo únicamente los documentos o *artifacts* necesarios para sostener la siguiente decisión.

El objetivo no fue completar una plantilla ideal. El objetivo fue preservar suficiente intención para construir algo pequeño sin perder el problema original.

## Por qué partir con Iteration 0

Domus Orbis no comenzó con Iteration 1 porque todavía no estaba claro cuál debía ser el primer comportamiento estable.

Antes de definir el primer Slice-First, fue necesario documentar la realidad actual:

* dónde aparecía la necesidad
* qué parte del escenario importaba
* qué proceso estaba fallando
* qué términos podían volverse importantes
* qué solución pequeña podía reducir fricción sin resolver todo el sistema

Por eso, Iteration 0 fue usada para entender y delimitar.

La regla observada fue:

> Iteration 0 documenta la realidad actual. Iteration 1 define el primer comportamiento estable Slice-First.

## Slice-First pequeño, no desechable

La solución inicial de Domus Orbis fue pequeña: un archivo YAML.

Pero eso no significa que fuera desechable.

La intención fue crear un *artifact* que pudiera sobrevivir a futuras iteraciones. Aunque después existan herramientas de consola, preparación automática de carrito o integraciones con mercados, el sistema seguirá necesitando saber qué productos se deben comprar, desde qué mercado y en qué cantidad.

Un buen Slice-First no es el código o *artifact* más pequeño posible. Es el comportamiento estable más pequeño que protege la necesidad actual.
