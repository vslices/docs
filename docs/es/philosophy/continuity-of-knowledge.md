# La continuidad del conocimiento

## Propósito

Este documento explica uno de los fundamentos filosóficos centrales de VSlices:

> El software se degrada cuando el conocimiento que lo creó deja de ser visible, compartido y evolutivo.

VSlices existe porque el software no se construye solo a partir de código. El software se construye a partir de:

* comprensión del dominio
* lenguaje de negocio
* decisiones
* restricciones
* procesos
* comportamientos esperados
* intención arquitectónica
* detalles de implementación

El código es una expresión de ese conocimiento. No es todo el conocimiento.

## Los negocios operan a través del conocimiento

Un negocio no vive solo a través de su software, sus servicios, sus bases de datos o sus workflows.

Esos son expresiones de algo más profundo. Un negocio opera a través del conocimiento:

* lo que la organización entiende
* lo que las personas deciden
* qué reglas deben seguirse
* qué restricciones existen
* qué necesitan los clientes
* qué procesos deben ocurrir
* qué riesgos se aceptan
* qué intenciones guían los cambios futuros

El software se vuelve valioso cuando preserva y ejecuta parte de ese conocimiento. Pero se vuelve frágil cuando su conocimiento se pierde.

## El problema

Muchos sistemas no fallan solo porque el código sea malo. Fallan porque el conocimiento alrededor del código desaparece:

- El sistema puede seguir compilando.
- Las pruebas pueden seguir pasando.
- Los servicios pueden seguir ejecutándose.

Pero si el equipo ya no entiende:

* por qué existe un comportamiento
* por qué se tomó una decisión
* por qué importa una restricción
* por qué existe una excepción
* por qué se trazó un límite
* por qué un proceso funciona de la manera en que lo hace

Entonces el sistema se vuelve más difícil de evolucionar con seguridad.

En ese punto, el equipo no solo está manteniendo software. El equipo está redescubriendo conocimiento olvidado.

## Conocimiento congelado

Un fallo común es documentar todo por adelantado como si el dominio no fuera a cambiar. Esto crea conocimiento congelado. La documentación puede ser detallada, pero lentamente deja de representar la realidad:

- El negocio cambia.
- Las reglas cambian.
- El lenguaje cambia.
- Los usuarios cambian.
- La arquitectura cambia.
- El software cambia.

Pero la documentación permanece como una imagen de un sistema más antiguo.

En este caso, la documentación no preserva continuidad. Preserva una captura.

## Conocimiento encapsulado

El fallo opuesto es no documentar nada y confiar en que el código será suficiente. Esto crea conocimiento encapsulado, un conocimiento que todavía existe, pero está encerrado dentro de:

- detalles de implementación
- supuestos implícitos
- convenciones de nomenclatura
- historial de tickets
- conversaciones antiguas
- la memoria de personas que quizá ya no estén presentes

El código puede ejecutar una decisión, mostrar lo que ocurre, sugerir cómo funciona algo. Pero el código rara vez explica lo suficiente por sí solo:

* por qué existe la decisión
* qué alternativas fueron rechazadas
* qué tensión de negocio la creó
* qué riesgo se aceptó
* qué tradeoff se eligió
* qué cambio futuro debe manejarse con cuidado

Pero cuando aparecen las consecuencias del conocimiento olvidado, la mayoría de los ingenieros se da cuenta:

- Instruir software no es lo mismo que enseñar a las personas.
- Programar no es lo mismo que hablar.
- Un lenguaje de programación, incluso uno simple, no es un lenguaje natural.

## La IA hace más fácil escribir, no automática la continuidad

El auge de la IA hace que la documentación sea más fácil de producir que nunca. Un equipo ahora puede generar:

* resúmenes
* guías
* diagramas
* explicaciones
* registros de decisión
* ejemplos
* documentación técnica

Con mucho menos esfuerzo de escritura que antes. Esto es útil. Pero escribir más fácil no crea automáticamente mejor continuidad del conocimiento. IA can help with writing, organization or even summarization.

Pero la IA no elimina la responsabilidad de ingeniería de decidir:

* qué conocimiento importa
* qué debe preservarse
* qué debe conectarse
* qué debe validarse
* qué cambió
* qué debe seguir siendo visible durante la evolución futura

El problema ya no es solo si la documentación puede producirse.

El problema más difícil es si la documentación preserva el conocimiento correcto en la estructura correcta en el momento correcto.

## La modernización no es reinvención

Modernización y reinvención no son lo mismo. La modernización ocurre cuando un sistema evoluciona preservando el conocimiento que le da significado. La reinvención ocurre cuando el conocimiento se perdió y el equipo debe redescubrir lo que la organización ya sabía.

Muchas reescrituras no son causadas solo por código malo, frameworks viejos o infraestructura obsoleta; ocurren porque el sistema ya no puede entenderse. El conocimiento de negocio todavía existe en algún lugar, pero está fragmentado entre:

* personas
* tickets antiguos
* documentos desactualizados
* reglas implícitas
* comportamiento de producción
* estructuras de base de datos
* código fuente
* convenciones accidentales

Cuando esto ocurre, reconstruir el sistema se convierte en un proyecto de recuperación de conocimiento disfrazado de proyecto de modernización técnica.

## La posición de VSlices

VSlices no existe para crear más documentación. VSlices existe para preservar continuidad.

El objetivo no es documentarlo todo. Es mantener conectado el conocimiento importante a través de:

* descubrimiento del dominio
* documentación
* diseño
* arquitectura
* implementación
* evolución

VSlices trata:

- la documentación como diseño vivo.
- la implementación como conocimiento ejecutable.
- la arquitectura como una estructura evolutiva que debe permanecer cerca del dominio.
- la evolución del software como un problema de continuidad, no solo de entrega.

## Qué intenta preservar VSlices

VSlices intenta preservar:

* intención del dominio
* lenguaje de negocio
* comportamientos esperados
* errores explícitos
* decisiones importantes
* límites arquitectónicos
* capacidades
* casos de uso
* procesos
* caminos de evolución

El objetivo no es la documentación perfecta. Es un significado recuperable.

Un equipo futuro debería poder entender no solo qué hace el sistema, sino por qué llegó a ser así y cómo puede seguir evolucionando sin perder su intención original.

## Conclusión

El software no es solo un artefacto técnico. El software es una expresión viva del conocimiento acumulado.

Cuando ese conocimiento deja de fluir, el sistema comienza a degradarse, y cuando ese conocimiento permanece visible, conectado y evolutivo, el sistema puede cambiar sin perderse a sí mismo.

VSlices existe para apoyar esa continuidad.
