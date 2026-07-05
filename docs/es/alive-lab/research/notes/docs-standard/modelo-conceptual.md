# Modelo conceptual base de VSlices Docs Standard

## 1. Propósito del modelo

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
* navegación del conocimiento

Docs Standard no reemplaza implementación, testing, operación ni tooling.

Su responsabilidad principal es explicar, conectar, ordenar y preservar conocimiento para que el sistema pueda evolucionar sin perder intención.

## 2. Términos

### 2.1. Generales

| Concepto                  | Definición                                                                                                                                                                 |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Concepto                  | Unidad de significado que puede ser explicada, conectada, mostrada, representada, organizada o trazada.                                                                    |
| Estructura de explicación | Forma propuesta por Docs Standard para explicar, conectar, mostrar, representar u ordenar conocimiento.                                                                    |
| Artifact                  | Materialización concreta de una estructura de explicación. Al ser concreto, puede preservarse, referenciarse, organizarse, versionarse o relacionarse con otros artifacts. |

### 2.2. Estructuras de explicación

| Concepto                | Definición                                                                                                  |
| ----------------------- | ----------------------------------------------------------------------------------------------------------- |
| Documento               | Estructura textual que explica conocimiento desde una pregunta documental principal.                        |
| Camino de continuidad   | Estructura que conecta un concepto a través de varias perspectivas de continuidad, artifacts o superficies. |
| Diagrama                | Estructura visual que muestra relaciones, estructuras, flujos o caminos.                                    |
| Mockup                  | Estructura visual que representa una experiencia, vista o superficie de producto.                           |
| Organización documental | Estructura de orden según pertenencia, secuencia, estado, etapa, colección o narrativa mayor.               |

### 2.3. Conceptos de apoyo

| Concepto                | Definición                                                                                                     |
| ----------------------- | -------------------------------------------------------------------------------------------------------------- |
| Tipo de documento       | Categoría documental definida por la pregunta principal que responde un documento.                             |
| Pregunta documental     | Pregunta central que orienta el propósito, alcance y contenido esperado de un documento.                       |
| Metadata                | Información estructurada que describe identidad, estado, relaciones o clasificación de un artifact.            |
| Referencia              | Relación explícita entre artifacts, documentos, conceptos, estructuras o caminos de continuidad.               |
| Nota de soporte         | Documento liviano para conocimiento auxiliar que todavía no justifica un documento más estable o específico.   |
| Documento de navegación | Documento que explica cómo recorrer un conjunto de artifacts, conceptos, estructuras o caminos de continuidad. |

## 3. Reglas semánticas base

| Elemento                | Responsabilidad principal         |
| ----------------------- | --------------------------------- |
| Documento               | Explica                           |
| Camino de continuidad   | Conecta                           |
| Diagrama                | Muestra                           |
| Mockup                  | Representa                        |
| Organización documental | Ordena                            |
| Metadata                | Clasifica y habilita trazabilidad |
| Referencia              | Relaciona explícitamente          |

Regla central:

Los documentos no deberían intentar hacer todo.

* Un documento explica conocimiento desde una pregunta principal.
* Un camino conecta perspectivas.
* Un diagrama muestra una relación.
* Un mockup representa una experiencia.
* Una organización documental ordena artifacts dentro de una narrativa o estructura mayor.

## 4. Modelo de Documento

Un Documento es una estructura textual de explicación.

Cuando se materializa, produce un artifact documental orientado a preservar conocimiento.

Todo Documento debería definir:

| Elemento   | Propósito                                                                   |
| ---------- | --------------------------------------------------------------------------- |
| Tema       | Concepto, situación, capacidad, decisión o cambio que el documento explica. |
| Tipo       | Tipo documental al que pertenece.                                           |
| Pregunta   | Pregunta principal que responde.                                            |
| Alcance    | Límite de lo que el documento intenta cubrir.                               |
| Estado     | Estado documental del artifact materializado.                               |
| Relaciones | Referencias hacia otros artifacts relevantes.                               |
| Contenido  | Explicación preservada.                                                     |

Definición compacta:

> Un Documento explica un Tema desde una Pregunta documental dentro de un Alcance determinado.

Ejemplo:

> Un Documento de Contexto explica dónde existe un concepto, problema, sistema, proyecto, capacidad, decisión o situación observada.

## 5. Modelo de Tipo de Documento

Un Tipo de Documento no existe principalmente por formato.

Existe porque responde una pregunta documental distinta.

| Tipo de Documento           | Pregunta principal              |
| --------------------------- | ------------------------------- |
| Documento de Navegación     | ¿Cómo exploramos?               |
| Vocabulario de Dominio      | ¿Cómo hablamos?                 |
| Documento de Contexto       | ¿Dónde existe?                  |
| Documento de Estructura     | ¿Cómo se organiza?              |
| Documento de Comportamiento | ¿Qué debe ocurrir?              |
| Documento de Consistencia   | ¿Qué debe respetar?             |
| Documento de Alcance        | ¿Hasta dónde llega?             |
| Documento de Viabilidad     | ¿Es viable?                     |
| Documento de Actualización  | ¿Qué se actualizará?            |
| Documento de Feedback       | ¿Qué recibimos al aplicar algo? |
| Registro de Decisión        | ¿Qué se decidió?                |
| Nota de Soporte             | ¿Qué se necesita?               |

Regla:

> Si dos documentos responden la misma pregunta principal, probablemente pertenecen al mismo tipo o necesitan diferenciar mejor su intención.

## 6. Modelo de Nota de Soporte

Nota de Soporte es un Documento liviano.

Su propósito es capturar conocimiento auxiliar sin forzar la creación prematura de un documento más formal.

Una Nota de Soporte puede registrar:

* dudas
* bloqueos
* borradores
* evidencia liviana
* resultados
* validaciones
* necesidades
* hipótesis incompletas
* especificaciones livianas de prueba

Nota de Soporte se especializa mediante `kind`.

Kinds iniciales:

| Kind         | Pregunta                                         | Uso                                                                                             |
| ------------ | ------------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| draft        | ¿Qué estamos esbozando?                          | Ideas, hipótesis o conocimiento incompleto.                                                     |
| result       | ¿Qué obtuvimos?                                  | Resultado observado al aplicar, probar, usar o revisar algo.                                    |
| validation   | ¿Qué significa lo obtenido frente a un criterio? | Interpretación de un resultado contra una expectativa o criterio.                               |
| testing-spec | ¿Cómo probaremos este comportamiento?            | Traducción liviana, normalmente BDD, de criterios de comportamiento hacia escenarios de prueba. |

Regla:

> Nota de Soporte existe para evitar sobreingeniería documental temprana.

## 7. Modelo de Documento de Viabilidad

Documento de Viabilidad es un Documento que evalúa si algo puede abordarse bajo condiciones actuales.

Su pregunta principal es:

> ¿Es viable?

El Documento de Viabilidad no define una única dimensión universal.

Se especializa mediante `kind`.

Kinds iniciales de viabilidad:

| Kind           | Pregunta orientadora                                                   |
| -------------- | ---------------------------------------------------------------------- |
| economic       | ¿El costo, inversión o esfuerzo se justifica por el valor esperado?    |
| technical      | ¿Esto es viable con las capacidades técnicas actuales?                 |
| operational    | ¿Esto puede sostenerse en la operación real?                           |
| temporal       | ¿Esto cabe en el tiempo, calendario o capacidad disponible?            |
| organizational | ¿Tenemos personas, roles, coordinación u ownership para hacerlo?       |
| adoption       | ¿Esto puede ser adoptado por usuarios, equipos o actores involucrados? |

Regla:

> El Documento de Viabilidad responde si algo es viable.
> El kind define desde qué dimensión se evalúa esa viabilidad.

## 8. Patrón Resultado / Validación / Feedback

Estos tres conceptos separan ocurrencia, interpretación y respuesta externa.

| Concepto   | Definición                                  | Artifact recomendado             |
| ---------- | ------------------------------------------- | -------------------------------- |
| Resultado  | Registra lo ocurrido                        | Nota de Soporte kind: result     |
| Validación | Interpreta lo ocurrido frente a un criterio | Nota de Soporte kind: validation |
| Feedback   | Registra una respuesta externa recibida     | Documento de Feedback            |

Fórmulas:

| Concepto   | Fórmula                                             |
| ---------- | --------------------------------------------------- |
| Resultado  | objeto aplicado + resultado observado               |
| Validación | resultado + criterio                                |
| Feedback   | respuesta externa al objeto, resultado o validación |

Regla:

> Resultado no interpreta.
> Validación interpreta.
> Feedback registra respuesta externa.

## 9. Modelo de Camino de Continuidad

Un Camino de Continuidad conecta conocimiento.

No es, por sí solo, un documento detallado.

Su propósito es permitir seguir un concepto cuando impacta varias perspectivas, artifacts o superficies del sistema.

Un Camino de Continuidad puede estar:

* representado por un diagrama
* explicado mediante texto de navegación
* apoyado por metadata y referencias
* conectado con documentos específicos

Definición compacta:

> Un Camino de Continuidad conecta un Concepto a través de una o más perspectivas de continuidad.

Regla:

> El Camino de Continuidad define el recorrido.
> El diagrama suele mostrar el camino.
> El texto de navegación explica cómo recorrerlo sin reemplazar los artifacts conectados.

## 10. Tipos de Caminos de Continuidad

Los Caminos de Continuidad se dividen inicialmente en dos grupos:

| Grupo       | Rol                                                                                                                                            |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Principales | Observan un concepto desde perspectivas principales de continuidad del negocio, dominio, viabilidad, evolución, software, producto o servicio. |
| Soporte     | Observan un concepto desde preocupaciones transversales.                                                                                       |

Los Caminos de Continuidad principales son estos:

| Camino              | Perspectiva            | Pregunta                                                                              |
| ------------------- | ---------------------- | ------------------------------------------------------------------------------------- |
| Business Scenario   | Escenario de negocio   | ¿Dónde estoy trabajando?                                                              |
| Business Driver     | Motivación de negocio  | ¿Por qué importa intervenir?                                                          |
| Domain Context      | Contexto de dominio    | ¿Qué lenguaje, reglas y límites pertenecen a esta parte del negocio?                  |
| Viability           | Viabilidad             | ¿Es viable abordar esto bajo las condiciones actuales?                                |
| Evolution           | Evolución              | ¿Cómo cambia este elemento en el tiempo sin perder su intención?                      |
| Software Initiative | Iniciativa de software | ¿Qué herramientas de software tengo o necesito para abordar esta parte del trabajo?   |
| Client Product      | Producto al cliente    | ¿Qué puede hacer el usuario con este sistema y qué aprendimos sobre esa experiencia?  |
| Consumable Service  | Servicio consumible    | ¿Qué puede consumir otro sistema o producto, y qué garantías debe recibir al hacerlo? |

Los Caminos de Continuidad de soporte son estos:

| Camino           | Perspectiva          | Pregunta                                                  |
| ---------------- | -------------------- | --------------------------------------------------------- |
| Software Project | Proyecto de software | ¿Cómo vive este concepto dentro del proyecto de software? |
| Ownership        | Responsabilidad      | ¿Quién lo entiende, decide, valida, mantiene u opera?     |
| Impact           | Impacto              | ¿Qué otros elementos se ven afectados?                    |
| Traceability     | Trazabilidad         | ¿De dónde viene y dónde terminó materializándose?         |

Regla:

> Los Caminos de Continuidad de soporte no reemplazan a los principales. Los complementan.

## 11. Modelo de Documento de Navegación

Un Documento de Navegación explica cómo recorrer conocimiento.

Puede explicar cómo explorar:

* una colección documental
* un camino de continuidad
* un conjunto de artifacts
* un concepto complejo
* una iteración
* un proyecto
* una release
* un caso de investigación

No debería repetir todo el contenido de los artifacts que conecta.

Definición compacta:

> Un Documento de Navegación explica cómo recorrer un conjunto de artifacts o caminos sin reemplazar el contenido de ellos.

Regla:

> Documento de Navegación orienta; no duplica.

## 12. Modelo de Organización Documental

Organización Documental define dónde viven los artifacts y cómo deberían recorrerse dentro de una estructura mayor.

No explica el conocimiento en detalle.

Puede ordenar artifacts por:

* producto
* proyecto
* iteración
* etapa
* concepto
* dominio o bounded context
* capability o feature
* servicio consumible
* superficie de producto
* milestone o release
* caso de investigación
* experimento o validación
* estado documental
* versiones anteriores
* colección navegable

Definición compacta:

> Organización Documental ordena artifacts según pertenencia, secuencia, estado, etapa, colección o narrativa mayor.

Regla:

> La organización documental no reemplaza la explicación documental.

## 13. Modelo de relaciones

El modelo conceptual puede leerse como estas relaciones:

* Un Concepto es explicado por uno o varios Documentos.
* Un Documento tiene un Tipo de Documento.
* Un Tipo de Documento responde a una Pregunta Documental.
* Una Nota de Soporte es una forma liviana de Documento.
* Una Nota de Soporte tiene un kind.
* Un Documento de Viabilidad tiene un kind de viabilidad.
* Un Resultado puede ser interpretado por un criterio, formando una Validación.
* Un Feedback responde a un Resultado o Validación.
* Un Camino de Continuidad conecta Conceptos.
* Un Documento de Navegación explica recorridos documentales.
* Un Diagrama puede mostrar visualmente un Camino de Continuidad.
* Una Organización documental agrupa Artifacts según un criterio.
* La metadata describe los Artifacts, su identidad, estado o relaciones.
* Las Referencias conectan Artifacts.

## 14. Lectura completa del modelo

La lectura completa sería:

* VSlices Docs Standard preserva conocimiento mediante estructuras de explicación materializadas como artifacts.
* Un concepto puede ser explicado, conectado, mostrado, representado, organizado o trazado.
* Cada documento explica un concepto desde una pregunta documental.
* Los tipos de documento existen porque responden preguntas distintas.
* Las notas de soporte permiten capturar conocimiento auxiliar sin inflar la taxonomía.
* El Documento de Viabilidad permite evaluar si algo puede abordarse bajo condiciones actuales.
* Los resultados registran ocurrencias.
* Las validaciones interpretan resultados contra criterios.
* Los documentos de feedback preservan respuestas externas.
* Los caminos de continuidad conectan conceptos entre perspectivas.
* Los documentos de navegación explican cómo recorrer caminos de continuidad o colecciones.
* Los diagramas muestran relaciones.
* Los mockups representan superficies visibles.
* La organización documental ordena artifacts dentro de una estructura o narrativa mayor.
* La metadata y las referencias habilitan trazabilidad futura sin exigir automatización temprana.

## 15. Límites del modelo

Docs Standard puede definir:

* intención documental
* tipos de documentos
* preguntas principales
* relaciones entre artifacts
* formas de navegación
* organización documental
* evidencia preservable
* viabilidad documentalmente evaluable
* reglas de trazabilidad documental

Docs Standard no debería intentar asumir directamente:

* ejecución
* testing automático
* monitoreo
* auditoría formal
* validación técnica completa
* sincronización viva con código
* contratos ejecutables
* grafos dinámicos obligatorios

Cuando esas necesidades aparecen, Docs Standard puede definir la intención y la estructura documental, pero la responsabilidad pasa a implementación, testing, operación o VSlices Tooling.

## 16. Principio de simplicidad

El modelo debe mantenerse pequeño.

* No todo necesita documento propio.
* No todo path necesita automatización.
* No toda relación necesita grafo.
* No toda evidencia necesita validación formal.
* No toda viabilidad necesita evaluación completa.
* No todo cambio necesita camino de evolución.

Primero preservamos intención y continuidad.

Después, cuando el uso real lo justifique, convertimos patrones repetidos en estructura, reglas o tooling.
