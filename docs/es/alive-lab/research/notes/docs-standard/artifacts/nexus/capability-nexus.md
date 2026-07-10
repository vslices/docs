# Nexus artifact "Capability" de <tema>

## Propósito del nexus

<!--
¿Para qué necesitamos este nexus?

Explicar qué continuidad se busca preservar alrededor de una capacidad sin crear un Capability Document monolítico.
-->

Este nexus busca preservar continuidad alrededor de una capacidad que necesita ser entendida desde varios artifacts relacionados.

Ayuda a responder:

> ¿Qué artifacts explican juntos esta capacidad?

Una capacidad puede requerir claridad sobre alcance, comportamiento, estructura, reglas, viabilidad, decisiones, validaciones, testing, riesgos o evidencia auxiliar.

Este nexus no intenta explicar todo el contenido de la capacidad.

Intenta componer los artifacts que, juntos, permiten entenderla sin duplicar responsabilidades documentales.

Es especialmente útil cuando una capacidad aparece en varios continuity paths, como contexto de dominio, iniciativa de software, servicio consumible, producto al cliente, viabilidad o proyecto de software.

## Punto de entrada

<!--
¿Por dónde empieza este nexus?

Indicar la capacidad, feature, operación, servicio, comportamiento o elemento compuesto que necesita ser explicado mediante varios artifacts.
-->

## Diagrama de composición

<!--
¿Qué composición vamos a recorrer?

Incluir el Diagrama de Nexus asociado a Capability.
El diagrama debe mostrar artifacts relacionados y el rol que cumplen dentro de la composición.
-->

```mermaid
flowchart LR
    A[["<b>Capability Nexus</b><br/>[Capacidad compuesta]<br/><small>Capability Nexus</small>"]]

    A --> P1["¿Qué cubre esta capacidad?"]
    A --> P2["¿Qué debe ocurrir?"]
    A --> P3["¿Cómo se organiza?"]
    A --> P4["¿Qué reglas debe respetar?"]
    A -.-> P5["¿Es viable sostenerla?"]
    A -.-> P6["¿Qué decisiones la delimitan?"]
    A -.-> P7["¿Qué soporte auxiliar existe?"]

    P1 --> S1[["<b>Scope</b><br/>[Límite de la capacidad]<br/><small>Scope Document</small>"]]
    P1 --> S2>"<b>Scope</b><br/>[Alcance identificado]"]

    P2 --> B1[["<b>Behavior</b><br/>[Comportamiento esperado]<br/><small>Behavior Document</small>"]]
    P2 --> B2>{{"<b>Behavior</b><br/>[Comportamiento que requiere documentación]<br/><small>Behavior Document<br/>Support Note kind: testing-spec</small>"}}

    P3 --> ST1[["<b>Structure</b><br/>[Organización de la capacidad]<br/><small>Structure Document</small>"]]
    P3 --> ST2>"<b>Structure</b><br/>[Estructura identificada]"]

    P4 --> C1[["<b>Consistency</b><br/>[Reglas o invariantes]<br/><small>Consistency Document</small>"]]
    P4 --> C2>{{"<b>Consistency</b><br/>[Regla que requiere documentación]<br/><small>Consistency Document<br/>Behavior Document</small>"}}

    P5 -.-> V1[["<b>Viability</b><br/>[Viabilidad evaluada]<br/><small>Viability Document</small>"]]
    P5 -.-> V2>{{"<b>Viability</b><br/>[Viabilidad pendiente]<br/><small>Viability Document<br/>Support Note kind: validation</small>"}}

    P6 -.-> D1[["<b>Decision</b><br/>[Decisión documentada]<br/><small>Decision Record</small>"]]
    P6 -.-> D2>{{"<b>Decision</b><br/>[Decisión pendiente]<br/><small>Decision Record<br/>Support Note kind: draft</small>"}}

    P7 -.-> N1[["<b>Support Note</b><br/>[Nota de soporte]<br/><small>Support Note kind: draft<br/>Support Note kind: result<br/>Support Note kind: validation<br/>Support Note kind: testing-spec<br/>Support Note kind: risk</small>"]]
    P7 -.-> F1[["<b>Feedback</b><br/>[Feedback relacionado]<br/><small>Feedback Document</small>"]]
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender la capacidad sin duplicar el contenido de los artifacts compuestos.
-->

| Orden | Nodo, artifact o concepto | Por qué revisarlo                                                                  |
| ----- | ------------------------- | ---------------------------------------------------------------------------------- |
| 1     | Capacidad compuesta       | Permite identificar qué capacidad estamos intentando entender                      |
| 2     | Alcance                   | Permite saber qué cubre, excluye o posterga la capacidad                           |
| 3     | Comportamiento esperado   | Permite entender qué debe ocurrir cuando la capacidad se usa o ejecuta             |
| 4     | Reglas o invariantes      | Permite reconocer qué condiciones no deben romperse                                |
| 5     | Estructura                | Permite entender qué partes, relaciones o responsabilidades sostienen la capacidad |
| 6     | Viabilidad                | Permite evaluar si la capacidad puede sostenerse bajo condiciones reales           |
| 7     | Decisiones                | Permite entender por qué la capacidad tiene esos límites, reglas o forma           |
| 8     | Notas de soporte          | Permite revisar conocimiento auxiliar, validaciones, testing, resultados o riesgos |
| 9     | Feedback                  | Permite entender si el uso real corrigió o confirmó la capacidad                   |

## Capability, documentos y composición

<!--
¿Cómo se distingue Capability Nexus de Capability Document?

Usar esta sección para evitar que el nexus se convierta en un documento monolítico.
-->

| Concepto             | Cómo se interpreta                                                            | Cuándo usarlo                                                                            |
| -------------------- | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Capability           | Capacidad que permite realizar, sostener o coordinar comportamiento relevante | Cuando una iniciativa, servicio, producto o contexto necesita una capacidad para operar  |
| Capability Nexus     | Composición de artifacts que explican una capacidad                           | Cuando la capacidad requiere varias perspectivas documentales                            |
| Scope Document       | Límite de la capacidad                                                        | Cuando necesitamos definir qué entra, sale o queda pendiente                             |
| Behavior Document    | Comportamiento esperado de la capacidad                                       | Cuando necesitamos explicar qué debe ocurrir                                             |
| Structure Document   | Organización de la capacidad                                                  | Cuando necesitamos explicar partes, relaciones o responsabilidades                       |
| Consistency Document | Reglas, invariantes o garantías                                               | Cuando la capacidad debe respetar condiciones fuertes                                    |
| Viability Document   | Evaluación de viabilidad                                                      | Cuando necesitamos saber si la capacidad puede sostenerse                                |
| Decision Record      | Decisiones que delimitan la capacidad                                         | Cuando necesitamos preservar por qué se eligió una forma, alcance o regla                |
| Support Note         | Apoyo liviano                                                                 | Cuando existe conocimiento auxiliar, incompleto, validación, testing, resultado o riesgo |
| Feedback Document    | Respuesta externa o aprendizaje                                               | Cuando el uso real confirma, corrige o cambia la capacidad                               |

## Roles de composición

<!--
¿Qué rol cumple cada artifact dentro del nexus?

Usar esta sección para orientar metadata, tooling o lectura humana.
-->

| Role              | Artifact habitual               | Qué preserva                                       |
| ----------------- | ------------------------------- | -------------------------------------------------- |
| boundary          | Scope Document                  | Límites, inclusiones, exclusiones y postergaciones |
| expected-behavior | Behavior Document               | Comportamiento esperado                            |
| organization      | Structure Document              | Organización, partes y responsabilidades           |
| rules             | Consistency Document            | Reglas, invariantes y garantías                    |
| feasibility       | Viability Document              | Condiciones reales de viabilidad                   |
| decision          | Decision Record                 | Decisiones que delimitan o justifican la capacidad |
| support           | Support Note                    | Apoyo auxiliar o temporal                          |
| validation        | Support Note kind: validation   | Interpretación frente a criterio                   |
| testing           | Support Note kind: testing-spec | Escenarios o criterios de prueba                   |
| risk              | Support Note kind: risk         | Riesgos asociados                                  |
| learning          | Feedback Document               | Aprendizaje desde uso o respuesta externa          |

## Front matter mínimo sugerido

<!--
La composición vive principalmente en metadata porque conecta artifacts.
No duplicar en el cuerpo contenido que pertenece a los documentos compuestos.
-->

```yaml
---
artifact: nexus
kind: capability
status: candidate
target: <capability-name>
scope: capability
language: es
composes:
  - artifact: <scope-document-id>
    role: boundary
  - artifact: <behavior-document-id>
    role: expected-behavior
  - artifact: <structure-document-id>
    role: organization
  - artifact: <consistency-document-id>
    role: rules
  - artifact: <viability-document-id>
    role: feasibility
  - artifact: <decision-record-id>
    role: decision
  - artifact: <support-note-id>
    role: support
---
```

## Reglas de uso

<!--
¿Qué reglas evitan que el nexus agregue ceremonia innecesaria?
-->

* Un Capability Nexus compone artifacts.
* Un Capability Nexus no reemplaza los documentos compuestos.
* Un Capability Nexus no duplica contenido.
* Un Capability Nexus puede partir incompleto.
* Un Capability Nexus no obliga a crear todos los artifacts listados.
* Si un solo documento basta, no crear Nexus.
* Si varios documentos explican una capacidad y quedan dispersos, usar Nexus.
* Si la composición no reduce fragmentación, no usar Nexus.

## Señales de sobreingeniería

<!--
¿Cuándo este nexus está resolviendo un problema futuro en vez de uno actual?
-->

Un Capability Nexus probablemente agrega complejidad prematura si:

* existe solo porque la palabra capability apareció una vez
* obliga a crear Scope, Behavior, Structure, Consistency y Viability desde el inicio
* repite el contenido de los documentos relacionados
* intenta convertirse en Capability Document
* reemplaza una navegación simple que ya era suficiente
* exige mantener una composición perfecta antes de tener evidencia real

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender esta capacidad sin pertenecer necesariamente a la composición principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con la capacidad | Path, artifact o nexus sugerido |
| ----------------------- | ------------------------- | ------------------------------- |
| <concepto>              | <relación>                | <path, artifact o nexus>        |
