# Terminar Method antes de expandir la documentación de Framework

## Estado

Accepted

## Contexto

VSlices v0.1-beta se centra actualmente en consolidar la base conceptual de la suite.

El trabajo pendiente más relevante es completar y estabilizar:

* VSlices Method
* VSlices Design
* VSlices Docs Standard

Estos productos definen el lenguaje, la estructura y el modelo de continuidad que luego guían la documentación de Framework y los ejemplos de implementación.

Al mismo tiempo, VSlices Framework todavía necesita documentación más completa. Sin embargo, documentar Framework demasiado pronto puede crear inestabilidad si Method, Design y Docs Standard aún están cambiando.

La documentación de Framework debe derivarse de un modelo de ingeniería más claro, no escribirse independientemente de él.

## Decisión

Terminaremos la base v0.1-beta para Method, Design y Docs Standard antes de expandir en profundidad la documentación de Framework.

La documentación de Framework puede seguir avanzando en paralelo solo cuando esté directamente respaldada por conceptos estables ya definidos por los otros productos. La prioridad inmediata es:

* completar Method
* alinear Design con Method
* alinear Docs Standard con Method y Design
* usar la estructura resultante para guiar la documentación de Framework

## Fundamento

Framework es el producto de VSlices orientado a la implementación, pero no debe definir la suite por sí solo.

VSlices está destinado a preservar la continuidad entre:

* descubrimiento
* documentación
* razonamiento de diseño
* arquitectura
* implementación
* evolución

Debido a eso, la documentación de Framework debería explicar no solo APIs o abstracciones, sino también el razonamiento que hace útiles esas abstracciones.

- Completar Method primero le da a la documentación de Framework una base más clara.
- Completar Design primero le da a la documentación de Framework un mejor lenguaje de modelado.
- Completar Docs Standard primero le da a la documentación de Framework una mejor continuidad con la documentación viva.

## Consecuencias

### Consecuencias positivas

* La documentación de Framework será más coherente con el resto de la suite.
* VSlices v0.1-beta tendrá una base conceptual más sólida.
* El trabajo de documentación evitará duplicar o contradecir ideas de Method aún no terminadas.
* Los ejemplos futuros de Framework podrán referenciar Method, Design y Docs Standard de forma consistente.
* Pueden surgir caminos de adopción a partir de escenarios validados en lugar de inventarse demasiado pronto.

### Consecuencias negativas

* La documentación de Framework permanecerá incompleta un poco más de tiempo.
* Algunos conceptos de implementación pueden esperar un lenguaje de Method más claro.
* Los usuarios que solo buscan uso de Framework pueden no tener guía completa de inmediato.

### Tradeoff

Aceptamos una documentación de Framework más lenta en el corto plazo para preservar una mayor coherencia de la suite en el mediano plazo.

## Estrategia de validación

Esta decisión se validará mediante los próximos proyectos de Alive Lab:

* generador de documentación Slice-First
* análisis Problem-First sin Framework
* exploración Context-First de Surreal Knowledge Manager / Surreal Atlas
* desarrollo Problem-First usando Framework en Domus Orbis

Cada proyecto debería aportar retroalimentación sobre:

* Method
* Design
* Docs Standard
* documentación de Framework
* futuros Adoption Paths

## Notas

Esta decisión no bloquea todo el trabajo de Framework.

Solo evita que la documentación de Framework se convierta en el impulsor principal antes de que la base conceptual de v0.1-beta esté estable.

La documentación de Framework debe continuar cuando ayude a explicar o validar conceptos ya definidos.
