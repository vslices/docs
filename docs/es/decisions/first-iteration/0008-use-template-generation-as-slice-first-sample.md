# 0008 - Usar la generación de templates como el primer sample Slice-First

## Estado

Accepted

## Contexto

La documentación de VSlices está creciendo a través de múltiples productos, versiones e idiomas.

Esto crea un problema de mantenimiento. Por ejemplo, una sola idea de documentación puede necesitar existir a través de:

* documentación en inglés
* documentación en español
* secciones específicas de producto
* documentación versionada
* archivos markdown generados
* páginas públicas de documentación

Mantener estos archivos manualmente crea trabajo duplicado y aumenta el riesgo de divergencia.

Al mismo tiempo, VSlices necesita ejemplos reales para validar su propio método, estándar de documentación, razonamiento de diseño y primitivas del framework.

El generador de documentación es un problema pequeño pero real observado dentro del propio VSlices. Debido a eso, es un candidato fuerte para el primer sample Slice-First.

## Decisión

Usaremos el generador de templates de documentación como el primer sample Slice-First para VSlices.

- El objetivo no es construir una plataforma de documentación completa.
- El objetivo es resolver el problema inmediato de generar artefactos de documentación consistentes a partir de una fuente de verdad más pequeña.

Este sample debe validar cómo VSlices aborda una slice concreta desde:

* problema observado
* necesidad de documentación
* razonamiento de diseño
* implementación
* retroalimentación
* evolución

## Fundamento

El generador es útil de inmediato. Apoya el trabajo actual v0.1 y reduce el mantenimiento manual de la documentación. También crea un escenario realista pero acotado para validar VSlices.

Esto lo hace mejor que un sample artificial. La slice es lo bastante pequeña para mantener el alcance controlado, pero lo bastante significativa para involucrar:

* estructura de documentación
* contenido fuente
* reglas de transformación
* markdown generado
* variantes de idioma
* retroalimentación de validación
* decisiones de implementación

## Definición de la slice

La slice inicial es:

> Generar archivos de documentación a partir de contenido de templates estructurado para reducir el mantenimiento manual duplicado en variantes de documentación.

La primera versión debe enfocarse en el workflow más pequeño útil:

* definir contenido fuente
* definir destinos de salida
* generar archivos markdown
* soportar al menos una estructura de documentación repetida
* mantener la salida generada legible y editable
* evitar features innecesarias de plataforma

## No objetivos explícitos

Esta decisión no compromete la construcción de:

* un CMS de documentación completo
* un editor visual
* una plataforma de localización completa
* un producto público
* un lenguaje de templates complejo
* un generador de sitios estáticos genérico
* un prototipo completo de Surreal Atlas

Eso solo puede convertirse en exploraciones futuras si la slice inicial valida la necesidad.

## Consecuencias

### Consecuencias positivas

* VSlices obtiene un ejemplo real de Slice-First.
* El mantenimiento de la documentación se vuelve más fácil.
* Los ejemplos de Framework pueden derivarse del uso interno real.
* Docs Standard puede validarse mediante restricciones de generación.
* Method puede probarse contra una ruta de implementación concreta.
* El sample puede informar más adelante Surreal Knowledge Manager o Surreal Atlas.

### Consecuencias negativas

* El generador puede distraer temporalmente de terminar v0.1-beta.
* Existe el riesgo de sobregeneralizar la herramienta demasiado pronto.
* Existe el riesgo de construir una plataforma en lugar de resolver el problema actual de documentación.
* La primera implementación puede necesitar reescribirse después de aprender del uso.

### Tradeoff

Aceptamos un pequeño esfuerzo de implementación ahora porque el generador resuelve un problema de documentación actual y proporciona un caso de validación Slice-First concreto.

No aceptamos expandir el generador más allá de la necesidad actual de documentación hasta que demuestre ser útil.

## Estrategia de validación

Esta decisión se validará si el generador ayuda a:

* reducir el trabajo duplicado de documentación
* mantener más consistentes las documentaciones en inglés y español
* generar salidas markdown útiles
* revelar mejores estructuras de Docs Standard
* producir ejemplos que puedan explicar VSlices Method y Framework
* soportar la documentación v0.1 sin aumentar la complejidad

Esta decisión se debilitará si:

* editar manualmente sigue siendo más fácil que generar
* los documentos generados se vuelven más difíciles de entender
* el generador requiere demasiada ceremonia
* la herramienta se vuelve más compleja que el problema de documentación
* la implementación bloquea el progreso de v0.1-beta

## Notas

El generador debe seguir los principios de VSlices:

* resolver primero un problema real
* mantener pequeña la primera slice
* preferir comportamiento explícito
* evitar magia oculta
* preservar documentación legible por humanos
* introducir complejidad progresivamente

El generador es una herramienta de validación antes que un producto.
