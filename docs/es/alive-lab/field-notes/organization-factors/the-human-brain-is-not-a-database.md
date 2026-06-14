# El cerebro humano no es una base de datos

*Cuando el conocimiento organizacional vive en la memoria en lugar de vivir en estructura*

## Definición

> Un patrón en el que las organizaciones acumulan gradualmente suficiente conocimiento, reglas, procesos, excepciones y dependencias como para que operar correctamente dependa principalmente de lo que las personas recuerdan, en lugar de lo que el sistema comunica explícitamente.
>
> Con el tiempo, el conocimiento crítico termina distribuido entre conversaciones, reuniones, correos, documentos, individuos y conocimiento tribal.
>
> La organización sigue operando, pero solo porque las personas compensan la estructura faltante mediante memoria.

## Contexto

Este patrón suele emerger durante años de crecimiento. Ninguna decisión individual crea el problema; la complejidad se acumula gradualmente a través de:

* decisiones no documentadas
* casos especiales
* excepciones organizacionales
* conocimiento histórico
* evolución de procesos
* cambios de personal
* comunicación informal

Cada adición individual parece inofensiva. En conjunto, eventualmente exceden lo que las personas pueden recordar razonablemente.

## Comportamiento observado

Se observaron varios patrones recurrentes:

* El conocimiento crítico existía solo en individuos específicos.
* La documentación se volvió incompleta u obsoleta.
* Los ingenieros dependían de la memoria para hacer cambios de forma segura.
* Las personas nuevas requerían una incorporación extensa.
* Las personas existentes tenían dificultades para explicar el sistema completo.
* Preguntas similares se hacían y respondían repetidamente.
* Entender un cambio requería conversaciones con múltiples personas.

La organización seguía funcionando. La documentación no.

## Señales comunes

Posibles indicadores de que este patrón está ocurriendo:

* "Pregúntale a esa persona, sabe cómo funciona."
* "Hay un documento en alguna parte."
* **"Necesitas contexto histórico para entender esto."**
* "Depende."
* "Antes de cambiar esto, habla con estas cinco personas."
* Nadie entiende el proceso completo.
* La incorporación toma meses.
* El conocimiento se redescubre con frecuencia.
* Los ingenieros tienen miedo de modificar sistemas existentes.

## Tensiones subyacentes

### Conocimiento vs memoria

> El conocimiento debería sobrevivir a la ausencia de la persona que lo descubrió.

### Flexibilidad vs explicitud

> Cada excepción no documentada se convierte en algo que alguien debe recordar.

### Crecimiento vs comprensión

> Los sistemas suelen volverse más complejos más rápido de lo que las personas pueden entenderlos.

### Velocidad vs sostenibilidad

> Moverse rápido hoy suele crear deuda de conocimiento mañana.

## Consecuencias

### Corto plazo

* Toma de decisiones rápida.
* Menor esfuerzo documental.
* Flexibilidad.
* Adaptación rápida.

### Largo plazo

* Silos de conocimiento.
* Mayor tiempo de incorporación.
* Mayor *bus factor*.
* Miedo al cambio.
* Menor predictibilidad.
* Mayor dependencia de individuos específicos.
* Fragilidad organizacional.

Irónicamente, la organización suele creer que está ahorrando tiempo al evitar documentación y gestión del conocimiento.

Después gasta mucho más tiempo buscando información del que originalmente ahorró.

## Impacto en ingeniería

* Los cambios se vuelven más lentos porque entender el sistema requiere conversaciones antes de que la implementación pueda comenzar.
* Los ingenieros evitan modificar partes del sistema porque las reglas reales no son visibles en código, pruebas o documentación.
* La incorporación depende de transmisión oral en lugar de caminos de aprendizaje estructurados.
* Las decisiones técnicas pierden su razonamiento original, haciendo que los cambios futuros sean más difíciles de evaluar.
* Problemas similares se resuelven repetidamente porque el conocimiento previo no es fácil de encontrar.
* La arquitectura se vuelve más difícil de evolucionar porque las dependencias ocultas y excepciones históricas no son explícitas.
* Las revisiones se vuelven menos confiables porque quienes revisan pueden no saber qué reglas invisibles aplican.
* Los incidentes tardan más en diagnosticarse cuando el conocimiento operacional está distribuido entre personas en lugar de artefactos.
* El *bus factor* aumenta a medida que individuos específicos se convierten en índices vivientes de la organización.
* Los equipos empiezan a tratar la complejidad como inevitable porque nadie puede ver de dónde vino.

Cuando el conocimiento vive solo en la memoria, el sistema real se vuelve más grande que el código base. El *software* puede ser ejecutable, pero la organización en sí no es comprensible sin entrevistar a las personas que sobrevivieron a su historia.

## Posibles intervenciones

* Identificar el conocimiento que se pregunta, redescubre o explica verbalmente de forma repetida.
* Empezar a documentar desde los puntos de fricción en lugar de intentar documentarlo todo.
* Reemplazar "pregúntale a esta persona" por "lee esto primero, luego pregunta si falta algo".
* Capturar el razonamiento detrás de decisiones importantes, no solo la decisión final.
* Documentar excepciones, casos especiales y restricciones históricas cerca del proceso o sistema que afectan.
* Crear caminos ligeros de incorporación para las áreas de confusión más comunes.
* Convertir explicaciones repetidas en documentación viva.
* Usar registros de decisión para elecciones cuyo contexto podría olvidarse más adelante.
* Hacer explícitas las dependencias ocultas en diagramas, notas, pruebas o estructura de código.
* Revisar documentación durante el trabajo real, no como una actividad ceremonial separada.
* Tratar la documentación obsoleta como un defecto del sistema, no como una falla personal.
* Emparejar a quienes poseen conocimiento con otras personas antes de que el conocimiento crítico se vuelva urgente.
* Preferir documentos pequeños y mantenibles por sobre documentos grandes en los que nadie confía.
* Conectar la documentación con propiedad, para que las personas sepan quién puede aclarar o evolucionar cada área.
* Preguntar después de cada incidente, traspaso o cambio difícil: "¿Qué necesitábamos saber que no estaba escrito en ninguna parte?"

El objetivo no es mover toda la organización a documentos. Es evitar que el conocimiento crítico dependa solo de la memoria.

## Preguntas de reflexión

* ¿Cuánto conocimiento crítico existe solo en la cabeza de las personas?
* ¿Podría una persona nueva entender este sistema sin entrevistar a medio equipo?
* ¿Qué ocurre cuando se va la persona que más sabe?
* ¿Con qué frecuencia se responden las mismas preguntas repetidamente?
* ¿El conocimiento se está almacenando o solo se está recordando?
* ¿Estamos construyendo sistemas que las personas entienden o sistemas que las personas memorizan?
* ¿Qué información se perdería si todo el equipo desapareciera mañana?

## Reflexión final

La mayoría de las organizaciones no fallan porque sus personas sean incapaces. Fallan porque esperan que las personas recuerden más de lo que una persona puede recordar razonablemente.

* Cada excepción.
* Cada caso especial.
* Cada decisión no documentada.
* Cada dependencia oculta.
* Cada conversación olvidada.

Eventualmente, el problema ya no es técnico. El problema es biológico.

La memoria humana es notable, pero finita.

> El cerebro humano es una herramienta extraordinaria para razonar.
>
> Es un lugar terrible para almacenar una organización.
