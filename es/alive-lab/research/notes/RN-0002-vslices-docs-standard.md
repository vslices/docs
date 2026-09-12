---
type: research-note
state: candidate
code: RN-0002
related_questions:
* RQ-001

related_notes:
* RN-0001

related_synthesis:
* SYN-0001

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
* Surreal Atlas
---

# RN-0002 — VSlices Docs Standard como superficie de continuidad documental

## Tipo

research-note

## Estado

candidate

## Propósito

Esta nota registra una hipótesis conceptual candidata para VSlices Research:

> VSlices Docs Standard puede entenderse como la superficie de VSlices encargada de preservar continuidad documental entre intención, contexto, lenguaje, estructura, comportamiento, decisiones, alcance, viabilidad, evolución, evidencia, composición y navegación del conocimiento.

La nota no valida todavía que Docs Standard funcione.

Tampoco convierte sus conceptos en parte adoptada de VSlices Research.

Su propósito es ordenar los mecanismos candidatos principales de Docs Standard para alimentar preguntas de investigación más pequeñas, observables y validables.

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

La pregunta fundacional estudia qué problema práctico dio origen a VSlices y cómo ese problema puede transformarse en una línea de investigación aplicada sobre continuidad de conocimiento sin perder su raíz práctica.

Esta nota explora cómo ese problema fundacional aparece específicamente en la superficie documental de VSlices.

## Notas relacionadas

[RN-0001 — Superficies de continuidad en VSlices](RN-0001-superficies-continuidad-vslices.md)

`RN-0001` propone que VSlices puede observarse como una suite compuesta por distintas superficies de continuidad:

* VSlices Design
* VSlices Docs Standard
* VSlices Method
* VSlices Framework

Esta nota toma la superficie de Docs Standard y la desarrolla con mayor detalle para preparar preguntas de investigación específicas.

## Síntesis relacionada

[SYN-0001 — Escenarios iniciales de ruptura o escape de continuidad de conocimiento](../synthesis/syn-0001-escenarios-iniciales-ruptura-escape-continuidad-conocimiento.md)

`SYN-0001` propone, en estado `candidate`, que la continuidad de conocimiento puede verse comprometida en al menos cuatro escenarios iniciales:

* pérdida histórica
* dispersión activa
* concentración personal
* escape inicial

Docs Standard podría aportar mecanismos para observar, preservar o reconstruir continuidad en algunos de estos escenarios, pero esa relación todavía debe validarse mediante casos concretos.

## Idea central

VSlices Docs Standard no debería investigarse inicialmente como un bloque monolítico.

En lugar de preguntar:

> ¿Funciona VSlices Docs Standard?

conviene investigar mecanismos candidatos más pequeños:

| Mecanismo candidato         | Pregunta general                                                                             |
| --------------------------- | -------------------------------------------------------------------------------------------- |
| Document artifacts          | ¿Cómo explicamos conocimiento desde preguntas documentales principales?                      |
| Support Notes               | ¿Cómo preservamos conocimiento auxiliar sin formalizarlo prematuramente?                     |
| Nexus artifacts             | ¿Cómo componemos artifacts relacionados alrededor de elementos compuestos?                   |
| Continuity Paths            | ¿Cómo conectamos perspectives, artifacts, decisiones y conceptos para preservar continuidad? |
| Organizaciones documentales | ¿Cómo ordenamos y proyectamos artifacts sin duplicar su fuente de verdad?                    |

Esta nota propone que estos mecanismos forman una superficie documental orientada a continuidad.

Su valor no está en producir más documentación, sino en reducir pérdida, dispersión, concentración o escape de conocimiento mediante artifacts con responsabilidades explícitas.

## Mecanismo candidato 1: Document artifacts

Los Document artifacts son artifacts que explican conocimiento desde una pregunta documental principal.

Su identidad no depende principalmente del formato, sino de la pregunta que intentan responder.

Ejemplos iniciales:

| Document artifact    | Pregunta principal              |
| -------------------- | ------------------------------- |
| Navigation Document  | ¿Cómo exploramos?               |
| Domain Vocabulary    | ¿Cómo hablamos?                 |
| Context Document     | ¿Dónde existe?                  |
| Structure Document   | ¿Cómo se organiza?              |
| Behavior Document    | ¿Qué debe ocurrir?              |
| Consistency Document | ¿Qué debe respetar?             |
| Scope Document       | ¿Hasta dónde llega?             |
| Viability Document   | ¿Es viable?                     |
| Update Document      | ¿Qué se actualizará?            |
| Feedback Document    | ¿Qué recibimos al aplicar algo? |
| Decision Record      | ¿Qué se decidió?                |

La hipótesis candidata es que una pregunta documental principal ayuda a evitar documentos ambiguos, plantillas rígidas o artifacts que mezclan demasiadas responsabilidades.

### Posible aporte a continuidad

Los Document artifacts podrían preservar continuidad al mantener visible:

* qué se intenta explicar
* sobre qué target aplica la explicación
* qué pregunta principal organiza el contenido
* qué intención documental debe mantenerse
* qué conocimiento pertenece al cuerpo y qué pertenece a metadata
* qué aspectos deben mantenerse separados de otros artifacts

### Riesgo

Los Document artifacts podrían introducir ceremonia si cada pregunta derivada se convierte en sección obligatoria o si el mapa completo de preguntas se interpreta como plantilla final.

### Pregunta de investigación candidata

¿En qué condiciones los Document artifacts definidos por preguntas principales ayudan a preservar conocimiento sin imponer plantillas rígidas ni documentación excesiva?

## Mecanismo candidato 2: Support Notes

Las Support Notes capturan conocimiento auxiliar sin obligar a crear prematuramente un Document artifact.

No son Documents livianos.

Son una familia propia para preservar conocimiento que todavía puede estar incompleto, ser auxiliar o requerir observación adicional.

Tipos candidatos iniciales:

| Support Note | Pregunta                                            |
| ------------ | --------------------------------------------------- |
| draft        | ¿Qué estamos esbozando?                             |
| result       | ¿Qué obtuvimos?                                     |
| validation   | ¿Qué significa lo obtenido frente a un criterio?    |
| testing-spec | ¿Cómo probaremos este comportamiento?               |
| risk         | ¿Qué podría salir mal?                              |
| external     | ¿Dónde vive el artifact externo y cómo debe usarse? |

La hipótesis candidata es que Support Notes permiten preservar conocimiento útil sin promoverlo demasiado temprano a documentación principal.

### Posible aporte a continuidad

Las Support Notes podrían preservar continuidad al registrar:

* ideas incompletas
* resultados observados
* validaciones frente a criterios
* riesgos
* especificaciones de prueba
* referencias externas
* evidencia auxiliar
* conocimiento temporal o de transición

También podrían ayudar a separar ocurrencia, interpretación y respuesta externa:

| Concepto   | Artifact recomendado          |
| ---------- | ----------------------------- |
| Result     | Support Note type: result     |
| Validation | Support Note type: validation |
| Feedback   | Feedback Document             |

### Riesgo

Las Support Notes podrían convertirse en un contenedor genérico para todo lo que no se sabe clasificar.

Si una Support Note crece hasta responder una pregunta documental principal, debería evaluarse si corresponde promoverla a Document artifact.

### Pregunta de investigación candidata

¿En qué condiciones las Support Notes ayudan a preservar conocimiento auxiliar, incompleto o temporal sin promoverlo prematuramente a Document artifact ni convertirse en un contenedor genérico de información no clasificada?

## Mecanismo candidato 3: Nexus artifacts

Los Nexus artifacts componen artifacts alrededor de un elemento compuesto.

No reemplazan los artifacts compuestos.

No duplican su contenido.

Su responsabilidad es declarar qué artifacts explican juntos un elemento y qué rol cumple cada uno dentro de esa composición.

Nexus candidatos iniciales:

| Nexus                     | Pregunta principal                                            |
| ------------------------- | ------------------------------------------------------------- |
| Capability Nexus          | ¿Qué artifacts explican juntos esta capacidad?                |
| Service Consumption Nexus | ¿Qué artifacts explican juntos cómo se consume este servicio? |

La hipótesis candidata es que un Nexus puede reducir fragmentación cuando un elemento relevante necesita varios artifacts para entenderse, pero no justifica crear un documento monolítico.

### Posible aporte a continuidad

Los Nexus podrían preservar continuidad al conectar artifacts relacionados alrededor de:

* una capability
* un servicio consumible
* una composición documental
* una decisión distribuida
* un conjunto de comportamientos
* una relación entre alcance, comportamiento, estructura, reglas y viabilidad

Por ejemplo, una capacidad puede requerir:

* Scope Document
* Behavior Document
* Structure Document
* Consistency Document
* Viability Document
* Decision Record
* Support Notes

Un Capability Nexus puede orientar esa composición sin convertirla en un Capability Document gigante.

### Riesgo

Los Nexus podrían agregar una capa documental innecesaria si se usan cuando un solo documento basta o cuando la composición no reduce fragmentación real.

También podrían volverse una forma indirecta de crear documentación obligatoria para cada capability, servicio o feature.

### Pregunta de investigación candidata

¿En qué condiciones los Nexos Documentales ayudan a preservar continuidad alrededor de elementos compuestos sin duplicar contenido ni crear documentos monolíticos?

## Mecanismo candidato 4: Continuity Paths

Los Continuity Paths conectan y orientan continuidad alrededor de un target.

No son explicación completa.

No son checklist documental.

No reemplazan los artifacts conectados.

Su responsabilidad es ayudar a recorrer un concepto, situación o elemento a través de perspectivas, artifacts, decisiones, relaciones o paths relevantes.

Categorías iniciales:

| Categoría  | Rol                                                         |
| ---------- | ----------------------------------------------------------- |
| Core       | Perspectivas principales de continuidad                     |
| Supporting | Preocupaciones transversales                                |
| Contextual | Situaciones específicas que requieren preservar continuidad |

Core Continuity Paths candidatos:

* Business Scenario
* Business Driver
* Domain Context
* Viability
* Evolution
* Software Initiative
* Client Product
* Consumable Service

Supporting Continuity Paths candidatos:

* Software Project
* Ownership
* Impact
* Traceability

Contextual Continuity Path inicial:

* Knowledge Handoff

La hipótesis candidata es que los Continuity Paths permiten hacer visibles conexiones relevantes entre conocimiento, artifacts y decisiones sin exigir que todo se documente al mismo tiempo.

### Posible aporte a continuidad

Los Continuity Paths podrían preservar continuidad al ayudar a identificar:

* dónde ocurre el trabajo
* qué motivación origina una decisión
* qué lenguaje pertenece a un contexto de dominio
* qué condiciones hacen viable una idea
* cómo cambia algo sin perder intención
* qué iniciativa de software cubre una parte del trabajo
* qué producto materializa una experiencia visible
* qué servicio expone una capacidad consumible
* quién entiende, decide, valida, mantiene u opera algo
* qué se ve afectado si algo cambia
* de dónde viene un concepto y dónde terminó materializándose
* qué conocimiento debe quedar disponible durante un handoff

### Riesgo

Los Continuity Paths podrían convertirse en checklist si se interpretan como una lista obligatoria de documentos o perspectivas que siempre deben recorrerse.

También podrían aumentar la complejidad si cada nodo identificado se convierte automáticamente en artifact.

### Pregunta de investigación candidata

¿En qué condiciones los Caminos de Continuidad ayudan a preservar continuidad de conocimiento entre perspectivas, artifacts, decisiones y conceptos sin convertirse en checklist documental obligatorio?

## Mecanismo candidato 5: Organizaciones documentales

Las organizaciones documentales separan varias responsabilidades que suelen confundirse:

| Concepto                    | Pregunta                                                          |
| --------------------------- | ----------------------------------------------------------------- |
| Fuente de verdad documental | ¿Dónde vive el contenido canónico?                                |
| Organización documental     | ¿Según qué criterio ordenamos artifacts?                          |
| Proyección navegable        | ¿Cómo mostramos esa organización sin mover ni duplicar contenido? |
| Navigation Document         | ¿Cómo exploramos esta organización?                               |

La hipótesis candidata es que separar estas responsabilidades ayuda a preservar continuidad sin imponer una estructura física única de carpetas.

Un artifact puede tener una fuente de verdad y participar en varias organizaciones o proyecciones.

Por ejemplo, un Decision Record podría aparecer en:

* una capability
* una iniciativa de software
* un proyecto
* una release
* un Continuity Path de Evolution
* un Nexus

Esa participación múltiple no debería crear múltiples fuentes de verdad.

### Posible aporte a continuidad

Las organizaciones documentales podrían preservar continuidad al permitir:

* ordenar artifacts según distintos criterios
* mostrar recorridos sin mover archivos
* generar proyecciones navegables
* evitar duplicación de contenido
* mantener una fuente canónica clara
* conectar con tooling o visualizaciones documentales
* habilitar Surreal Atlas como superficie de navegación sin convertirlo en fuente de verdad

### Riesgo

Una proyección navegable podría duplicar contenido canónico y convertirse en una segunda fuente de verdad.

También podría confundirse organización documental con arquitectura obligatoria de carpetas.

### Pregunta de investigación candidata

¿En qué condiciones separar fuente de verdad, organización documental, proyección navegable y navegación ayuda a preservar continuidad sin duplicar contenido ni imponer una estructura física única?

## Relación candidata entre mecanismos

Una lectura inicial del modelo podría ser:

```text
VSlices Docs Standard
  ├─ Document artifacts
  │   └─ explican conocimiento desde preguntas principales
  ├─ Support Notes
  │   └─ apoyan, registran o referencian conocimiento auxiliar
  ├─ Nexus artifacts
  │   └─ componen artifacts alrededor de elementos compuestos
  ├─ Continuity Paths
  │   └─ conectan y orientan continuidad entre perspectivas
  └─ Organizaciones documentales
      └─ ordenan y proyectan artifacts sin duplicar fuente de verdad
```

Esta relación es candidata.

No debe tratarse todavía como arquitectura definitiva de Docs Standard.

## RQs candidatas derivadas

Esta nota alimenta inicialmente cuatro preguntas de investigación.

### RQ-002 — Caminos de Continuidad

¿En qué condiciones los Caminos de Continuidad ayudan a preservar continuidad de conocimiento entre perspectivas, artifacts, decisiones y conceptos sin convertirse en checklist documental obligatorio?

### RQ-003 — Nexos Documentales

¿En qué condiciones los Nexos Documentales ayudan a preservar continuidad alrededor de elementos compuestos sin duplicar contenido ni crear documentos monolíticos?

### RQ-004 — Documentos

¿En qué condiciones los Document artifacts definidos por preguntas principales ayudan a preservar conocimiento sin imponer plantillas rígidas ni documentación excesiva?

### RQ-005 — Organizaciones Documentales

¿En qué condiciones separar fuente de verdad, organización documental, proyección navegable y navegación ayuda a preservar continuidad sin duplicar contenido ni imponer una estructura física única?

### RQ-006 — Notas de Soporte

¿En qué condiciones las Support Notes ayudan a preservar conocimiento auxiliar, incompleto o temporal sin promoverlo prematuramente a Document artifact ni convertirse en un contenedor genérico de información no clasificada?

## Orden recomendado de investigación

Aunque los Caminos de Continuidad son el mecanismo más directamente conectado con el problema fundacional, conviene investigar primero la unidad documental base.

Orden candidato:

1. Document artifacts
2. Continuity Paths
3. Nexus artifacts
4. Organizaciones documentales

La razón es que Continuity Paths, Nexus y organizaciones documentales conectan, componen u ordenan artifacts.

Si todavía no entendemos bien cómo funciona un Document artifact como unidad explicativa, los otros mecanismos pueden quedar flotando.

## Relación con Alive Lab

Esta nota debe validarse mediante casos concretos de Alive Lab.

Los casos no deberían intentar probar Docs Standard completo.

Deberían observar mecanismos pequeños en situaciones reales o realistas.

Cada caso podría preguntarse:

* ¿Qué conocimiento estaba en riesgo?
* ¿Qué mecanismo documental se aplicó?
* ¿Qué continuidad intentaba preservar?
* ¿Qué artifact se creó o evitó crear?
* ¿Qué fragmentación redujo?
* ¿Qué ceremonia introdujo?
* ¿Qué evidencia quedó disponible?
* ¿Qué evidencia sigue faltando?
* ¿Qué mecanismo debería ajustarse?

## Relación con Domus Orbis

Domus Orbis puede servir para observar Docs Standard en un contexto doméstico, ambiguo y progresivamente digitalizado.

Puede aportar evidencia sobre:

* Context Documents
* Domain Vocabulary
* Behavior Documents
* Classification como conocimiento de dominio
* Support Notes para conocimiento incompleto
* Continuity Paths entre escenario doméstico, dominio, producto y evolución
* Organizaciones documentales pequeñas sin tooling pesado

Domus Orbis es especialmente útil para observar si Docs Standard ayuda cuando el conocimiento existe en práctica cotidiana antes de convertirse en software.

## Relación con Surreal Atlas

Surreal Atlas puede servir para observar Docs Standard desde navegación, relaciones, proyecciones y continuidad entre artifacts.

Puede aportar evidencia sobre:

* fuente de verdad documental
* organizaciones documentales
* proyecciones navegables
* Navigation Documents
* Continuity Paths
* Nexus artifacts
* visualización de relaciones documentales
* separación entre contenido canónico y representación navegable

Surreal Atlas no debería validar por sí solo que Docs Standard funciona.

Puede ayudar a observar si los artifacts y relaciones definidos por Docs Standard son navegables, visibles y reutilizables sin duplicar contenido.

## Evidencia inicial disponible

Esta nota se apoya inicialmente en:

* la formulación de `RQ-001`
* la síntesis candidata `SYN-0001`
* la nota `RN-0001`
* el modelo conceptual candidato de VSlices Docs Standard
* los artifacts candidatos de Documents, Support Notes, Nexus, Continuity Paths y organizaciones documentales
* la intención explícita de evitar documentación por ceremonia
* la necesidad de validar mecanismos mediante casos concretos

## Evidencia faltante

Para fortalecer esta nota, todavía falta observar:

* si los Document artifacts ayudan a preservar intención en casos reales
* si las preguntas principales ayudan a elegir el artifact correcto
* si las Support Notes evitan documentación prematura
* si los Nexus reducen fragmentación real
* si los Continuity Paths orientan sin convertirse en checklist
* si las organizaciones documentales permiten múltiples proyecciones sin duplicar contenido
* si los usuarios pueden distinguir Documents, Support Notes, Nexus, Continuity Paths y Navigation Documents
* si estos mecanismos siguen siendo útiles sin tooling
* si tooling mejora la continuidad o introduce complejidad adicional
* si los mecanismos funcionan fuera de los casos iniciales

## Riesgos metodológicos

### Riesgo de validar Docs Standard como bloque único

Docs Standard no debería validarse como una unidad completa en esta etapa.

Las RQs deben estudiar mecanismos candidatos específicos.

### Riesgo de convertir mecanismos en obligación

Un mecanismo útil en un caso no debe transformarse automáticamente en regla universal.

Cada artifact debe existir porque preserva continuidad en un contexto concreto.

### Riesgo de usar los casos para confirmar la teoría

Los casos de estudio deben poder mostrar fallas, límites, sobrecarga o solapamientos.

No deben usarse solo para demostrar que Docs Standard estaba bien diseñado.

### Riesgo de sobreformalizar antes de observar

La existencia de front-matter, diagramas, roles y familias puede dar apariencia de madurez.

Mientras no exista evidencia suficiente, todo debe mantenerse como candidate.

### Riesgo de confundir navegación con continuidad

Una organización navegable puede mejorar exploración sin necesariamente preservar continuidad.

La investigación debe observar cuándo la navegación realmente ayuda a mantener intención, relaciones o trazabilidad significativa.

### Riesgo de acoplar Docs Standard a Tooling demasiado temprano

Tooling puede ayudar a generar, validar o visualizar artifacts.

Pero Docs Standard debe poder explicar su valor documental antes de depender de automatización.

## Lo que esta nota no afirma

Esta nota no afirma que Docs Standard funcione.

No afirma que sus familias estén completas.

No afirma que todos los proyectos necesiten Documents, Support Notes, Nexus, Continuity Paths u organizaciones documentales.

No afirma que los tres casos de estudio futuros validen universalmente el estándar.

No convierte los conceptos de Docs Standard en estado `adopted`.

No demuestra que estos mecanismos preserven continuidad mejor que otras formas de documentación.

Solo propone una estructura candidata para abrir preguntas de investigación más pequeñas.

## Límite actual

Esta nota debe usarse como puente entre el problema fundacional de continuidad y las RQs específicas sobre Docs Standard.

Su valor actual está en ordenar el campo de investigación.

No debe convertirse todavía en principio oficial, taxonomía final ni decisión de producto.

La pregunta central que deja abierta es:

> ¿Qué mecanismos documentales preservan continuidad de conocimiento, bajo qué condiciones, con qué costo y con qué límites?
