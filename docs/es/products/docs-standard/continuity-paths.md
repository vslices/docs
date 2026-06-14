# Caminos de continuidad

VSlices Docs Standard usa caminos de continuidad para explicar cómo se mueve el conocimiento entre documentos.

Un camino de continuidad muestra cómo una pieza de conocimiento puede descubrirse, documentarse, transformarse en decisiones, reflejarse en la implementación, validarse y evolucionar.

El objetivo no es forzar cada documento a seguir una secuencia fija. El objetivo es mantener conectado el conocimiento importante.

## Idea central

La documentación pierde valor cuando los documentos se vuelven aislados.

- Un Documento de contexto (_Context Document_ en inglés) puede explicar dónde está trabajando el equipo.
- Un Documento de proceso (_Process Document_ en inglés) puede explicar cómo se realiza el trabajo.
- Un Documento de caso de uso (_Use Case Document_ en inglés) puede explicar qué significa un comportamiento.
- Un Documento de capacidad (_Capability Document_ en inglés) puede explicar qué debe ser posible.
- Un Registro de decisión (_Decision Record_ en inglés) puede explicar por qué se eligió una dirección.
- Una Nota de validación (_Validation Note_ en inglés) puede explicar qué se aprendió.
- Un camino de continuidad conecta esos artefactos para que los lectores futuros puedan entender cómo evolucionó el conocimiento.

## Camino general

Un camino de continuidad común puede verse así:

```text
escenario
-> línea de trabajo
-> proceso
-> flujo 
-> caso de uso
-> capacidad
-> decisión
-> implementación
-> validación
-> actualización del conocimiento
```

Este camino es descriptivo, no obligatorio. Un equipo puede comenzar desde un scenario, un problema, un workflow, un use case, una decisión o una pequeña implementación.

Lo importante es que el conocimiento importante siga siendo trazable.

## Contribución de cada documento

Cada documento preserva una parte distinta del camino:

- __Vocabulario de dominio (_Domain Vocabulary_ en inglés)__: preserva el lenguaje necesario para entender el camino.
- __Documento de contexto (_Context Document_ en inglés)__: preserva el scenario y los work lines donde comienza el camino.
- __Documento de proceso (_Process Document_ en inglés)__: preserva cómo se organiza y se ejecuta el trabajo.
- __Documento de caso de uso (_Use Case Document_ en inglés)__: preserva el significado, la consecuencia, las validaciones y los errores esperados del comportamiento.
- __Documento de capacidad (_Capability Document_ en inglés)__: preserva capacidades estables que requiere el negocio o el sistema.
- __Registro de decisión (_Decision Record_ en inglés)__: preserva por qué se seleccionó una dirección y qué tradeoffs se aceptaron.
- __Nota de validación (_Validation Note_ en inglés)__: preserva evidencia, aprendizaje y cambios después de una revisión, implementación o uso.
- __Nota de soporte (_Support Note_ en inglés)__: preserva conocimiento temprano o incierto antes de que se vuelva estructurado.

## Ejemplo de camino: del scenario al comportamiento

Un equipo puede descubrir que una empresa tiene un scenario de reservas fragmentado.

El camino de continuidad puede convertirse en:

```text
Documento de contexto
-> define el scenario de reservas y los work lines involucrados.

Vocabulario de dominio
-> aclara términos como reserva, booking, cancelación y disponibilidad.

Documento de proceso
-> explica cómo se gestionan actualmente las reservas.

Documento de caso de uso
-> define qué significa confirmar una reserva.

Documento de capacidad
-> identifica la necesidad de validar disponibilidad.

Registro de decisión
-> explica por qué la validación de disponibilidad pertenece cerca de la confirmación de reserva.

Nota de validación
-> captura si el comportamiento implementado coincidió con las necesidades operativas reales.
```

El valor no está en la cantidad de documentos.

El valor está en que el comportamiento pueda rastrearse hasta el conocimiento que lo justificó.

## Ejemplo de camino: del aprendizaje al cambio

La continuidad también se mueve hacia atrás.

Una feature, una _slice_, una revisión o un comportamiento en producción puede revelar que la comprensión previa era incompleta.

El camino de continuidad puede convertirse en:

```text
Nota de validación
-> captura evidencia de que una regla se entendió mal.

Documento de caso de uso
-> actualiza el comportamiento esperado.

Documento de proceso
-> actualiza el workflow afectado por la regla.

Registro de decisión
-> reemplaza la decisión anterior.

Documento de contexto
-> actualiza el scenario si el aprendizaje cambia la comprensión más amplia.
```

Por eso la documentación debe apoyar la evolución.

La implementación no termina el aprendizaje.

A menudo crea mejores preguntas.

## Trazabilidad ligera

Las referencias simples son suficientes.

```md
Contexto relacionado:
- context.reservations

Proceso relacionado:
- process.reservation-management

Casos de uso relacionados:
- use-case.confirm-booking

Capacidad relacionada:
- capability.validate-availability

Decisiones relacionadas:
- decision.booking-validation-boundary

Validaciones relacionadas:
- validation.booking-feedback
```

Las referencias deberían ayudar a los lectores a moverse por el conocimiento.

No deberían convertirse en ruido administrativo.

## Cuándo crear referencias

Agrega referencias cuando mejoren la claridad. Las referencias útiles suelen conectar:

- __causa con consecuencia__: por qué existe un documento o una decisión.
- __comportamiento con contexto__: dónde obtiene significado un caso de uso.
- __decisión con evidencia__: qué respaldó o cuestionó una elección.
- __capacidad con comportamiento__: qué casos de uso requieren una capacidad.
- __validación con cambio__: qué aprendizaje afectó algo después de aparecer evidencia.

No agregues referencias solo porque una plantilla tenga un lugar para ellas.

## Principio de continuidad

Un camino de continuidad sigue un principio: __el conocimiento importante debe permanecer conectado con los artefactos y decisiones de los que depende__.

- Si un documento no puede explicar con qué se conecta, puede estar demasiado aislado.
- Si una implementación no puede rastrearse hasta el contexto, el comportamiento, la capacidad o la decisión, el equipo puede haber perdido la intención.
- Si la validación no actualiza la comprensión futura, el equipo puede estar ignorando lo que el sistema le ha enseñado.
