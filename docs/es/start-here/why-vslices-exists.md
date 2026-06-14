# Por qué existe VSlices

## Una brecha de conexión del conocimiento

El camino de la ingeniería de software no consiste solo en escribir código. Antes del código hay comprensión y, para que esa comprensión sea útil, se necesita educación.

Pero la educación en ingeniería de software puede ser enredada. Esto no ocurre necesariamente porque el sistema educativo sea malo, o porque a las personas no les importe lo suficiente. Ocurre porque la vida es más grande que las horas que pasamos estudiando, las tareas que completamos o los proyectos que se nos pide construir.

Cuando alguien sale de la universidad, de un bootcamp o de cualquier otro entorno de aprendizaje, gran parte del conocimiento que lleva consigo suele quedar desconectado. Los conceptos se aprenden en secuencia, pero no siempre en relación entre sí.

La arquitectura, el diseño, la documentación, las pruebas, el modelado del dominio, los paradigmas de programación, la infraestructura y la forma de pensar el producto pueden enseñarse o descubrirse como piezas separadas. Con el tiempo, la experiencia empieza a conectar esas piezas.

Pero esa conexión suele ser personal, implícita y difícil de transferir; hay una diferencia entre saber y entender.

VSlices existe porque la propia ingeniería de software no es solo una secuencia de inventos completamente nuevos. También es una larga historia de descubrimientos, redescubrimientos, refinamientos y conexiones entre ideas que ya estaban ahí.

VSlices es un intento de hacer explícitas esas conexiones.

## Un problema de continuidad

Muchos proyectos de software sufren una brecha de continuidad. Los equipos descubren el dominio en un lugar, lo documentan en otro, discuten la arquitectura en otro y luego implementan el sistema en código que puede no preservar el razonamiento original.

El resultado de esto puede no ser siempre visible al principio, pero con el tiempo el sistema se vuelve más difícil de explicar, más difícil de cambiar y más difícil de confiar.

- La documentación puede alejarse de la implementación.
- La arquitectura puede desconectarse de las necesidades reales del dominio.
- El código puede contener intención de negocio que no es visible en ningún otro lugar.
- Las decisiones pueden tomarse una vez, pero su razonamiento puede desaparecer.

VSlices existe para reducir esa brecha.

## Un problema de contexto de IA

La ingeniería de software está entrando en un período en el que el código ya no lo escriben exclusivamente los humanos. Los Large Language Models pueden generar arquitecturas, implementaciones, pruebas, documentación y propuestas de diseño en segundos.

Esto cambia cómo se produce el software, pero no elimina la necesidad de ingeniería. En muchos casos, incluso la aumenta, porque los sistemas de IA generan resultados basados en:

- su entrenamiento
- la información disponible en el contexto actual
- y las restricciones proporcionadas explícitamente

Cuando el conocimiento del dominio, la intención arquitectónica, las reglas de negocio y las decisiones de ingeniería son implícitos, fragmentados o no están documentados, los sistemas de IA se ven obligados a llenar los huecos usando supuestos. A veces esos supuestos son útiles y a veces no lo son.

El desafío no es que la IA genere código, sino asegurarse de que el código generado refleje las necesidades reales, las restricciones y las intenciones del sistema que se está construyendo.

VSlices existe para hacer esas intenciones más explícitas.

## Un problema de complejidad progresiva

Los proyectos de software suelen moverse entre dos extremos.

- Algunos proyectos introducen demasiada arquitectura demasiado pronto.
> Comienzan con capas, patrones, abstracciones, convenciones y decisiones de infraestructura antes de que el dominio haya demostrado que esas decisiones son necesarias.
- Otros proyectos evitan la estructura durante demasiado tiempo.
> Comienzan simples, pero a medida que el sistema crece, el comportamiento se vuelve implícito, los límites se vuelven difusos y los cambios se vuelven más difíciles de razonar.

La mayoría de las veces, el problema no es que los equipos tomen malas decisiones a propósito. El problema es que no pueden saber por completo cómo crecerá el dominio.

Por supuesto, no podemos ver el futuro, pero sí podemos razonar sobre el uso esperado, la evolución probable, la presión operativa y cómo el sistema puede afectar a distintas partes de una organización en el corto y largo plazo.

VSlices existe para apoyar la complejidad progresiva.

## Un problema de comportamiento oculto

En muchos sistemas, el comportamiento importante no es explícito.

- Las reglas de negocio pueden estar ocultas dentro de servicios.
- Los errores esperados pueden representarse como excepciones en tiempo de ejecución.
- Las dependencias pueden asumirse en lugar de declararse.
- Los efectos secundarios pueden aparecer en lugares donde la intención del dominio es difícil de ver.

Con el tiempo, esto hace que el sistema sea más difícil de entender y más difícil de cambiar con seguridad.

VSlices existe para hacer el comportamiento más explícito.
