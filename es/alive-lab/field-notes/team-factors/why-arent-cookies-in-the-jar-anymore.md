# ¿Por qué ya no hay galletas en el tarro?

*Cuando se concede autonomía sin límites de seguridad*

## Definición

> Un patrón en el que ingenieros sin suficiente experiencia reciben responsabilidades, permisos o autonomía más allá de su entendimiento actual, sin supervisión, revisión o mecanismos de seguridad suficientes.
>
> Cuando los errores finalmente ocurren, el foco suele desplazarse hacia la persona que cometió el error en lugar de mirar el entorno que hizo posible que el error ocurriera.
>
> Las fallas resultantes suelen tratarse como sorpresas a pesar de haber sido completamente predecibles.

## Contexto

Este patrón suele aparecer cuando ingenieros junior comienzan a recibir propiedad sobre sistemas de producción, infraestructura, permisos o procesos críticos de negocio. La intención suele ser positiva:

* acelerar el crecimiento
* aumentar la autonomía
* reducir la dependencia de ingenieros senior

Sin embargo, el nivel de responsabilidad frecuentemente crece más rápido que el entendimiento que el ingeniero tiene del sistema.

La organización asume competencia y seguridad en las acciones del profesional. Ninguna de esas suposiciones fue validada por otro ingeniero con conocimiento profundo.

## Comportamiento observado

Se observaron varios patrones recurrentes:

* Se concedía acceso sin límites claros.
* Se ejecutaban operaciones sin entender su impacto completo.
* La documentación estaba incompleta o no estaba disponible.
* Los riesgos potenciales no se comunicaban.
* Las revisiones se omitían para cambios aparentemente simples.
* Las salvaguardas existentes estaban ausentes o eran insuficientes.

El ingeniero sabía lo suficiente para ejecutar la tarea exitosamente. Pero no para predecir sus consecuencias.

## Señales comunes

Posibles indicadores de que este patrón está ocurriendo:

* "Solo haz el cambio, es trabajo de 5 minutos, como medio *story point*."

  * "De hecho, ¿por qué eso es una historia de Jira? No amerita tanto."
* Acceso a producción concedido temprano sin supervisión.
* Falta de revisión para cambios de infraestructura o seguridad.
* Operaciones críticas ejecutadas por un solo ingeniero sin suficiente experiencia.
* Sin estrategia de *rollback*.
* Sin ambiente de *staging*.
* Límites de propiedad poco claros.
* Dependencia de conocimiento tribal.

## Tensiones subyacentes

### Autonomía vs guía

> Independencia sin apoyo no es autonomía. Es abandono.

### Confianza vs verificación

> La confianza no debería eliminar la revisión.

### Responsabilidad vs capacidad

> La responsabilidad puede asignarse más rápido de lo que la competencia puede desarrollarse.

### Crecimiento vs seguridad

> Los ingenieros aprenden a través de errores. Los sistemas deberían estar diseñados para sobrevivirlos.

## Consecuencias

### Corto plazo

* Incidentes inesperados.
* Correcciones de emergencia.
* Inestabilidad en producción.
* Ingenieros senior arrastrados a esfuerzos de recuperación.

### Largo plazo

* Pérdida de confianza.
* Miedo a hacer cambios.
* Menor disposición a tomar propiedad.
* Silos de conocimiento.
* Mayor riesgo organizacional.

Irónicamente, el ingeniero suele aprender la lección, pero la organización rara vez aprende la suya.

## Impacto en ingeniería

* Los sistemas de producción se vuelven frágiles cuando acciones críticas pueden ejecutarse sin revisión, contexto o salvaguardas adecuadas.
* Los incidentes se vuelven más probables cuando los permisos se conceden más rápido de lo que se desarrolla el entendimiento.
* Los cambios aparentemente simples pueden producir consecuencias inesperadas porque las dependencias ocultas no son visibles.
* Los ingenieros junior pueden perder confianza cuando errores normales de aprendizaje generan daños desproporcionados.
* Los ingenieros senior son arrastrados a recuperación de emergencia en lugar de mentoría planificada o trabajo de diseño.
* Los equipos pueden volverse más restrictivos después de incidentes, reduciendo autonomía en lugar de mejorar seguridad.
* La propiedad se vuelve confusa cuando las personas son responsables de sistemas que todavía no entienden profundamente.
* Las revisiones pierden efectividad cuando los cambios riesgosos se tratan como demasiado pequeños para merecer atención.
* El conocimiento operacional permanece tribal porque el error revela conocimiento que debió haberse vuelto explícito antes.
* La entrega se ralentiza después de incidentes evitables porque la confianza debe reconstruirse.
* La organización puede culpar a la persona que disparó la falla en lugar de arreglar el sistema que permitió que fuera peligrosa.
* El aprendizaje se asocia con miedo cuando los errores se castigan en lugar de contenerse.

Cuando se concede autonomía sin límites de seguridad, la organización no está acelerando el crecimiento. Está aumentando el radio de explosión de la inexperiencia. El objetivo no debería ser evitar que los ingenieros junior cometan errores, sino evitar que errores ordinarios se conviertan en incidentes graves.

## Posibles intervenciones

* Definir qué acciones requieren supervisión, revisión o aprobación antes de ejecutarse.
* Conceder permisos progresivamente según entendimiento, recuperabilidad y riesgo.
* Usar *staging*, *sandboxes* o ambientes de prueba antes de permitir cambios en producción.
* Requerir planes de *rollback* para operaciones de infraestructura, datos, seguridad o producción.
* Agregar listas de verificación para tareas riesgosas recurrentes como despliegues, migraciones o cambios de configuración.
* Emparejar ingenieros sin suficiente experiencia con ingenieros senior para cambios de alto impacto.
* Documentar dependencias ocultas, restricciones operacionales y riesgos conocidos cerca del sistema afectado.
* Tratar los "cambios simples" como riesgosos cuando su impacto no se entiende por completo.
* Hacer explícitos los límites de propiedad antes de asignar responsabilidad.
* Usar revisión de código, revisión de cambios o revisión operacional como mecanismos de seguridad, no como señales de desconfianza.
* Diseñar sistemas para que los errores comunes sean recuperables.
* Después de un incidente, preguntar qué barrera de seguridad habría reducido el radio de explosión.
* Evitar conceder acceso solo porque alguien necesita completar una tarea rápidamente.
* Enseñar las consecuencias de las acciones antes de esperar ejecución independiente.
* Reemplazar la culpa por mejora del sistema: ¿qué hizo que este error fuera posible, peligroso o difícil de detectar?

Una intervención útil es preguntar: "¿Cuál es el peor resultado razonable si esta persona comete aquí un error normal de aprendizaje?"

Esa pregunta ayuda a diseñar autonomía con límites en lugar de autonomía mediante abandono.

## Preguntas de reflexión

* ¿Quién revisó esta decisión?
* ¿Qué salvaguardas existían antes del cambio?
* ¿El ingeniero estaba preparado para esta responsabilidad?
* ¿Un ingeniero senior habría cometido el mismo error sin contexto?
* ¿Qué conocimiento se asumió pero nunca se enseñó?
* ¿Qué impidió que este error se detectara antes?
* Si esta falla era predecible, ¿por qué el sistema quedó expuesto a ella?

## Reflexión final

Tener tu propio ingeniero junior es como tener un hijo: **no lo abandones**. Cuando no lo estás mirando, está comiendo galletas... digo, rompiendo producción.

La reacción inmediata suele ser:

> "¿Quién hizo este cambio?"

Una pregunta más útil podría ser:

> "¿Por qué este cambio era posible en primer lugar?"

El ingeniero cometió un error; el entorno hizo que ese error fuera peligroso.

Se supone que los ingenieros junior cometen errores. Los sistemas, procesos y equipos deberían diseñarse teniendo esa realidad en mente.

Porque cuando las galletas desaparecen del tarro, el verdadero misterio rara vez es quién se las comió. El verdadero misterio es por qué nadie estaba mirando la cocina.
