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
- VSlices Research
- VSlices Docs Standard
- VSlices Method
- VSlices Framework
* VSlices Tooling
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

Aunque el caso puede alimentar varias RQs, no debe intentar validarlas todas con el mismo peso.

Su foco principal debería ser `RQ-004`, `RQ-002`, `RQ-005` y `RQ-007`.

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

Este estudio observa la continuidad de un sistema institucional existente durante una adopción parcial de VSlices Framework.

Su alcance incluye la recuperación y organización del conocimiento necesario para evolucionar productos ya realizados, y la migración progresiva hacia una arquitectura de Productos y Servicios. La migración no se considera un caso independiente: constituye una fase de la misma adopción, orientada a preservar, clarificar y extender la continuidad de las responsabilidades ya existentes.

En particular, se observará:

* cómo se identifican y preservan límites semánticos, responsabilidades y autoridad al reorganizar productos existentes;
* cómo una división semántica puede preceder —sin exigir— una separación física de repositorios, procesos, bases de datos o despliegues;
* la realización progresiva de productos, comenzando por gestión de cuentas, y las fases posteriores de pavimentación y gestión de solicitudes;
* las dependencias e integraciones que aparezcan entre productos y servicios;
* las tensiones entre desacoplamiento, coordinación y preservación de una fuente de verdad autoritativa;
* la continuidad entre intención, comportamiento, estructura, decisiones e implementación durante la evolución.

La evidencia se registrará de forma anonimizada o sintética cuando sea necesario.

## Fuera de alcance

Este estudio no busca demostrar que una arquitectura de Productos y Servicios sea universalmente adecuada ni comparar exhaustivamente todas las arquitecturas posibles.

Tampoco evalúa una migración institucional completa, una separación obligatoria hacia microservicios, ni independencia física por defecto. Las decisiones de despliegue, persistencia, repositorio o proceso se observarán sólo cuando las fuerzas reales del caso las vuelvan relevantes.

El estudio no trata cada producto realizado como un caso independiente mientras su propósito principal siga siendo dar continuidad al sistema y a los productos preexistentes.
existentes.

Su foco actual no es cubrir el desarrollo completo de nuevos módulos, sino mantener una línea viva de observación sobre continuidad en sistemas existentes y en soporte institucional.

## Relación con módulos o sistemas futuros

A partir de noviembre se espera retomar comunicación para generación de nuevos módulos o sistemas.

Cuando aparezca un nuevo módulo o sistema con alcance propio, duración significativa o proceso completo de descubrimiento, documentación, desarrollo y validación, ese trabajo no debería absorberse dentro de `STU-007`.

En esos casos se deberá crear un nuevo Study independiente.

La regla candidata es:

> `STU-007` observa continuidad en puntos especificos solicitados por PO, incluyendo en un inicio una documentación sistemas existentes.
> 
> Cada nuevo módulo o sistema con ciclo propio de desarrollo debe generar su propio Study.

Esto es importante porque los nuevos módulos suelen implicar varios meses de trabajo y pueden activar toda la suite VSlices:

* VSlices Design
* VSlices Docs Standard
* VSlices Method
* VSlices Framework
* VSlices Tooling

Cada nuevo módulo puede producir evidencia suficiente para una pregunta local propia, artifacts propios, decisiones propias y findings locales propios.

Por lo tanto, `STU-007` puede actuar como study base, pero no debe convertirse en contenedor de todos los futuros módulos.

## Studies derivados esperados

Este estudio puede generar a futuro una familia de studies derivados.

La estructura candidata es:

```text
STU-007
  Caso base actualizable mes a mes
  Continuidad, documentación, soporte y entendimiento de sistemas existentes

STU-XXX
  Contrato de soporte Serviu, una vez finalizada la documentación inicial del STU-007.

STU-YYY
  Nuevo módulo o sistema 1

STU-ZZZ
  Nuevo módulo o sistema 2

STU-NNN
  Nuevo módulo o sistema N
```

El patrón esperado es:

```text
1 + N studies derivados
```

Donde:

* `1` corresponde al study dedicado al contrato de soporte
* `N` corresponde a la cantidad de nuevos módulos o sistemas desarrollados posteriormente

Esta separación evita mezclar soporte continuo, documentación de sistemas existentes y desarrollo de nuevos módulos en un solo artifact de investigación.

## Diferencia con el STU-006

Este caso se parece parcialmente al caso de Hual que se cubrire en los [STU-011](./stu-011-digitalizacion-escenario-uso-vslices.md) y [STU-012](./stu-012-mejora-capacidad-limitada-uso-vslices.md) sobre módulos nuevos y mejora continua, pero tiene una diferencia contractual importante.

En esos STU, el escenario esperado combina:

```text
Mejoras continuas + soporte
dentro de una bolsa limitada de 25 horas mensuales
```

En Serviu, el escenario esperado se separa en dos líneas:

```text
Digitalización continua
por un lado

Contrato de soporte con bolsa ilimitada de horas
por otro lado
```

Esto cambia la naturaleza de la investigación.

En Hual, la restricción principal es maximizar valor con capacidad mensual limitada.

En Serviu, la tensión principal puede aparecer entre soporte abierto, continuidad institucional, nuevos módulos de larga duración y convivencia entre sistemas legacy y sistemas nuevos.

Por eso, el contrato de soporte de Serviu debería tratarse como un study.

## Ajuste al límite del estudio

Este estudio debe mantenerse como un caso vivo y actualizable mes a mes.

Sus conclusiones deben interpretarse según el alcance observado en cada período.

`STU-007` no debe absorber automáticamente nuevos módulos, nuevos sistemas o el contrato de soporte completo.

Cuando aparezcan líneas de trabajo con alcance propio, especialmente desarrollos de varios meses o soporte institucional continuo, deberán abrirse studies derivados.

El valor de `STU-007` está en funcionar como caso base para observar continuidad en sistemas existentes, documentación de aplicaciones legacy, adopción parcial de VSlices Framework y evolución mensual del conocimiento disponible.

## Fuera de alcance

Queda fuera de alcance:

* juzgar los sistemas legacy con criterios actuales como si hubieran nacido con VSlices
* demostrar que VSlices Framework es superior por definición
* publicar detalles internos completos de los sistemas
* reconstruir toda la historia técnica de las aplicaciones
* convertir inferencias retrospectivas en evidencia directa
* validar universalmente la relación entre Framework y continuidad documental

El valor del estudio está en observar diferencias locales de continuidad entre sistemas heredados, documentación para entendimiento profundo y una Proof of Concept más cercana a VSlices.
