# Nexus artifacts

## Propósito

Este documento introduce el concepto de **Nexus artifacts** dentro de VSlices Docs Standard.

Su objetivo es definir una forma liviana de componer artifacts existentes alrededor de un elemento compuesto sin crear documentos monolíticos prematuramente.

Un Nexus ayuda cuando un elemento aparece repetidamente a través de varias preguntas documentales, pero no tiene una única pregunta principal suficiente para justificar un nuevo tipo de documento.

## Problema que resuelven

Algunos elementos relevantes no viven naturalmente en un solo documento.

Por ejemplo, una capacidad puede requerir explicar:

* qué cubre
* qué debe ocurrir
* cómo se organiza
* qué reglas respeta
* si es viable
* qué decisiones la delimitan
* qué validaciones o riesgos la acompañan

Crear un documento único para todo eso puede duplicar responsabilidades que ya pertenecen a otros artifacts.

Un Nexus permite declarar la composición sin absorber el contenido.

## Qué es un Nexus

Un **Nexus** es un artifact liviano que agrupa artifacts relacionados para explicar un elemento compuesto.

No reemplaza los documentos que compone.

Su responsabilidad principal es declarar:

* qué elemento compuesto se está explicando
* qué artifacts participan
* qué rol cumple cada artifact
* qué lectura sugerida ayuda a entender el conjunto

Definición compacta:

> Un Nexus compone artifacts existentes alrededor de un elemento compuesto sin duplicar su contenido.

## Qué no es un Nexus

Un Nexus no debería confundirse con:

* un documento detallado del elemento
* una plantilla que mezcla varios documentos en uno
* un Continuity Path
* un Navigation Document
* una matriz de trazabilidad obligatoria
* una carpeta
* una taxonomía exhaustiva
* una excusa para formalizar todo

El Nexus declara composición.

Los documentos explican el contenido.

## Regla semántica base

VSlices Docs Standard separa responsabilidades:

* Los **documentos** explican.
* Los **continuity paths** conectan.
* Los **diagramas** muestran.
* Los **mockups** representan.
* La **organización documental** ordena.
* Los **nexus** componen.

Regla compacta:

> Los Nexus componen artifacts alrededor de un elemento compuesto.

## Diferencia con artifacts cercanos

| Artifact            | Responsabilidad                                             |
| ------------------- | ----------------------------------------------------------- |
| Documento           | Explica una pregunta principal                              |
| Continuity Path     | Conecta un concepto a través de perspectivas de continuidad |
| Navigation Document | Orienta una lectura humana de una colección o recorrido     |
| Artifact Index      | Presenta una familia de artifacts y sus reglas              |
| Nexus               | Declara qué artifacts explican juntos un elemento compuesto |

## Cuándo considerar un Nexus

Conviene considerar un Nexus cuando:

* un elemento aparece repetidamente en distintos paths
* el elemento requiere varios documentos para entenderse
* crear un documento único duplicaría responsabilidades
* la composición aporta claridad real
* existe riesgo de perder continuidad entre artifacts relacionados
* la lectura del conjunto necesita orientación mínima

Regla práctica:

> Si un elemento aparece repetidamente como composición de varias preguntas documentales, considerar un Nexus antes de crear un nuevo Document.

## Cuándo no usar un Nexus

No conviene usar un Nexus cuando:

* un solo documento responde suficientemente la pregunta
* la relación entre artifacts es obvia
* el elemento solo fue mencionado una vez
* no existe pérdida real de continuidad
* la composición todavía es especulativa
* el Nexus solo agrega una capa de navegación sin valor propio

Regla anti-ceremonia:

> Un Nexus debe existir para reducir fragmentación, no para decorar la documentación.

## Modelo base

Un Nexus distingue entre:

* **Elemento compuesto**: concepto, capacidad, feature, contrato, flujo o cambio que requiere varios artifacts para explicarse.
* **Artifact compuesto**: documento, nota, mockup, path o referencia que aporta una parte de la explicación.
* **Rol**: responsabilidad que cumple un artifact dentro de la composición.
* **Lectura sugerida**: orden recomendado para entender el conjunto.
* **Composición**: relación declarada entre el elemento compuesto y sus artifacts.

## Nexus oficial inicial

El primer Nexus oficial candidato es:

* `capability`

Su propósito es explicar capacidades sin crear un `Capability Document` monolítico.

## Capability Nexus

Un `Capability Nexus` agrupa los artifacts que explican una capacidad.

Pregunta principal:

> ¿Qué artifacts explican juntos esta capacidad?

Composición típica:

| Artifact             | Rol                                                             |
| -------------------- | --------------------------------------------------------------- |
| Scope Document       | Define qué cubre la capacidad                                   |
| Behavior Document    | Explica qué debe ocurrir                                        |
| Structure Document   | Explica cómo se organiza                                        |
| Consistency Document | Explica qué reglas debe respetar                                |
| Viability Document   | Evalúa si puede sostenerse                                      |
| Decision Record      | Preserva decisiones relevantes                                  |
| Support Note         | Captura apoyo temporal, evidencia, validación, testing o riesgo |

## Front matter mínimo candidato

```yaml
---
artifact: nexus
kind: capability
status: candidate
target: product-registration
scope: capability
language: es
composes:
  - artifact: scope.product-registration
    role: boundary
  - artifact: behavior.product-registration
    role: expected-behavior
  - artifact: structure.product-registration
    role: organization
  - artifact: consistency.product-registration
    role: rules
  - artifact: viability.product-registration
    role: feasibility
  - artifact: decision.product-registration-boundaries
    role: decision
---
```

## Cuerpo mínimo candidato

```markdown
# Capability Nexus - <capability>

## Propósito

Este Nexus agrupa los artifacts que explican la capacidad `<capability>`.

## Artifacts compuestos

| Artifact | Rol |
|---|---|
| Scope Document | Define qué cubre la capacidad |
| Behavior Document | Explica qué debe ocurrir |
| Structure Document | Explica cómo se organiza |
| Consistency Document | Explica qué reglas debe respetar |
| Viability Document | Evalúa si puede sostenerse |
| Decision Record | Preserva decisiones relevantes |
| Support Note | Captura apoyo temporal o evidencia auxiliar |

## Lectura sugerida

1. Scope
2. Behavior
3. Consistency
4. Structure
5. Viability
6. Decisions
7. Support Notes
```

## Nexos candidatos futuros

Estos nexos pueden observarse, pero no deberían implementarse todavía como parte del MVP.

| Nexus              | Qué podría componer                                           |
| ------------------ | ------------------------------------------------------------- |
| `feature`          | Behavior, Scope, Testing Spec, Result, Validation, Decision   |
| `service-contract` | Structure, Behavior, Consistency, Domain Vocabulary, Decision |
| `product-flow`     | Mockup Flow, Behavior, Feedback, Scope, Decision              |
| `change`           | Update, Decision, Scope, Feedback, Validation, Impact         |
| `handoff`          | Context, Navigation, Ownership, Support Notes, Decisions      |
| `domain-concept`   | Domain Vocabulary, Context, Consistency, Behavior, Decision   |

## Relación con Capability Document

VSlices Docs Standard no introduce un `Capability Document` por ahora.

La capacidad aparece como elemento compuesto.

Su explicación puede emerger desde artifacts existentes.

Regla:

> Capability Nexus coordina la explicación de una capacidad.
> No reemplaza Scope, Behavior, Structure, Consistency, Viability ni Decision Record.

## Relación con metadata y cuerpo

La composición pertenece principalmente a metadata porque conecta artifacts. De igual manera se agregará en el front-matter para facilitar la relación entre VSlices Tooling y Surreal Atlas locales

El cuerpo del Nexus debe explicar solo lo mínimo necesario para orientar la lectura.

Regla práctica:

* Si declara relación entre artifacts, va en `composes`.
* Si explica el rol de lectura, puede ir en el cuerpo.
* Si explica conocimiento de dominio, pertenece al documento correspondiente.
* Si orienta un recorrido humano amplio, puede requerir Navigation Document.
* Si conecta perspectivas de continuidad, puede requerir Continuity Path.

## Señales de sobreingeniería

Una propuesta de Nexus probablemente agrega complejidad prematura si:

* exige crear todos los artifacts compuestos
* duplica contenido de los documentos relacionados
* convierte cada concepto compuesto en Nexus obligatorio
* reemplaza un documento simple que ya era suficiente
* intenta resolver trazabilidad completa
* obliga a mantener una composición perfecta desde el inicio
* crea más nexos que documentos útiles

## Regla de cierre

Un Nexus existe para preservar continuidad entre artifacts que ya necesitan convivir.

No existe para crear una nueva capa obligatoria de documentación.

Toda propuesta de Nexus debe preguntarse:

* ¿Este elemento realmente requiere varios artifacts?
* ¿La composición reduce fragmentación?
* ¿Evita crear un documento monolítico?
* ¿Ayuda a humanos o tooling a entender el conjunto?
* ¿Podemos partir con una versión más pequeña?

Si un solo documento preserva suficiente intención, preferimos ese documento.

Si varios documentos son necesarios pero quedan fragmentados, preferimos un Nexus mínimo.
