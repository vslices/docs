# Mantener los productos separados pero conectados

## Estado

Aceptada.

## Contexto

VSlices evoluciona como una suite de ingeniería de software compuesta por múltiples productos:

* VSlices Framework
* VSlices Design
* VSlices Docs Standard
* VSlices Method

Cada producto aborda una parte distinta del ciclo de vida del software. La suite existe para preservar la continuidad entre:

* descubrimiento del dominio
* documentación
* razonamiento de diseño
* arquitectura
* implementación
* validación
* evolución

Apareció un riesgo mientras se definía la estructura de la documentación: tratar todos los productos como si fueran solo secciones del framework.

Eso haría que la suite fuera más fácil de describir a corto plazo, pero más débil a largo plazo. VSlices Framework es solo un producto orientado a la implementación dentro de la suite.

VSlices Design, VSlices Docs Standard y VSlices Method deben poder evolucionar de forma independiente del framework.

## Decisión

Los productos de VSlices se documentarán y evolucionarán como productos separados pero conectados.

Cada producto debe tener:

* su propia identidad,
* su propia responsabilidad,
* su propia sección de documentación,
* su propio camino de evolución,
* y sus propios criterios de validación.

Los productos deben permanecer conectados mediante principios compartidos y relaciones trazables, pero ningún producto debe reducirse a una subsección de otro producto.

La suite se organizará como:

```text
VSlices Suite
  VSlices Framework
  VSlices Design
  VSlices Docs Standard
  VSlices Method
```

La conexión compartida entre productos es el modelo de continuidad.

Los productos no son independientes porque no tengan relación. Son independientes porque resuelven problemas distintos dentro del mismo ciclo de vida.

## Límites de producto

VSlices Framework es responsable del soporte de implementación.

Proporciona bibliotecas, primitivas, abstracciones, adaptadores, convenciones y patrones de desarrollo que ayudan a implementar software orientado al dominio con baja ceremonia y arquitectura progresiva.

VSlices Design es responsable del razonamiento de diseño.

Proporciona técnicas de modelado, estrategias de análisis, guía de descubrimiento del dominio, heurísticas de separación y herramientas de razonamiento arquitectónico.

VSlices Docs Standard es responsable de la estructura de la documentación.

Define cómo se preservan el conocimiento del dominio, las decisiones arquitectónicas, los casos de uso, las capacidades, las vistas, los procesos, los errores esperados y los invariantes en documentación viva.

VSlices Method es responsable de la continuidad del ciclo de vida.

Explica cómo Design, Docs Standard y Framework pueden trabajar juntos a lo largo del descubrimiento, la documentación, la arquitectura, la implementación y la evolución.

## Fundamento

Mantener separados los productos evita el acoplamiento accidental entre productos.

Si todo se trata como parte de VSlices Framework, aparecen varios problemas:

* las técnicas de diseño se vuelven dependientes del uso del framework,
* los estándares de documentación se vuelven específicos de la implementación,
* el método queda oculto detrás de ejemplos de código,
* los usuarios que no son desarrolladores quedan excluidos,
* y la suite se vuelve más difícil de explicar con honestidad.

> VSlices Design debería ser útil incluso cuando un equipo no usa VSlices Framework.
> VSlices Docs Standard debería ser útil incluso cuando la implementación no está escrita en .NET.
> VSlices Method debería guiar la continuidad incluso antes de que exista código.
> VSlices Framework debería seguir siendo un acelerador de implementación, no el propietario de toda la suite.

Al mismo tiempo, separar demasiado los productos crearía otro problema: fragmentación.

Los productos no deben derivar hacia herramientas no relacionadas.

Deben permanecer conectados mediante vocabulario compartido, principios compartidos y relaciones trazables del ciclo de vida.

## Consecuencias

Esta decisión le da a cada producto espacio para madurar de forma independiente. También hace que la documentación sea más clara porque cada sección puede enfocarse en una responsabilidad.

El tradeoff es que algunos conceptos pueden aparecer en más de un producto. Cuando eso ocurra, cada producto debe explicar el concepto desde su propia perspectiva. Por ejemplo:

* VSlices Design puede explicar una capacidad como un concepto de modelado.
* VSlices Docs Standard puede explicar cómo documentar una capacidad.
* VSlices Framework puede explicar cómo implementar una capacidad.
* VSlices Method puede explicar cuándo y por qué la capacidad se mueve a través del ciclo de vida.

Esta repetición es aceptable cuando preserva la perspectiva.

Solo se convierte en un problema cuando los documentos duplican la misma explicación sin agregar valor específico del producto.

## Regla de documentación

La documentación de los productos debe evitar mezclar responsabilidades.

Una página de índice debe explicar el propósito y el alcance del producto.

No debe intentar explicar toda la suite.

Las relaciones detalladas entre productos deben vivir en la documentación orientada al método o a la suite.

Cada página de producto debe responder:

* ¿De qué es responsable este producto?
* ¿Para quién es?
* ¿Qué problema resuelve?
* ¿Qué no resuelve intencionalmente?
* ¿Cómo se conecta con el resto de VSlices?

## Regla de validación

Un producto no debe absorber responsabilidades de otro producto solo porque resulte conveniente.

Antes de mover un concepto a un producto, pregúntate:

* ¿Esta responsabilidad pertenece aquí?
* ¿Este concepto es específico de la implementación?
* ¿Este concepto es específico de la documentación?
* ¿Este concepto es específico del diseño?
* ¿Este concepto es específico del ciclo de vida?
* ¿Seguiría teniendo sentido si el framework no existiera?

Si el concepto sigue teniendo sentido sin el framework, probablemente pertenezca primero a Design, Docs Standard o Method antes de pertenecer a Framework.

## Tradeoff aceptado

VSlices acepta un poco más de estructura de documentación a cambio de límites de producto más claros.

La suite debe sentirse conectada, pero no colapsada en un solo producto. Esto evita el acoplamiento prematuro y mantiene abierta la evolución futura.

## Principio

Los productos deben separarse por responsabilidad. Los productos deben conectarse por continuidad.

VSlices es una suite porque el ciclo de vida está conectado. VSlices no es un solo producto porque cada problema del ciclo de vida merece su propia forma.
