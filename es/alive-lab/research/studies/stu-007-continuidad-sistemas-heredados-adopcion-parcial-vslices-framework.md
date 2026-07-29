---
type: study
state: candidate
code: STU-007
visibility: private-redacted
evidence_policy: summarized
study_scope: bounded

related_questions:
- RQ-001
- RQ-002
- RQ-003
- RQ-004
- RQ-005
- RQ-006
- RQ-007
- RQ-008

related_notes:
- RN-0001
- RN-0002
- RN-0003

related_synthesis:
- SYN-0001

related_findings:
- FND-0001
- FND-0002

affects:
- VSlices Docs Standard
- VSlices Framework
- VSlices Tooling
---

# STU-007 — Continuidad entre sistemas heredados y adopción parcial de VSlices Framework

## Estado

candidate

## Visibilidad

private-redacted

## Política de evidencia

Este estudio trabaja con un caso real compuesto por sistemas institucionales desarrollados en distintos momentos de madurez técnica y documental.

Por restricciones de privacidad, confidencialidad y responsabilidad profesional, el estudio no debe publicar documentos internos completos, nombres sensibles, detalles operacionales específicos, datos institucionales, información de usuarios, diagramas completos ni material que permita reconstruir procesos privados del contexto.

La evidencia podrá utilizarse en forma de:

* descripciones generales
* artifacts redactados
* diagramas simplificados
* ejemplos sintéticos derivados
* observaciones metodológicas
* comparación entre estados documentales
* comparación entre enfoques técnicos
* resultados agregados
* feedback general de personas involucradas
* análisis de continuidad sin exponer detalles internos

Los artifacts reales podrán resumirse, anonimizarse o transformarse en ejemplos equivalentes cuando sea necesario.

## Contexto

Este estudio ocurre en un contexto institucional donde existen varios sistemas desarrollados en distintos momentos.

El caso incluye:

* sistemas creados hace años, antes de que VSlices estuviera formalizado
* un sistema más reciente que utiliza una versión más actual o parcial de VSlices Framework
* conocimiento técnico y documental distribuido entre código, experiencia previa, documentación existente y decisiones acumuladas

Esto permite observar una situación especialmente valiosa para VSlices Research:

> ¿Qué diferencias aparecen en la continuidad de conocimiento cuando se comparan sistemas heredados con un sistema más reciente que adopta parcialmente ideas de VSlices Framework?

La comparación no debe entenderse como una demostración de superioridad.

Debe entenderse como un contraste exploratorio entre distintos niveles de madurez técnica, documental y metodológica.

## Situación observada

En sistemas desarrollados antes de VSlices, parte del conocimiento puede existir, pero no necesariamente estar organizado según preguntas documentales, continuity paths, nexus, support notes o mecanismos explícitos de continuidad.

Ese conocimiento puede estar repartido entre:

* código
* estructura de carpetas
* convenciones históricas
* memoria del desarrollador
* documentación parcial
* decisiones no registradas
* comportamiento esperado conocido por uso
* necesidades institucionales
* ajustes realizados durante años

En un sistema más reciente, algunas ideas de VSlices Framework pueden estar presentes en la forma de organizar comportamiento, features, slices, estructura técnica o separación de responsabilidades.

Esto permite observar si una adopción parcial de VSlices cambia la forma en que el conocimiento puede recuperarse, explicarse o mantenerse.

## Problema de continuidad

El problema central es observar cómo cambia la continuidad de conocimiento entre sistemas con distinta historia y madurez.

La continuidad puede verse afectada por:

* sistemas antiguos con conocimiento implícito
* documentación insuficiente o desactualizada
* decisiones técnicas no registradas
* diferencias entre arquitectura real e intención original
* ausencia de trazabilidad entre necesidad, comportamiento e implementación
* adopción parcial de patrones técnicos sin documentación equivalente
* distancia entre Framework, Docs Standard y Method
* dificultad para explicar sistemas heredados usando conceptos actuales

El riesgo es asumir que un sistema más reciente preserva mejor continuidad solo porque usa una versión parcial de VSlices Framework.

Eso debe observarse, no darse por hecho.

## Pregunta local del estudio

¿Qué diferencias aparecen en la continuidad de conocimiento entre sistemas heredados y un sistema con adopción parcial de VSlices Framework, especialmente al analizarlos mediante mecanismos candidatos de VSlices Docs Standard?

## RQs relacionadas

Este estudio puede alimentar varias preguntas de investigación de Docs Standard.

| RQ                                   | Relación con el estudio                                                                         |
| ------------------------------------ | ----------------------------------------------------------------------------------------------- |
| [RQ-002 — Caminos de Continuidad](../questions/rq-002-continuity-paths.md)      | Observa si paths ayudan a reconstruir continuidad en sistemas antiguos y recientes              |
| [RQ-003 — Nexos Documentales](../questions/rq-003-document-nexus.md)          | Puede observar si capabilities, servicios o módulos compuestos requieren composición documental |
| [RQ-004 — Documentos](../questions/rq-004-documents.md)                  | Observa si Documents por pregunta principal ayudan a explicar sistemas con distinta madurez     |
| [RQ-005 — Organizaciones Documentales](../questions/rq-005-documental-organization.md) | Observa cómo organizar artifacts de varios sistemas sin duplicar contenido                      |
| [RQ-006 — Notas de Soporte](../questions/rq-006-support-notes.md)            | Observa si notas auxiliares ayudan a capturar incertidumbre, riesgos o validaciones parciales   |
| [RQ-007 — Diagramas Documentales](../questions/rq-007-diagrams.md)      | Observa si diagramas ayudan a comparar recorridos, estructuras o diferencias de continuidad     |
| [RQ-008 — Realización semántica en VSlices Framework](../questions/rq-008-realizacion-semantica-vslices-framework.md) | Contrasta cómo Framework preserva intención, límites y autoridad durante la migración |\n
Aunque el caso puede alimentar varias RQs, no debe intentar validarlas todas con el mismo peso.

Su foco principal debería ser `RQ-008`, junto con `RQ-004`, `RQ-002`, `RQ-005` y `RQ-007` como preguntas complementarias de continuidad documental.

## Mecanismos de Docs Standard observados

### Document artifacts

El estudio puede observar Documents orientados a explicar sistemas de distinta madurez.

Artifacts especialmente relevantes:

* Context Document
* Structure Document
* Behavior Document
* Scope Document
* Consistency Document
* Decision Record
* Update Document
* Navigation Document

En sistemas heredados, estos documents pueden ayudar a reconstruir intención y comportamiento.

En el sistema con adopción parcial de VSlices Framework, pueden ayudar a verificar si la estructura técnica preserva continuidad suficiente o si requiere explicación documental adicional.

### Continuity Paths

Este estudio puede usar Continuity Paths para recorrer conocimiento entre necesidad, contexto, sistema y materialización técnica.

Paths especialmente relevantes:

* Software Project
* Software Initiative
* Domain Context
* Business Scenario
* Traceability
* Evolution
* Impact
* Ownership
* Client Product
* Consumable Service

El path de Traceability puede ser especialmente relevante para observar conexiones entre origen, decisión, comportamiento e implementación.

El path de Evolution puede ayudar a distinguir conocimiento vigente, histórico, reemplazado o parcialmente migrado.

### Nexus artifacts

El estudio puede observar si ciertos elementos requieren Nexus para explicar composición documental.

Posibles candidatos:

* capability institucional
* módulo o subsistema relevante
* servicio consumible
* integración entre sistemas
* flujo que atraviesa más de un sistema
* feature implementada con VSlices Framework
* área donde comportamiento, estructura y decisiones aparecen repartidos

El Nexus solo debería aparecer si reduce fragmentación real.

### Organizaciones documentales

El estudio puede observar cómo organizar artifacts alrededor de varios sistemas.

Posibles organizaciones:

* por sistema
* por iniciativa
* por capability
* por flujo institucional
* por estado de madurez
* por continuidad histórica
* por adopción de VSlices
* por tipo documental
* por prioridad de revisión
* por riesgo de pérdida de conocimiento

La organización debe permitir comparar sin duplicar fuentes de verdad.

### Support Notes

El estudio puede usar Support Notes para preservar:

* dudas sobre comportamiento heredado
* hipótesis de intención original
* riesgos de interpretación
* referencias a documentación existente
* resultados de revisión
* validaciones parciales
* notas sobre diferencias entre sistemas
* observaciones sobre adopción parcial de Framework

Las Support Notes pueden ser especialmente útiles cuando no existe evidencia suficiente para afirmar una decisión como vigente.

### Diagramas documentales

El estudio puede usar diagramas para representar:

* comparación entre sistemas
* continuidad entre necesidad, comportamiento e implementación
* evolución histórica
* diferencias de estructura
* rutas de trazabilidad
* zonas documentadas y zonas inciertas
* impacto entre sistemas
* adopción parcial de VSlices Framework
* composición de capabilities o servicios

Los diagramas deben mantenerse simplificados y redactados si existe riesgo de exponer información sensible.

## Conceptos de Framework observados

Este estudio contrasta conceptos provisionales de VSlices Framework en una migración real. No busca verificarlos como reglas universales: observa bajo qué condiciones preservan continuidad, dónde requieren precisión y qué costos o tensiones producen.

### Realización semántica

Se observa si la migración permite conservar una relación explicable entre intención preservada, decisiones, arquitectura, implementación y evolución, reduciendo interpretaciones incompatibles sin asumir que la documentación se convierte automáticamente en código.

### Arquitecturas y límites

Se observa la distinción entre:

* arquitectura de proyecto, que organiza una pieza internamente;
* arquitectura de solución, que organiza responsabilidades y relaciones entre piezas;
* arquitectura de despliegue, que las materializa operacionalmente.

La migración contrasta la regla de que la división semántica debe preceder a la física. Un límite lógico no implica por sí solo repositorio, proceso, almacenamiento, despliegue o comunicación de red independientes.

### Productos y Servicios

Se observa Productos y Servicios como arquitectura de solución candidata:

* los Productos organizan líneas de trabajo, experiencias, consultas y representaciones;
* los Servicios poseen conceptos, reglas, datos y capacidades delimitadas;
* las Dependencies encapsulan capacidades técnicas reutilizables y cohesionadas;
* los Nexus componen escenarios operacionales sin apropiarse de la lógica de negocio de sus componentes.

La observación debe distinguir estas responsabilidades lógicas de cualquier realización física concreta.

### Autoridad y consistencia

Se observa si cada responsabilidad mantiene ownership explícito sobre sus reglas, datos e invariantes, y si reducir acoplamiento evita duplicar autoridad, reglas o fuentes de verdad.

Cuando resulte relevante, el estudio puede analizar límites de consistencia: qué contenido e invariantes pertenecen a una misma unidad, qué autoridad los preserva y qué queda fuera de ella.

### Criterios de organización arquitectónica

Las fronteras se observan mediante criterios complementarios:

* **coherencia:** la pieza representa correctamente su propósito;
* **cohesión:** reúne elementos que pertenecen juntos;
* **acoplamiento:** sus relaciones son necesarias, explícitas y administrables.

Estos criterios son lentes de evaluación contextual, no métricas mecánicas ni pruebas de corrección.

## Preguntas operativas de Framework

Durante la migración, el estudio puede preguntar:

* ¿Qué intención, responsabilidad y autoridad permite explicar cada producto, servicio, dependency o nexus?
* ¿Qué frontera es semántica y cuál es solamente una decisión de realización actual?
* ¿Qué dependencias son necesarias y cuál es su razón semántica?
* ¿La separación propuesta conserva coherencia, cohesión y un acoplamiento administrable?
* ¿Alguna reducción de dependencia duplica reglas, datos o autoridad?
* ¿Qué presiones reales justificarían —o aún no justificarían— una separación física?
* ¿La reorganización preserva continuidad con el conocimiento y productos heredados?

## Evidencia disponible

La evidencia inicial esperada puede incluir:

* sistemas desarrollados en etapas anteriores
* sistema más reciente con adopción parcial de VSlices Framework
* documentación existente
* artifacts redactados
* decisiones técnicas recordadas o documentadas
* estructura de código revisable internamente
* diagrams simplificados
* notas de soporte
* observaciones de mantenimiento
* comparación entre enfoques técnicos
* comparación entre niveles de continuidad documental
* feedback general de personas involucradas

La evidencia publicada deberá ser resumida, redactada o transformada en ejemplos sintéticos cuando corresponda.

## Observaciones esperadas

Este estudio podría permitir observar:

* qué conocimiento es más difícil de reconstruir en sistemas heredados
* qué conocimiento se preserva mejor cuando existe una estructura técnica más explícita
* qué limitaciones tiene una adopción parcial de VSlices Framework sin Docs Standard equivalente
* si los Documents ayudan a explicar sistemas antiguos y recientes con el mismo lenguaje
* si los Continuity Paths ayudan a reconstruir trazabilidad
* si los diagramas ayudan a comparar continuidad entre sistemas
* si los Nexus reducen fragmentación en capabilities o integraciones
* si las Support Notes permiten capturar incertidumbre sin forzar conclusiones
* si la organización documental permite navegar varios sistemas sin duplicar contenido

## Evidencia faltante

Todavía falta observar:

* qué sistemas serán comparados directamente
* qué artifacts existentes pueden usarse
* qué zonas tienen conocimiento documentado
* qué zonas dependen de memoria o código
* qué partes del sistema reciente usan realmente VSlices Framework
* qué continuidad preserva la estructura técnica por sí sola
* qué continuidad requiere documentación adicional
* qué paths serán útiles para reconstruir relaciones
* qué diagramas ayudan a visualizar diferencias
* qué evidencia deberá mantenerse privada
* qué feedback entregan personas que lean los artifacts resultantes

## Criterios iniciales de observación

El estudio puede considerar señales positivas si:

* los Documents ayudan a explicar sistemas con distinta madurez
* los paths reconstruyen relaciones entre origen, comportamiento e implementación
* los diagramas aclaran diferencias sin revelar información sensible
* las Support Notes capturan incertidumbre sin convertirla en verdad documental
* los Nexus reducen fragmentación cuando un elemento cruza varios artifacts
* la organización documental permite comparar sistemas sin duplicar contenido
* la adopción parcial de Framework hace más visible alguna continuidad técnica
* el análisis permite distinguir conocimiento vigente, histórico, incierto o reemplazado

El estudio puede considerar señales problemáticas si:

* se asume que Framework equivale automáticamente a continuidad
* los sistemas heredados se juzgan injustamente con criterios actuales
* los paths generan reconstrucciones demasiado especulativas
* los diagramas simplificados pierden evidencia relevante
* las Support Notes acumulan dudas sin cierre
* los Documents duplican documentación existente
* la comparación se vuelve narrativa de superioridad y no observación
* la privacidad impide sostener afirmaciones con evidencia suficiente

## Riesgos metodológicos

### Riesgo de comparación injusta

Los sistemas heredados fueron construidos en condiciones distintas.

No deben evaluarse como si hubieran tenido acceso a VSlices Method, Docs Standard o Framework actuales.

### Riesgo de narrativa triunfalista

El estudio no debe concluir que el sistema con adopción parcial de VSlices Framework es superior por definición.

Debe observar diferencias concretas de continuidad, límites y costos.

### Riesgo de confundir estructura técnica con continuidad completa

Una estructura técnica más explícita puede ayudar, pero no reemplaza necesariamente contexto, decisiones, dominio, alcance o evolución documentada.

### Riesgo de reconstrucción retrospectiva

Al analizar sistemas antiguos, parte de la intención original puede inferirse desde código o memoria.

Esa inferencia debe marcarse como tal.

### Riesgo de privacidad

El caso contiene información institucional privada.

La necesidad de redactar evidencia puede limitar la verificabilidad externa del estudio.

### Riesgo de atribuir diferencias solo a VSlices

Las diferencias entre sistemas pueden deberse a:

* cambios de experiencia del equipo
* cambios tecnológicos
* cambios de contexto
* presión de entrega
* tamaño del sistema
* disponibilidad de usuarios
* requisitos institucionales
* madurez profesional acumulada

VSlices puede ser un factor, pero no debe asumirse como única explicación.

## Límites del estudio

Este estudio no puede demostrar que VSlices Framework mejora universalmente la continuidad de conocimiento.

No puede publicar toda la evidencia directa.

No puede comparar sistemas como si hubieran sido desarrollados bajo las mismas condiciones.

No puede aislar completamente el efecto de VSlices frente a experiencia, contexto, tecnología o madurez del equipo.

No debe concluir que todo sistema heredado necesita ser reorganizado bajo VSlices.

Su valor está en observar diferencias locales de continuidad entre sistemas con distinta historia y en identificar qué mecanismos de Docs Standard ayudan a explicar, reconstruir o comparar esas diferencias.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre continuidad en sistemas heredados
* Observations sobre adopción parcial de VSlices Framework
* Tensions entre reconstrucción retrospectiva y evidencia directa
* Tensions entre estructura técnica y explicación documental
* Findings locales sobre utilidad o límites de Documents, Paths, Organizations, Notes, Nexus y Diagrams
* criterios para documentar sistemas antiguos sin reescribir toda su historia
* criterios para acompañar VSlices Framework con Docs Standard
* límites explícitos sobre evidencia privada redactada

## Relación con estudios fundacionales

Este estudio se relaciona especialmente con escenarios de pérdida histórica y dispersión activa de conocimiento.

Puede alimentar `SYN-0001` al observar cómo conocimiento de sistemas antiguos puede degradarse, dispersarse o depender de inferencias retrospectivas.

También puede complementar `STU-006`, porque ambos observan sistemas de largo plazo, pero desde enfoques distintos:

* `STU-006` observa continuidad documental sostenida en un sistema operacional vivo
* `STU-007` observa contraste entre sistemas heredados y adopción parcial de VSlices Framework

## Límite actual

Este estudio debe mantenerse en estado `candidate` mientras no se haya revisado evidencia suficiente.

El caso es metodológicamente valioso porque permite contrastar sistemas construidos en distintas etapas de madurez técnica y documental.

Sin embargo, por su carácter privado, institucional y parcialmente retrospectivo, sus conclusiones deben formularse con especial prudencia y distinguir claramente entre evidencia observada, reconstrucción inferida e interpretación local.

## Alcance del estudio

Este estudio observa la continuidad de sistemas institucionales existentes durante una adopción parcial de VSlices Framework.

Su alcance incluye recuperar y organizar el conocimiento necesario para evolucionar productos ya realizados, y migrarlos progresivamente hacia una arquitectura de Productos y Servicios. Esta migración no constituye un caso independiente: es una fase de la misma adopción, orientada a preservar, clarificar y extender responsabilidades preexistentes.

En particular, se observará:

* cómo se identifican y preservan límites semánticos, responsabilidades, autoridad e invariantes al reorganizar productos existentes;
* cómo una división semántica puede preceder —sin exigir— una separación física de repositorios, procesos, bases de datos o despliegues;
* la realización progresiva de productos, comenzando por gestión de cuentas, y las fases posteriores de pavimentación y gestión de solicitudes;
* las dependencias e integraciones que aparezcan entre productos, servicios, dependencies y nexus;
* las tensiones entre desacoplamiento, coordinación y preservación de una fuente de verdad autoritativa;
* la continuidad entre intención, comportamiento, estructura, decisiones, implementación y evolución.

La evidencia se registrará de forma anonimizada o sintética cuando sea necesario.

## Fuera de alcance

Este estudio no busca demostrar que Productos y Servicios sea una arquitectura universal ni comparar exhaustivamente todas las arquitecturas posibles.

Tampoco evalúa una migración institucional completa, una separación obligatoria hacia microservicios ni independencia física por defecto. Las decisiones de despliegue, persistencia, repositorio o proceso se observarán sólo cuando fuerzas reales del caso las vuelvan relevantes.

El estudio no trata cada producto realizado como un caso independiente mientras su propósito principal siga siendo dar continuidad al sistema y a los productos preexistentes. Si en el futuro aparece un caso cuyo problema práctico central deje de ser esa continuidad y requiera evidencia propia, su frontera podrá revisarse entonces.

## Límite actual

Este estudio se mantiene en estado `candidate` mientras no exista evidencia suficiente.

Por su carácter institucional, privado y parcialmente retrospectivo, sus conclusiones deberán distinguir con especial prudencia entre evidencia observada, reconstrucción inferida e interpretación local. El estudio contrasta conceptos candidatos de Docs Standard y Framework; no los valida universalmente ni atribuye por defecto toda diferencia observada a VSlices.
