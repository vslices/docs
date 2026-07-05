# Repaso base: documentos, continuity paths y organización documental

## 1. Documentos de VSlices Docs Standard

Los documentos sirven para detallar conocimiento.

Cada documento responde una pregunta principal. Esa pregunta ayuda a decidir cuándo usarlo y cuándo no.

| Documento            | Pregunta principal              | Definición                                                                                                                                                                                           |
| -------------------- | ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Navigation Document  | ¿Cómo exploramos?               | Explica cómo recorrer un conjunto de artifacts, conceptos, documentos, caminos de continuidad, diagramas o mockups. Su objetivo es dar contexto de navegación, no repetir todo el contenido.         |
| Domain Vocabulary    | ¿Cómo hablamos?                 | Define el lenguaje usado dentro de un dominio, contexto, proyecto o línea de trabajo. Preserva términos, significados, sinónimos, ambigüedades, palabras en desuso y diferencias entre vocabularios. |
| Context Document     | ¿Dónde existe?                  | Explica el contexto donde existe un concepto, problema, sistema, proyecto, capacidad, decisión o situación observada. Evita documentar soluciones sin explicar el escenario que las origina.         |
| Structure Document   | ¿Cómo se organiza?              | Explica cómo se organiza un concepto y cómo se relacionan sus partes. Puede describir estructuras de dominio, módulos, componentes, bounded contexts, clasificaciones o arquitectura lógica.         |
| Behavior Document    | ¿Qué debe ocurrir?              | Explica qué comportamiento se espera desde la perspectiva del dominio, producto, sistema o servicio. No responde primero cómo se programa, sino qué debe pasar y por qué.                            |
| Consistency Document | ¿Qué debe respetar?             | Documenta reglas, invariantes o condiciones que deben mantenerse verdaderas dentro del dominio o sistema. Su foco es preservar consistencia conceptual o comportamental.                             |
| Scope Document       | ¿Hasta dónde llega?             | Explica los límites de un concepto, iniciativa, capacidad, proyecto, iteración o cambio. Ayuda a separar lo actual de lo futuro y evita expansión accidental de alcance.                             |
| Viability Document   | ¿Es viable?                     | Evalúa si un concepto, iniciativa, cambio, feature, capability, servicio, producto, experimento, decisión o artifact puede sostenerse bajo condiciones actuales según un kind de viabilidad.         |
| Update Document      | ¿Qué se actualizará?            | Explica qué cambiará, por qué cambiará y qué impacto tiene sobre documentos, conceptos, estructuras, comportamientos o decisiones existentes.                                                        |
| Feedback Document    | ¿Qué recibimos al aplicar algo? | Registra una respuesta externa recibida después de aplicar, mostrar, validar o usar algo. Puede venir de usuarios, stakeholders, equipo, revisión externa o uso real.                                |
| Decision Record      | ¿Qué se decidió?                | Registra una decisión relevante, su contexto, razón y consecuencias. Evita que decisiones importantes queden escondidas en conversaciones, commits o memoria informal.                               |
| Support Note         | ¿Qué se necesita?               | Registra información auxiliar, necesidades, bloqueos, dudas, evidencia liviana, resultados, validaciones, pruebas o borradores. Es extensible mediante `kind`.                                       |

## 2. Kinds iniciales de Support Note

`Support Note` funciona como documento liviano para conocimiento auxiliar que no justifica todavía un documento propio.

| Kind         | Pregunta                                         | Definición                                                                                                                             |
| ------------ | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| draft        | ¿Qué estamos esbozando?                          | Registra una idea, hipótesis, fragmento o conocimiento incompleto que todavía no está listo para convertirse en documento estable.     |
| result       | ¿Qué obtuvimos?                                  | Registra un resultado observado al aplicar, probar, usar o revisar algo. No interpreta necesariamente si fue bueno, malo o suficiente. |
| validation   | ¿Qué significa lo obtenido frente a un criterio? | Interpreta un resultado contra una expectativa, criterio, comportamiento esperado, regla, alcance o hipótesis.                         |
| testing-spec | ¿Cómo probaremos este comportamiento?            | Traduce criterios de comportamiento hacia escenarios de prueba, normalmente de forma liviana y cercana a BDD.                          |

## 3. Relación entre Result, Validation y Feedback

| Concepto   | Fórmula                                             | Artifact recomendado            |
| ---------- | --------------------------------------------------- | ------------------------------- |
| Result     | objeto aplicado + resultado observado               | `Support Note kind: result`     |
| Validation | resultado + criterio                                | `Support Note kind: validation` |
| Feedback   | respuesta externa al objeto, resultado o validación | `Feedback Document`             |

Regla simple:

> Result registra lo ocurrido.
> Validation interpreta lo ocurrido frente a un criterio.
> Feedback registra la respuesta externa recibida.

## 4. Continuity Paths

Los Continuity Paths sirven para navegar conocimiento cuando un concepto impacta varios artifacts, perspectivas o superficies del sistema.

Un Continuity Path no es, por sí solo, un documento detallado.

Dentro de esta versión, lo entendemos como un camino de navegación del conocimiento donde el diagrama suele ser protagonista y el texto alrededor orienta cómo recorrerlo.

El Continuity Path muestra el recorrido.

El texto del path explica cómo leerlo, cuándo usarlo, cuándo cambiar de perspectiva y qué riesgos evitar.

## 5. Core Continuity Paths

Los Core Continuity Paths observan un concepto desde perspectivas principales de continuidad del negocio, dominio, viabilidad, evolución, software, producto o servicio.

| Continuity Path     | Perspectiva de continuidad | Pregunta central                                                                      | Definición                                                                                                                                                                 |
| ------------------- | -------------------------- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Business Scenario   | Escenario de negocio       | ¿Dónde estoy trabajando?                                                              | Observa un concepto desde el contexto operativo donde ocurre el trabajo: escenarios, líneas de trabajo, procesos, flujos, actores, responsabilidades y reglas operativas.  |
| Business Driver     | Motivación de negocio      | ¿Por qué importa intervenir?                                                          | Observa un concepto desde la necesidad, dolor, oportunidad, restricción, consecuencia, decisión o iniciativa que justifica intervenir.                                     |
| Domain Context      | Contexto de dominio        | ¿Qué lenguaje, reglas y límites pertenecen a esta parte del negocio?                  | Observa una parte del negocio desde sus límites semánticos: lenguaje, reglas, invariantes, comportamientos, responsabilidades y significados propios.                      |
| Viability           | Viabilidad                 | ¿Es viable abordar esto bajo las condiciones actuales?                                | Observa un concepto, iniciativa, cambio o decisión desde las condiciones, restricciones, riesgos y kinds de viabilidad que determinan si puede sostenerse.                 |
| Evolution           | Evolución                  | ¿Cómo cambia este elemento en el tiempo sin perder su intención?                      | Observa cómo un elemento cambia por alcance, feedback, validación, restricciones o decisiones, preservando qué intención sigue viva.                                       |
| Software Initiative | Iniciativa de software     | ¿Qué herramientas de software tengo o necesito para abordar esta parte del trabajo?   | Observa un esfuerzo organizado de software desde la cobertura funcional que intenta abordar, las piezas que usa, las capacidades que requiere y los proyectos que origina. |
| Client Product      | Producto al cliente        | ¿Qué puede hacer el usuario con este sistema y qué aprendimos sobre esa experiencia?  | Observa un producto desde acciones visibles, usuarios, procesos, flujos, servicios coordinados, decisiones de experiencia, feedback y validación.                          |
| Consumable Service  | Servicio consumible        | ¿Qué puede consumir otro sistema o producto, y qué garantías debe recibir al hacerlo? | Observa un servicio desde capacidad ofrecida, contrato, consumidores, entradas, salidas, errores esperados, comportamiento y garantías.                                    |

## 6. Supporting Continuity Paths

Los Supporting Continuity Paths observan conceptos desde preocupaciones transversales.

No reemplazan a los Core Continuity Paths. Los complementan.

| Continuity Path  | Perspectiva de continuidad | Pregunta central                                          | Definición                                                                                                                                                         |
| ---------------- | -------------------------- | --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Software Project | Proyecto de software       | ¿Cómo vive este concepto dentro del proyecto de software? | Observa un concepto desde su materialización técnica: estructura del proyecto, implementación, decisiones técnicas, dependencias, adapters y evolución del código. |
| Ownership        | Responsabilidad            | ¿Quién lo entiende, decide, valida, mantiene u opera?     | Observa un concepto desde las personas, roles, equipos o áreas que sostienen conocimiento, decisión, validación, operación o mantenimiento.                        |
| Impact           | Impacto                    | ¿Qué otros elementos se ven afectados?                    | Observa un concepto desde los efectos que puede provocar sobre dominio, producto, servicio, proyecto, decisiones, documentación o validación.                      |
| Traceability     | Trazabilidad               | ¿De dónde viene y dónde terminó materializándose?         | Observa un concepto desde su origen, transformaciones, decisiones, artifacts asociados y materialización final.                                                    |

## 7. Viability kinds

`Viability Document` evalúa viabilidad mediante un `kind`.

El kind define qué dimensión de viabilidad se está observando.

| Kind           | Pregunta orientadora                                                   |
| -------------- | ---------------------------------------------------------------------- |
| economic       | ¿El costo, inversión o esfuerzo se justifica por el valor esperado?    |
| technical      | ¿Esto es viable con las capacidades técnicas actuales?                 |
| operational    | ¿Esto puede sostenerse en la operación real?                           |
| temporal       | ¿Esto cabe en el tiempo, calendario o capacidad disponible?            |
| organizational | ¿Tenemos personas, roles, coordinación o ownership para hacerlo?       |
| adoption       | ¿Esto puede ser adoptado por usuarios, equipos o actores involucrados? |

Regla simple:

> Viability Document responde si algo es viable.
> El kind define desde qué dimensión se evalúa esa viabilidad.

## 8. Organización documental

La organización documental sirve para ordenar artifacts según pertenencia, secuencia, estado, etapa, colección o narrativa mayor.

No explica el conocimiento en detalle.

Explica dónde vive, a qué pertenece, qué historia mayor ayuda a contar y cómo debería recorrerse dentro de una colección documental.

Regla simple:

> Los documentos explican.
> Los paths conectan.
> Los diagramas muestran.
> Los mockups representan.
> La organización documental ordena.

## 9. Organizaciones documentales iniciales

| Organización documental       | Escenario que cubre                                                                                 | Qué permite ordenar                                                                   |
| ----------------------------- | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| Por producto                  | Cuando la documentación pertenece a un producto de la suite o sistema                               | `docs-standard`, `framework`, `method`, `design`, `tooling`                           |
| Por proyecto                  | Cuando necesitamos entender el estado y evolución de un proyecto completo                           | contexto, alcance, viabilidad, decisiones, soporte, navegación y estado actual        |
| Por iteración                 | Cuando queremos preservar lo ocurrido durante una iteración de trabajo                              | understanding, planning, building, validating, feedback, updates                      |
| Por etapa                     | Cuando una iteración necesita separar artifacts por momento del proceso                             | descubrimiento, contextualización, planificación, construcción, validación            |
| Por concepto                  | Cuando un concepto acumula vocabulario, contexto, estructura, decisiones, cambios y feedback        | historia y evolución documental de un concepto                                        |
| Por dominio o bounded context | Cuando el conocimiento pertenece a una zona del dominio                                             | vocabulario, reglas, comportamientos, estructura y límites del contexto               |
| Por capability o feature      | Cuando queremos agrupar comportamiento, alcance, estructura y decisiones asociadas a una capacidad  | documentos de una funcionalidad o capacidad concreta                                  |
| Por servicio consumible       | Cuando existe una API, servicio, integración, contrato o capacidad consumida por terceros           | comportamiento, estructura, contrato conceptual, errores, evolución                   |
| Por superficie de producto    | Cuando queremos organizar pantallas, vistas, mockups y comportamiento visible                       | experiencia visible, navegación, representación, feedback y decisiones de producto    |
| Por milestone o release       | Cuando queremos ordenar entregas, versiones, objetivos o incrementos                                | scope, viability, updates, decisions, feedback y artifacts relacionados a una entrega |
| Por caso de investigación     | Cuando queremos preservar evidencia y aprendizaje de un caso real o realista                        | contexto, observaciones, resultados, validaciones, feedback y decisiones              |
| Por experimento o validación  | Cuando queremos registrar una aplicación controlada o una prueba de una idea                        | contexto, criterio, resultado, validación, feedback y viabilidad                      |
| Por estado documental         | Cuando necesitamos separar artifacts activos, candidatos, reemplazados, archivados o experimentales | vigencia, madurez y confiabilidad documental                                          |
| Por versiones anteriores      | Cuando un artifact o concepto evoluciona y queremos preservar historia                              | documentos antiguos, razones del cambio y updates relacionados                        |
| Por colección navegable       | Cuando varios artifacts deben explorarse juntos aunque no pertenezcan a la misma carpeta conceptual | navegación transversal mediante Navigation Document y Continuity Paths                |

## 10. Escenarios cubiertos por organización documental

| Escenario                                 | Organización recomendada                        | Apoyos                                                                                                                  |
| ----------------------------------------- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Cómo va una iteración de desarrollo       | Por iteración + por etapa                       | `Navigation Document`, `Scope Document`, `Viability Document`, `Update Document`, `Feedback Document`, support notes    |
| Cómo va un proyecto en este momento       | Por proyecto + estado documental                | `Navigation Document`, metadata, `Context Document`, `Viability Document`, `Support Note`                               |
| Cómo evoluciona un concepto               | Por concepto + versiones anteriores             | `Update Document`, `Decision Record`, `Feedback Document`, `Evolution Continuity Path`, support notes                   |
| Cómo se organiza un dominio               | Por dominio o bounded context                   | `Domain Vocabulary`, `Context Document`, `Structure Document`, `Consistency Document`, `Domain Context Continuity Path` |
| Cómo se evalúa si algo puede abordarse    | Por proyecto, iteración, concepto o experimento | `Viability Document`, `Scope Document`, `Decision Record`, `Support Note kind: validation`                              |
| Cómo se entrega una capability            | Por capability o feature                        | `Scope Document`, `Viability Document`, `Behavior Document`, `Structure Document`, `Decision Record`                    |
| Cómo se expone un servicio                | Por servicio consumible                         | `Consumable Service Continuity Path`, `Behavior Document`, `Structure Document`, diagramas                              |
| Cómo se representa una vista de producto  | Por superficie de producto                      | mockups, `Behavior Document`, `Feedback Document`, `Client Product Continuity Path`                                     |
| Cómo se documenta una release             | Por milestone o release                         | roadmap, diagrama, `Scope Document`, `Viability Document`, `Update Document`, `Decision Record`                         |
| Cómo se preserva aprendizaje aplicado     | Por caso de investigación o experimento         | `Context Document`, `Support Note kind: result`, `Support Note kind: validation`, `Feedback Document`                   |
| Cómo se mantiene historia documental      | Por versiones anteriores + estado documental    | metadata, `Update Document`, `Decision Record`, `Traceability Continuity Path`                                          |
| Cómo se exploran relaciones transversales | Por colección navegable                         | `Navigation Document`, Continuity Paths, diagramas, metadata                                                            |

## 11. Features iniciales candidatas

A partir de esta taxonomía, las features iniciales más sanas para VSlices Docs Standard / Tooling podrían ser:

| Feature inicial                     | Qué habilita                                                                               | Por qué es MVP-friendly                                                |
| ----------------------------------- | ------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| Catálogo de documentos              | Definir documentos, preguntas principales y usos esperados                                 | Es base conceptual y no requiere automatización compleja               |
| Catálogo de Continuity Paths        | Definir paths core/support y sus perspectivas                                              | Permite navegación del conocimiento sin crear muchos documentos nuevos |
| Navigation Document básico          | Explicar cómo explorar una colección documental                                            | Une paths, documentos, diagramas y organización                        |
| Support Note con `kind` extensible  | Registrar draft, result, validation y testing-spec sin crear documentos nuevos             | Evita sobreingeniería documental                                       |
| Viability Document con `kind`       | Evaluar viabilidad económica, técnica, operacional, temporal, organizacional o de adopción | Cubre decisiones de alcance sin crear un documento por dimensión       |
| Organización documental recomendada | Proponer estructuras de carpetas por proyecto, iteración, concepto, dominio, feature, etc. | Ayuda a ordenar sin imponer una arquitectura documental única          |
| Metadata mínima de estado           | Distinguir draft, candidate, active, superseded, archived, etc.                            | Apoya validez documental sin depender solo de carpetas                 |
| Referencias mínimas entre artifacts | Conectar documentos, paths, notas, diagramas y mockups                                     | Es la base de trazabilidad futura                                      |
| Diagramas como artifacts asociados  | Permitir visualización de conocimiento sin mezclarlo todo en texto                         | Mantiene documentos más simples                                        |
| Mockups como artifacts asociados    | Representar vistas o experiencia visible sin crear View Document prematuramente            | Cubre producto/UX sin inflar la taxonomía                              |

## 12. Regla de cierre

VSlices Docs Standard no intenta ejecutar, validar automáticamente, auditar formalmente ni operar sistemas.

Su responsabilidad es preservar:

* intención
* contexto
* lenguaje
* estructura
* comportamiento
* decisiones
* alcance
* viabilidad
* evolución
* evidencia documental
* navegación del conocimiento

Cuando algo requiere ejecución, automatización, validación técnica, monitoreo, contratos formales o grafos vivos, Docs Standard puede definir la intención y la relación documental, pero la responsabilidad pasa a implementación, testing, operación o VSlices Tooling.
