# Iteration 0

*Documentar la realidad actual antes de definir el primer Slice-First*

## Propósito

Esta iteración documenta cómo Domus Orbis abordó un problema real de compra mensual usando VSlices Method.

El objetivo no fue construir inmediatamente una aplicación, automatizar una tienda o resolver pagos. El objetivo fue entender la realidad actual, delimitar el alcance y producir una solución pequeña que redujera fricción sin introducir complejidad demasiado pronto.

Iteration 0 existió para responder una pregunta previa a la implementación:

> ¿Qué realidad actual debemos preservar antes de definir el primer comportamiento estable?

## Escenario observado

El problema apareció en la compra mensual del hogar.

La compra suele repetirse mes a mes, pero actualmente requiere reconstruir manualmente la lista dentro de una aplicación de mercado. Si esa lista no está lista al momento del pago, la compra puede postergarse.

Cuando la compra se posterga, el dinero destinado a despensa puede dispersarse en otros gastos, urgencias o decisiones del día a día.

El problema no era solamente comprar. El problema era que la intención de compra mensual no existía antes del momento crítico.

## 1. Understanding

La primera fase fue Understanding.

En vez de partir diseñando una solución, se documentó el escenario donde aparecía la necesidad.

| Tipo de documento                                                                             | Nombre específico                                                                                                                 | Utilidad                                                                                                                                                                           |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Documento de contexto L0](../../../../products/docs-standard/taxonomy/context-document.md)   | [context.scenario](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/context.scenario.md) | Explicó el contexto real: compra mensual, dinero disponible, carga ejecutiva, tiempo limitado y riesgo de dispersión del dinero.                                                   |
| [Nota de soporte](../../../../products/docs-standard/taxonomy/support-note.md)                | [scope.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/scope.iteration.md)   | Delimitó qué parte del escenario se analizaría. Esto evitó expandir la iteración hacia inventario completo, automatización de pagos, múltiples mercados o una aplicación completa. |
| [Vocabulario de dominio L1](../../../../products/docs-standard/taxonomy/domain-vocabulary.md) | [vocabulary.domain](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/vocabulary.domain.md)             | Preservó términos importantes como lista mensual de compra, lista preparada, mercado, carrito, día de pago, dispersión del dinero y carga ejecutiva.                               |

El vocabulario se trabajó en paralelo con los documentos de contexto y scope. No fue necesario esperar a que el escenario estuviera completamente cerrado para empezar a capturar términos.

## 2. Contextualizing

Después de entender el escenario, se documentó el proceso actual.

| Tipo de documento                                                                       | Nombre específico                                                                                                                                       | Utilidad                                    |
| --------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| [Documento de proceso](../../../../products/docs-standard/taxonomy/process-document.md) | [process.household-shopping](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/contextualizing/process.household-shopping.md) | Mostró cómo ocurre hoy la compra del hogar. |

El flujo identificado fue:

* se recibe el pago mensual;
* se evalúa si hay tiempo, energía y foco;
* si los hay, se entra a la aplicación de mercado;
* se reconstruye manualmente la lista en el carro;
* se compra;
* si no los hay, la compra se posterga;
* durante la postergación, el dinero puede dispersarse.

El proceso se representó con un diagrama de flujo porque el problema dependía de secuencia, momento y fricción.

Esto permitió ver que el punto frágil no estaba al final del proceso, sino antes: la lista no existía como intención preparada antes del pago.

## 3. Planning

Con el escenario y el proceso claros, se pasó a Planning.

| Tipo de documento | Nombre específico                                                                                                                    | Utilidad                                                            |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- |
| Support Note      | [proposal.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/proposal.solution.md)       | Definió la solución, dónde se desenvuelve, qué hará y cómo lo hará. |
| Support Note      | [improvement.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/improvement.solution.md) | Definió cómo podría evolucionar la solución.                        |

La propuesta de solución fue intencionalmente pequeña.

No se propuso construir Domus Orbis completo. No se propuso automatizar el pago. No se propuso integrar una tienda de forma definitiva.

La solución elegida fue crear un archivo YAML centralizado para registrar la compra mensual.

El formato inicial debía permitir registrar:

* versión del formato;
* nombre de la lista;
* mercados;
* URL base del mercado;
* productos;
* nombre del producto;
* URL del producto;
* cantidad o peso.

La idea era que la lista existiera fuera del carrito de una tienda específica. Así podía prepararse antes del pago y usarse como punto de partida para reconstruir la compra con menos fricción.

Entre las mejoras futuras quedaron:

* validar el YAML;
* agregar unidad de peso;
* agregar notas por producto;
* marcar productos esenciales;
* generar una vista humana de la lista;
* preparar carrito de forma asistida;
* automatizar preparación de carrito;
* soportar múltiples mercados de forma más explícita;
* registrar lista como pagada;
* pagar una lista.

Esto permitió preservar ideas sin convertir la iteración en algo más grande de lo necesario.

## 4. Building

La fase Building produjo el artifact mínimo útil.

| Tipo de documento | Nombre específico                                                                                                                                          | Utilidad                                                           |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Artifact          | [artifact.monthly-shopping-list](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/building/artifact.monthly-shopping-list.yaml) | Contenedor del YAML que se empleará para definir listas de compra. |

En este caso no se creó una guía de uso formal porque el usuario, el cliente y el experto de dominio eran la misma persona.

La entrega fue simplemente el YAML.

Esto dejó un aprendizaje importante:

> Building no siempre implica código. A veces el primer artifact útil es un archivo, una plantilla, una configuración o una estructura persistida.

Para este contexto, construir una aplicación habría sido demasiado. El archivo YAML era suficiente para validar si una lista centralizada reducía fricción real.

## 5. Validating

La fase Validating se planteó como una nota de feedback personal.

| Tipo de documento | Nombre específico                                                                                                           | Utilidad                                                    |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| Validation Note   | [validation.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/validation.iteration.md) | Entregó riesgos y feedback en base a la solución realizada. |

El método de validación fue feedback de usuario y revisión de experto de dominio.

Como el usuario real también era el experto de dominio, no se necesitó una ceremonia formal. Bastaba con observar si el artifact ayudaba durante el uso real.

La primera observación relevante fue:

> Una lista centralizada puede ser común, pero cada mercado tiene su propia forma de convertir esa lista en compra.

Este aprendizaje sugiere que el dominio de la lista mensual debe separarse de los adaptadores de mercado.

La lista puede ser estable. La forma de preparar el carrito puede cambiar según el mercado.

## Conclusión

Iteration 0 de Domus Orbis mostró que un Slice-First puede comenzar antes del código.

La iteración no produjo una aplicación. Produjo entendimiento, scope, vocabulario, proceso, propuesta, mejora futura, artifact y validación documentada.

El resultado fue pequeño, pero útil. La principal conclusión fue:

> El primer slice no debe ser una miniatura del sistema futuro. Debe proteger la necesidad actual con la menor cantidad de contexto suficiente.

En Domus Orbis, la necesidad actual era clara:

> La lista mensual debe existir antes del pago.

Esa fue la base para continuar hacia Iteration 1.
