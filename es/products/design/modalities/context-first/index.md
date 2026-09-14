# Context-First

_Context-First_ es una modalidad de VSlices Design que prioriza el entendimiento amplio del dominio antes de definir artefactos concretos de *software*.

Es útil cuando el equipo necesita entender el contexto de negocio antes de decidir qué debería construirse, mejorarse, automatizarse, integrarse o modernizarse.

_Context-First_ asume que la estructura de *software* debería emerger progresivamente desde el entendimiento del dominio.

No parte desde una arquitectura preferida, un patrón técnico, un modelo de base de datos, una pantalla, una API o una lista de *features*. Parte desde el contexto.

## Definición

_Context-First_ es una modalidad de diseño donde el equipo construye una base contextual fuerte antes de avanzar hacia la implementación.

En la metáfora de la pirámide, _Context-First_ da más peso a la base que a la altura.

```text
base / height -> large
```

Esto significa que el equipo invierte más esfuerzo en Understanding y Contextualizing antes de Planning y Building.

El objetivo no es analizar para siempre. Es reducir la incertidumbre contextual lo suficiente para que las decisiones de implementación sean más seguras, claras y trazables.

## Cuándo usarlo

Usa _Context-First_ cuando el dominio todavía no está lo suficientemente claro como para definir estructura de *software* con seguridad.

Es especialmente útil cuando:

* el proceso de negocio es poco claro o fragmentado
* participan varios departamentos, áreas, roles o actores externos
* el trabajo ocurre actualmente mediante procesos manuales o semimanuales
* el sistema modernizará o reemplazará un *workflow* existente
* la organización depende de conocimiento implícito que no está documentado
* distintas áreas entienden el mismo proceso de forma diferente
* el equipo necesita descubrir límites antes de diseñar *features*
* el costo de construir algo incorrecto es alto
* las decisiones de implementación pueden afectar flujos adyacentes
* el trabajo técnico depende de entendimiento de negocio que todavía falta

_Context-First_ también es útil cuando el equipo está entrando a un dominio por primera vez.

## Cuándo no usarlo

_Context-First_ puede ser excesivo cuando:

* el dominio ya está bien entendido
* el cambio es pequeño y aislado
* el problema ya está claro y delimitado
* el equipo necesita *feedback* de implementación más que análisis adicional
* el riesgo de construir algo incorrecto es bajo
* una iteración previa ya creó suficiente base contextual
* el trabajo es principalmente técnico y no requiere descubrimiento amplio del dominio

En esos casos, Problem-First o Slice-First pueden ser más apropiados.

## Características

_Context-First_ normalmente tiene estas características:

* exploración amplia antes de planificación estrecha
* foco fuerte en lenguaje de dominio
* identificación temprana de actores, áreas, roles y responsabilidades
* atención a flujos existentes antes que a flujos objetivo
* descubrimiento de límites antes que estructura de implementación
* tratamiento explícito de incertidumbre y supuestos
* movimiento inicial más lento hacia la implementación
* trazabilidad más fuerte entre contexto de negocio y artefactos de *software*
* alta sensibilidad a procesos adyacentes e impacto organizacional

_Context-First_ no intenta modelar todo el negocio.

Intenta entender suficiente del contexto de negocio relevante para tomar mejores decisiones de diseño.

## Ventajas

_Context-First_ ayuda al equipo a:

* reducir implementación prematura
* evitar diseñar *features* desde requerimientos aislados
* mejorar el lenguaje compartido
* revelar dependencias ocultas
* detectar flujos adyacentes y responsabilidades afectadas
* descubrir límites de dominio
* entender por qué los procesos actuales se comportan como lo hacen
* identificar riesgos antes de que se vuelvan problemas de implementación
* producir artefactos de *software* respaldados por contexto de negocio
* reducir complejidad accidental causada por supuestos débiles

Es especialmente valioso cuando el mayor riesgo es malentender el negocio.

## Desventajas

_Context-First_ también tiene costos. Puede:

* ralentizar la entrega inicial
* requerir más acceso a expertos de dominio
* sentirse demasiado amplio para cambios pequeños o urgentes
* crear demasiados artefactos si no se mantiene progresivo
* derivar en parálisis por análisis si el equipo no define alcance
* retrasar el *feedback* de implementación
* volverse difícil de gestionar cuando la exploración no tiene criterio de detención

El principal peligro de _Context-First_ es confundir entendimiento con descubrimiento infinito. El equipo debería construir suficiente base para moverse con seguridad, no intentar eliminar toda incertidumbre posible antes de construir.
