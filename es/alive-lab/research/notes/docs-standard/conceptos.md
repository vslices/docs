# Repaso base de VSlices Docs Standard

## Propósito

Este documento resume los conceptos principales de VSlices Docs Standard.

No introduce nuevas categorías, estados, relaciones ni tipos de artifacts.

Las definiciones formales deben mantenerse en:

* el modelo conceptual
* los índices de cada familia de artifacts
* las especificaciones de front-matter
* los artifacts específicos correspondientes

## Familias principales de artifacts

VSlices Docs Standard distingue inicialmente cuatro familias formalizadas.

| Familia         | Responsabilidad principal                                        |
| --------------- | ---------------------------------------------------------------- |
| Document        | Explica conocimiento desde una pregunta documental principal     |
| Support Note    | Apoya, registra o referencia conocimiento auxiliar               |
| Nexus           | Compone artifacts alrededor de un elemento compuesto             |
| Continuity Path | Conecta y orienta continuidad entre artifacts, conceptos o paths |

Regla base:

> Los Documents explican.
> Las Support Notes apoyan, registran o referencian.
> Los Nexus componen.
> Los Continuity Paths conectan y orientan continuidad.

Los diagramas muestran.

Los mockups representan.

La organización documental ordena.

## Document artifacts

Cada Document artifact responde una pregunta documental principal.

| Documento            | Pregunta principal              | Definición                                                                                                      |
| -------------------- | ------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Navigation Document  | ¿Cómo exploramos?               | Explica cómo recorrer un conjunto de artifacts, conceptos, paths, diagramas o mockups sin duplicar su contenido |
| Domain Vocabulary    | ¿Cómo hablamos?                 | Preserva términos, significados, ambigüedades y diferencias de lenguaje dentro de un contexto                   |
| Context Document     | ¿Dónde existe?                  | Explica la situación o contexto donde existe el elemento documentado                                            |
| Structure Document   | ¿Cómo se organiza?              | Explica sus partes, relaciones y forma de organización                                                          |
| Behavior Document    | ¿Qué debe ocurrir?              | Explica el comportamiento esperado desde dominio, producto, sistema o servicio                                  |
| Consistency Document | ¿Qué debe respetar?             | Preserva reglas, invariantes y condiciones que deben mantenerse                                                 |
| Scope Document       | ¿Hasta dónde llega?             | Explica límites, inclusiones, exclusiones y postergaciones                                                      |
| Viability Document   | ¿Es viable?                     | Evalúa si algo puede sostenerse bajo condiciones actuales                                                       |
| Update Document      | ¿Qué se actualizará?            | Explica qué debe cambiar, por qué y cuándo debe aplicarse                                                       |
| Feedback Document    | ¿Qué recibimos al aplicar algo? | Registra una respuesta externa producida por uso, revisión, validación o aplicación                             |
| Decision Record      | ¿Qué se decidió?                | Preserva una decisión, su contexto, razón y consecuencias                                                       |

El tipo documental define la pregunta principal.

`artifact.scope` identifica la clase, naturaleza o escala del elemento declarado en `artifact.target`.

No representa la profundidad del documento ni el límite de su contenido.

## Support Note artifacts

Una Support Note captura conocimiento auxiliar sin obligar a crear prematuramente un Document artifact.

No es un Document liviano.

Es una familia propia de artifacts.

| Tipo           | Pregunta                                            | Uso                                                                             |
| -------------- | --------------------------------------------------- | ------------------------------------------------------------------------------- |
| `draft`        | ¿Qué estamos esbozando?                             | Ideas, hipótesis, fragmentos o conocimiento incompleto                          |
| `result`       | ¿Qué obtuvimos?                                     | Resultado observado al aplicar, probar, usar o revisar algo                     |
| `validation`   | ¿Qué significa lo obtenido frente a un criterio?    | Interpretación de un resultado frente a una expectativa o criterio              |
| `testing-spec` | ¿Cómo probaremos este comportamiento?               | Escenarios o criterios de prueba, normalmente cercanos a BDD                    |
| `risk`         | ¿Qué podría salir mal?                              | Riesgos asociados al artifact o elemento soportado                              |
| `external`     | ¿Dónde vive el artifact externo y cómo debe usarse? | Referencia a especificaciones, contratos, repositorios u otras fuentes externas |

Regla:

> Una Support Note puede contener conocimiento incompleto.
> Si crece hasta responder una pregunta documental principal, debería promoverse a Document artifact.

## Result, Validation y Feedback

Estos conceptos separan ocurrencia, interpretación y respuesta externa.

| Concepto   | Fórmula                                             | Artifact recomendado            |
| ---------- | --------------------------------------------------- | ------------------------------- |
| Result     | objeto aplicado + resultado observado               | `Support Note type: result`     |
| Validation | resultado + criterio                                | `Support Note type: validation` |
| Feedback   | respuesta externa al objeto, resultado o validación | `Feedback Document`             |

> Result registra lo ocurrido.
> Validation interpreta lo ocurrido frente a un criterio.
> Feedback registra la respuesta externa recibida.

## Nexus artifacts

Un Nexus compone artifacts que explican juntos un elemento compuesto.

No reemplaza los artifacts compuestos ni duplica su contenido.

Nexus candidatos iniciales:

| Nexus                     | Pregunta principal                                            |
| ------------------------- | ------------------------------------------------------------- |
| Capability Nexus          | ¿Qué artifacts explican juntos esta capacidad?                |
| Service Consumption Nexus | ¿Qué artifacts explican juntos cómo se consume este servicio? |

Un Nexus debe usarse cuando la composición reduce fragmentación real.

Si un solo documento preserva suficiente intención, no necesitamos un Nexus.

## Continuity Paths

Un Continuity Path conecta un objetivo a través de perspectivas, artifacts o paths relevantes.

No es una explicación completa ni una lista obligatoria de documentos.

El path conecta y orienta continuidad.

El diagrama muestra el recorrido.

Los artifacts conectados preservan el detalle.

## Core Continuity Paths

Los Core Continuity Paths representan perspectivas principales de continuidad.

| Path                | Perspectiva            |
| ------------------- | ---------------------- |
| Business Scenario   | Escenario de negocio   |
| Business Driver     | Motivación de negocio  |
| Domain Context      | Contexto de dominio    |
| Viability           | Viabilidad             |
| Evolution           | Evolución              |
| Software Initiative | Iniciativa de software |
| Client Product      | Producto al cliente    |
| Consumable Service  | Servicio consumible    |

## Supporting Continuity Paths

Los Supporting Continuity Paths representan preocupaciones transversales.

| Path             | Perspectiva          |
| ---------------- | -------------------- |
| Software Project | Proyecto de software |
| Ownership        | Responsabilidad      |
| Impact           | Impacto              |
| Traceability     | Trazabilidad         |

No reemplazan los Core Continuity Paths.

Los complementan cuando la pregunta cambia hacia materialización técnica, responsabilidad, impacto o trazabilidad.

## Contextual Continuity Paths

Los Contextual Continuity Paths aparecen frente a una situación específica.

No representan necesariamente una perspectiva universal que deba recorrerse siempre.

Primer candidato contextual:

| Path              | Pregunta                                                                     |
| ----------------- | ---------------------------------------------------------------------------- |
| Knowledge Handoff | ¿Qué conocimiento debe quedar disponible para que el equipo pueda continuar? |

## Viability kinds

Viability Document utiliza `document.viability.kind` para indicar la dimensión evaluada.

| Kind             | Pregunta orientadora                                                |
| ---------------- | ------------------------------------------------------------------- |
| `economic`       | ¿El costo, inversión o esfuerzo se justifica por el valor esperado? |
| `technical`      | ¿Es viable con las capacidades técnicas actuales?                   |
| `operational`    | ¿Puede sostenerse en la operación real?                             |
| `temporal`       | ¿Cabe en el tiempo o capacidad disponible?                          |
| `organizational` | ¿Existen personas, roles y coordinación para sostenerlo?            |
| `adoption`       | ¿Puede ser adoptado por los actores involucrados?                   |

> Viability Document responde si algo es viable.
> El kind define desde qué dimensión se evalúa.

## Fuente de verdad, organización y proyección

Estos conceptos tienen responsabilidades distintas.

| Concepto                    | Pregunta                                 | Responsabilidad                                    |
| --------------------------- | ---------------------------------------- | -------------------------------------------------- |
| Fuente de verdad documental | ¿Dónde vive el contenido canónico?       | Mantener el contenido vigente                      |
| Organización documental     | ¿Según qué criterio ordenamos artifacts? | Definir pertenencia, secuencia, estado o narrativa |
| Proyección navegable        | ¿Cómo mostramos esa organización?        | Representar el orden mediante referencias          |
| Navigation Document         | ¿Cómo exploramos esta organización?      | Explicar el recorrido recomendado                  |

Una organización documental no obliga a mover ni duplicar artifacts.

Una proyección navegable puede materializarse mediante:

* TreeView
* índices
* tablas
* referencias
* metadata procesada por tooling
* Navigation Documents

## Organizaciones documentales posibles

Una colección puede organizarse por:

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

Estas estrategias no constituyen una arquitectura obligatoria de carpetas.

Deben elegirse según la continuidad que necesitemos preservar.

## Regla de crecimiento documental

Los artifacts no evolucionan mediante niveles obligatorios.

Cada tipo tiene un mapa amplio de preguntas posibles y un punto de partida recomendado.

Tooling podrá representar:

* segmentos recomendados como sólidos
* preguntas todavía no incorporadas como translúcidas
* segmentos adicionales como sólidos cuando el caso los necesite

El artifact concreto materializa únicamente las preguntas necesarias.

No necesita completar todo el mapa.

## Regla de cierre

VSlices Docs Standard preserva:

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

No intenta reemplazar:

* implementación
* testing automático
* operación
* monitoreo
* auditoría formal
* contratos ejecutables
* VSlices Tooling

Cuando una solución más pequeña preserva suficiente intención, preferimos la solución más pequeña.
