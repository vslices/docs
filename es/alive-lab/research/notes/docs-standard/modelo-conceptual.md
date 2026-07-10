# Modelo conceptual base de VSlices Docs Standard

## Propósito

VSlices Docs Standard define una forma de preservar conocimiento relevante durante el ciclo de vida de un sistema.

Su objetivo no es producir documentación por ceremonia, sino mantener continuidad entre:

* intención
* contexto
* lenguaje
* estructura
* comportamiento
* decisiones
* alcance
* viabilidad
* evolución
* evidencia
* composición
* navegación del conocimiento

Docs Standard no reemplaza implementación, testing, operación ni tooling.

Su responsabilidad es ofrecer estructuras documentales que permitan explicar, apoyar, componer, conectar y organizar conocimiento sin perder intención.

## Conceptos generales

| Concepto              | Definición                                                                                                             |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Concepto              | Unidad de significado que puede ser explicada, apoyada, compuesta, conectada, mostrada, representada u organizada      |
| Estructura documental | Forma propuesta para preservar conocimiento mediante una responsabilidad explícita                                     |
| Artifact              | Materialización concreta de una estructura documental que puede preservarse, referenciarse, organizarse y relacionarse |
| Target                | Elemento concreto sobre el que aplica un artifact                                                                      |
| Scope                 | Clase, naturaleza o escala del target                                                                                  |
| Metadata              | Información estructurada que describe estado y relaciones generales de un artifact                                     |
| Referencia            | Relación explícita entre artifacts o elementos relevantes                                                              |

## Familias formalizadas de artifacts

VSlices Docs Standard distingue inicialmente cuatro familias.

| Familia         | Responsabilidad principal                                        |
| --------------- | ---------------------------------------------------------------- |
| Document        | Explica conocimiento desde una pregunta documental principal     |
| Support Note    | Apoya, registra o referencia conocimiento auxiliar               |
| Nexus           | Compone artifacts alrededor de un elemento compuesto             |
| Continuity Path | Conecta y orienta continuidad entre artifacts, conceptos o paths |

Regla semántica:

> Los Documents explican.
> Las Support Notes apoyan, registran o referencian.
> Los Nexus componen.
> Los Continuity Paths conectan y orientan continuidad.

Estas responsabilidades no son intercambiables.

Un artifact debería mantener una responsabilidad principal clara.

## Modelo de Document

Un Document explica conocimiento desde una pregunta documental principal.

Cuando se materializa, declara:

| Elemento  | Propósito                                                 |
| --------- | --------------------------------------------------------- |
| Type      | Tipo documental definido por la pregunta principal        |
| Scope     | Clase, naturaleza o escala del target                     |
| Target    | Elemento concreto que se explica                          |
| Question  | Pregunta documental principal                             |
| Status    | Estado del artifact dentro de su ciclo de vida documental |
| Relations | Relaciones generales con otros artifacts                  |
| Content   | Explicación preservada                                    |

Definición compacta:

> Un Document explica un target desde una pregunta documental principal.

El límite del contenido no debe confundirse con `artifact.scope`.

`artifact.scope` clasifica el target.

Los límites, inclusiones o exclusiones pertenecen al contenido o a un Scope Document.

## Tipos de Document

Un tipo documental no existe principalmente por su formato.

Existe porque responde una pregunta distinta.

| Tipo              | Pregunta principal              |
| ----------------- | ------------------------------- |
| Navigation        | ¿Cómo exploramos?               |
| Domain Vocabulary | ¿Cómo hablamos?                 |
| Context           | ¿Dónde existe?                  |
| Structure         | ¿Cómo se organiza?              |
| Behavior          | ¿Qué debe ocurrir?              |
| Consistency       | ¿Qué debe respetar?             |
| Scope             | ¿Hasta dónde llega?             |
| Viability         | ¿Es viable?                     |
| Update            | ¿Qué se actualizará?            |
| Feedback          | ¿Qué recibimos al aplicar algo? |
| Decision Record   | ¿Qué se decidió?                |

> Si dos tipos responden la misma pregunta principal, probablemente pertenecen al mismo tipo o necesitan diferenciar mejor su intención.

Cada Document declara `document.question`.

Cuando necesita metadata específica del tipo, la declara bajo una subcategoría propia dentro de `document`.

## Modelo de Support Note

Una Support Note captura conocimiento auxiliar sin obligar a crear prematuramente un Document.

Es una familia propia de artifacts.

No es un tipo de Document.

Puede registrar:

* borradores
* resultados
* validaciones
* especificaciones de prueba
* riesgos
* referencias externas
* conocimiento incompleto

Tipos iniciales:

| Tipo           | Pregunta                                            |
| -------------- | --------------------------------------------------- |
| `draft`        | ¿Qué estamos esbozando?                             |
| `result`       | ¿Qué obtuvimos?                                     |
| `validation`   | ¿Qué significa lo obtenido frente a un criterio?    |
| `testing-spec` | ¿Cómo probaremos este comportamiento?               |
| `risk`         | ¿Qué podría salir mal?                              |
| `external`     | ¿Dónde vive el artifact externo y cómo debe usarse? |

> Si una Support Note crece hasta responder una pregunta documental principal, debería promoverse a Document.

## Resultado, Validación y Feedback

Estos conceptos separan ocurrencia, interpretación y respuesta externa.

| Concepto   | Definición                                   | Artifact recomendado      |
| ---------- | -------------------------------------------- | ------------------------- |
| Resultado  | Registra lo ocurrido                         | Support Note `result`     |
| Validación | Interpreta un resultado frente a un criterio | Support Note `validation` |
| Feedback   | Registra una respuesta externa               | Feedback Document         |

> Resultado no interpreta.
> Validación interpreta.
> Feedback registra una respuesta externa.

## Modelo de Nexus

Un Nexus compone artifacts que explican juntos un elemento compuesto.

Su responsabilidad es declarar:

* qué target compuesto se intenta entender
* qué artifacts participan
* qué rol cumple cada artifact dentro de la composición

Definición compacta:

> Un Nexus compone artifacts alrededor de un target sin duplicar su contenido.

La composición se declara en `composition.composes`.

Las relaciones generales que no forman parte de la composición se declaran en `metadata.relates`.

Nexus candidatos iniciales:

* Capability Nexus
* Service Consumption Nexus

Si un solo Document preserva suficiente intención, no necesitamos un Nexus.

## Modelo de Continuity Path

Un Continuity Path conecta un target a través de perspectivas, artifacts o paths relevantes.

No es una explicación completa ni una lista obligatoria de documentos.

Su responsabilidad es preservar continuidad visible.

Definición compacta:

> Un Continuity Path conecta y orienta continuidad alrededor de un target.

El path declara:

* la pregunta de continuidad
* el foco que intenta preservar
* los artifacts o paths conectados
* el rol que cada conexión cumple

El diagrama muestra el recorrido.

Los artifacts conectados preservan el detalle.

## Categorías de Continuity Paths

Los Continuity Paths se agrupan inicialmente en tres categorías.

| Categoría  | Rol                                                         |
| ---------- | ----------------------------------------------------------- |
| Core       | Perspectivas principales de continuidad                     |
| Supporting | Preocupaciones transversales                                |
| Contextual | Situaciones específicas que requieren preservar continuidad |

Core iniciales:

* Business Scenario
* Business Driver
* Domain Context
* Viability
* Evolution
* Software Initiative
* Client Product
* Consumable Service

Supporting iniciales:

* Software Project
* Ownership
* Impact
* Traceability

Contextual inicial:

* Knowledge Handoff

Estas categorías orientan el uso.

No constituyen una taxonomía cerrada ni obligatoria.

## Representaciones asociadas

Algunas estructuras ayudan a materializar o mostrar conocimiento, aunque todavía no formen parte de las familias formalizadas mediante schema.

| Representación | Responsabilidad                                            |
| -------------- | ---------------------------------------------------------- |
| Diagram        | Muestra relaciones, estructuras, flujos o caminos          |
| Mockup         | Representa una experiencia, vista o superficie de producto |

Un diagrama no reemplaza la explicación preservada en otros artifacts.

Un mockup no reemplaza la definición del comportamiento esperado.

## Fuente de verdad y organización documental

Estos conceptos tienen responsabilidades distintas.

| Concepto                    | Pregunta                                  | Responsabilidad                                    |
| --------------------------- | ----------------------------------------- | -------------------------------------------------- |
| Fuente de verdad documental | ¿Dónde vive el contenido canónico?        | Mantener el contenido vigente                      |
| Organización documental     | ¿Según qué criterio se ordenan artifacts? | Definir pertenencia, secuencia, estado o narrativa |
| Proyección navegable        | ¿Cómo se muestra esa organización?        | Representar el orden mediante referencias          |
| Navigation Document         | ¿Cómo recorremos esa organización?        | Explicar el recorrido recomendado                  |

Una organización documental no define necesariamente la ubicación física de un artifact.

Una proyección navegable no cambia su fuente de verdad.

Un mismo artifact puede aparecer en varias organizaciones sin duplicar su contenido.

## Modelo de relaciones

El modelo puede leerse mediante estas relaciones:

* Un Artifact tiene un kind, type, scope y target.
* Un Document responde una pregunta documental.
* Una Support Note apoya un artifact o elemento principal.
* Un Nexus compone artifacts mediante roles explícitos.
* Un Continuity Path conecta artifacts o paths mediante roles de continuidad.
* Metadata describe estado y relaciones generales.
* Un Diagram puede mostrar un Nexus o Continuity Path.
* Una Organización documental ordena artifacts según un criterio.
* Una Proyección navegable muestra una organización mediante referencias.
* Un Navigation Document explica cómo recorrer una colección o proyección.

Las relaciones especializadas no deberían duplicarse en `metadata.relates`.

## Lectura completa del modelo

VSlices Docs Standard preserva conocimiento mediante artifacts con responsabilidades explícitas.

Un target puede:

* ser explicado por Documents
* recibir apoyo mediante Support Notes
* ser entendido como composición mediante Nexus
* seguirse entre perspectivas mediante Continuity Paths
* mostrarse mediante diagramas
* representarse mediante mockups
* ordenarse mediante organizaciones documentales
* aparecer en proyecciones navegables sin duplicar su fuente de verdad

La metadata ayuda a preservar estado y relaciones sin convertir Docs Standard en un grafo obligatorio.

## Límites del modelo

Docs Standard puede definir:

* intención documental
* familias y tipos de artifacts
* preguntas principales
* relaciones documentales
* composición
* continuidad
* formas de navegación
* organización documental
* evidencia preservable
* reglas para tooling documental

Docs Standard no asume directamente:

* ejecución
* testing automático
* monitoreo
* auditoría formal
* validación técnica completa
* sincronización viva con código
* contratos ejecutables
* grafos dinámicos obligatorios

Cuando estas necesidades aparecen, Docs Standard preserva su intención documental.

La ejecución corresponde a implementación, testing, operación o VSlices Tooling.

## Principio de simplicidad

El modelo debe mantenerse pequeño.

* No todo necesita Document.
* No todo conocimiento auxiliar debe formalizarse.
* No todo elemento compuesto necesita Nexus.
* No todo concepto necesita recorrer todos los Continuity Paths.
* No toda relación necesita un grafo.
* No toda organización necesita una estructura física.
* No toda evidencia necesita validación formal.

Primero preservamos intención y continuidad.

Después, cuando el uso real lo justifique, convertimos patrones repetidos en estructura, reglas o tooling.
