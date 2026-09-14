# Espera... ¿ese niño está bebiendo vodka?

> ¿Cómo que "*otra vez*"?

*Cuando la responsabilidad crece más rápido que la mentoría*

## Definición

> Un patrón en el que se espera que ingenieros sin suficiente experiencia tomen decisiones, operen sistemas, resuelvan problemas y asuman responsabilidades más allá de su nivel actual de entendimiento, sin la guía necesaria para desarrollar esas capacidades de forma segura.
>
> Cuando los errores finalmente ocurren, el foco suele desplazarse hacia la persona en lugar de mirar el entorno que creó las condiciones para que el error ocurriera.
>
> Las fallas resultantes suelen tratarse como inesperadas, a pesar de ser completamente predecibles.

## Contexto

Este patrón suele aparecer en organizaciones donde la presión por entregar toma prioridad de forma constante sobre la mentoría.

La organización suele creer que la transferencia de conocimiento, la incorporación y el acompañamiento pueden ocurrir orgánicamente mientras el trabajo normal continúa sin interrupciones. A diferencia del sueño de cualquier inversionista, eso no ocurre.

Los ingenieros senior se vuelven cada vez más ocupados manteniendo compromisos de entrega, mientras los ingenieros junior reciben progresivamente más responsabilidad con progresivamente menos guía.

La intención rara vez es maliciosa. Las motivaciones comunes pueden incluir:

* acelerar la entrega
* reducir la dependencia de personas clave
* aumentar la autonomía
* reducir cuellos de botella
* escalar la capacidad del equipo

Lamentablemente, la capacidad rara vez crece a la misma velocidad que la responsabilidad.

## Comportamiento observado

Se observaron varios patrones recurrentes:

* Los ingenieros junior recibían responsabilidades para las que aún no estaban preparados.
* El contexto importante existía solo en la mente de ingenieros senior.
* La mentoría ocurría de forma reactiva en lugar de intencional.
* Las preguntas se postergaban porque todo el mundo estaba ocupado.
* La transferencia de conocimiento se volvía menos prioritaria que la entrega.
* Se tomaban decisiones críticas sin contexto suficiente.
* Los ingenieros aprendían a través de incidentes en producción en lugar de guía.

La organización esperaba crecimiento. El entorno entregaba exposición.

No son lo mismo.

## Señales comunes

Posibles indicadores de que este patrón está ocurriendo:

* "Ya lo va a resolver."
* "Solo dale acceso."
* "Ahora no tenemos tiempo para capacitación."
* "Es un cambio simple."
* "Pregunta si tienes dudas."
* Conocimiento crítico concentrado en pocas personas.
* Incorporación altamente dependiente de conocimiento tribal.
* Ingenieros junior con miedo de hacer preguntas.
* Ingenieros senior constantemente demasiado ocupados para mentorear.
* Aprendizaje ocurriendo principalmente a través de errores.

## Tensiones subyacentes

### Entrega vs mentoría

> Cada hora invertida en enseñar parece reducir la entrega de corto plazo. Hasta que la falta de enseñanza empieza a reducir la entrega mucho más.

### Responsabilidad vs capacidad

> La responsabilidad puede asignarse de inmediato. La capacidad requiere tiempo.

### Autonomía vs abandono

> Independencia sin apoyo no es empoderamiento. Es negligencia.

### Exposición vs desarrollo

> La exposición crea oportunidades para aprender. El desarrollo requiere guía.

## Consecuencias

### Corto plazo

* Delegación de tareas más rápida.
* Menor dependencia inmediata de ingenieros senior.
* Mayor percepción de escalabilidad del equipo.

### Largo plazo

* Errores repetidos.
* Sistemas frágiles.
* Miedo a tomar propiedad.
* Incorporación lenta.
* Silos de conocimiento.
* Sobrecarga de ingenieros senior.
* Dependencia organizacional del conocimiento tribal.

Irónicamente, la organización suele ahorrar tiempo evitando la mentoría. Después gasta mucho más tiempo recuperándose de las consecuencias.

## Impacto en ingeniería

* Los cambios críticos se vuelven más riesgosos porque las personas que los ejecutan pueden no entender el contexto circundante.
* Los errores se vuelven más probables cuando la responsabilidad se asigna sin conocimiento, revisión o apoyo equivalentes.
* Los incidentes en producción pueden tratarse como fallas individuales, aunque el sistema los haya vuelto predecibles.
* Los ingenieros senior permanecen sobrecargados porque la mentoría se postergó hasta que los problemas se volvieron urgentes.
* Los ingenieros junior pueden desarrollar miedo a tomar propiedad después de quedar expuestos a consecuencias que no estaban preparados para manejar.
* Los silos de conocimiento se fortalecen cuando los ingenieros senior están demasiado ocupados para enseñar y los ingenieros junior deben inferir contexto.
* Las revisiones de código se vuelven insuficientes si quienes revisan asumen conocimiento que nunca fue enseñado.
* La velocidad de entrega se vuelve frágil porque la delegación de corto plazo crea retrabajo de largo plazo.
* La arquitectura se vuelve más difícil de evolucionar cuando solo unas pocas personas entienden por qué el sistema funciona como funciona.
* La capacidad del equipo parece aumentar, pero la capacidad real permanece subdesarrollada.
* La incorporación se vuelve inconsistente porque el crecimiento depende de suerte, cercanía y conversaciones informales.
* La organización puede confundir exposición a responsabilidad con desarrollo de competencia.

Cuando la mentoría está ausente, el sistema no deja de enseñar. Simplemente enseña a través de errores, incidentes, miedo y retrabajo. Ese tipo de aprendizaje es caro, desigual y muchas veces dañino.

## Posibles intervenciones

* Definir qué responsabilidades son seguras para que el ingeniero tome de forma independiente.
* Identificar qué responsabilidades requieren *pairing*, revisión o supervisión.
* Hacer de la mentoría una responsabilidad explícita, no un efecto secundario accidental de la entrega.
* Crear niveles progresivos de responsabilidad en lugar de asignar propiedad crítica de una sola vez.
* Emparejar ingenieros junior con ingenieros experimentados en trabajo de alto contexto o alto riesgo.
* Documentar el contexto necesario para tomar decisiones seguras en áreas críticas.
* Incentivar preguntas antes de que los errores se vuelvan la única fuente de *feedback*.
* Reemplazar "pregunta si tienes dudas" por guía programada, puntos de control y momentos de revisión.
* Tratar errores repetidos como señales de falta de apoyo, no solo como problemas de desempeño individual.
* Dar acceso de forma progresiva y conectar el acceso con entendimiento, recuperabilidad y revisión.
* Usar listas de verificación para operaciones peligrosas, despliegues, migraciones o cambios en producción.
* Hacer visible la carga de mentoría de los ingenieros senior al planificar capacidad.
* Proteger tiempo para enseñar antes de que la falta de enseñanza se convierta en retrabajo.
* Después de un incidente, preguntar qué conocimiento, barrera de seguridad o guía habría hecho menos probable el error.
* Medir el crecimiento por aumento de criterio, no solo por aumento de tareas asignadas.

Una intervención útil es preguntar: "¿Qué necesitaría entender esta persona antes de que esta responsabilidad sea segura?"

Esa pregunta desplaza el foco desde la culpa hacia el desarrollo de capacidad.

## Preguntas de reflexión

* ¿Quién es responsable de enseñar a este ingeniero?
* ¿Cuándo fue la última sesión de mentoría intencional?
* ¿Qué conocimiento se asume pero nunca se explica?
* ¿Qué decisiones críticas puede tomar este ingeniero de forma segura?
* ¿Un error en esta área sería recuperable?
* ¿La autonomía se está desarrollando o solo se está asignando?
* ¿Qué pasaría si la persona que más sabe se fuera mañana?
* ¿Estamos creando futuros seniors o consumiendo a los actuales?

## Reflexión final

Cuando la gente ve a un niño bebiendo vodka, la reacción inmediata suele ser:

> "¿Por qué ese niño está bebiendo vodka?"

Una pregunta más útil podría ser:

> "¿Por qué el vodka estaba disponible para el niño en primer lugar?"

Se supone que los ingenieros junior van a:

* cometer errores
* hacer preguntas
* no saber cosas
* pedir vodka

  * incluso si estamos en horario laboral

Nada de eso es una falla.

La falla ocurre cuando una organización espera que la competencia emerja sin crear las condiciones necesarias para desarrollarla.

Los niños no se vuelven adultos por accidente. Los ingenieros tampoco se vuelven seniors por accidente.

> Si nadie tuvo tiempo para enseñar, eventualmente alguien tendrá tiempo para arreglar.
