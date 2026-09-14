---
type: research-question
state: candidate
code: RQ-008

related_questions:
* RQ-001
* RQ-002
* RQ-003
* RQ-004
* RQ-005
* RQ-006
* RQ-007

related_notes:
* RN-0001
* RN-0002
* RN-0003
* RN-0004

related_synthesis:
* SYN-0001

related_studies: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
---

# RQ-008 — Asistencia de IA en VSlices Docs Standard

## Pregunta

¿En qué condiciones la asistencia de IA puede orientarse para producir, revisar o conectar artifacts de VSlices Docs Standard sin reemplazar evidencia, introducir sobreformalización, aumentar ruido documental ni debilitar la trazabilidad del conocimiento?

## Estado

candidate

## Nivel de exploración

Esta pregunta es altamente exploratoria.

Es más exploratoria que [RQ-007 — Diagramas Documentales](./rq-007-diagrams.md)

En `RQ-007`, al menos existen representaciones candidatas iniciales, como el Diagrama de Camino de Continuidad y el Diagrama de Ramificación de Preguntas.

En esta pregunta, el problema es más abierto:

> Sabemos parcialmente qué no debería hacer la IA, pero todavía no sabemos cómo orientarla de forma confiable para que ayude según los criterios de VSlices Docs Standard.

Por ahora no existe un método estable para:

* preparar contexto para IA
* limitar inferencias
* validar salidas
* medir señal y ruido
* distinguir evidencia de propuesta
* generar prompts reutilizables
* controlar privacidad
* evitar sobreformalización
* revisar trazabilidad
* decidir cuándo una salida asistida por IA es aceptable

Por eso esta RQ debe mantenerse como exploratoria y no debe convertirse todavía en práctica oficial de VSlices.

## Origen

Esta pregunta surge desde [RN-0004 — Asistencia de IA en la producción y revisión de artifacts documentales](../notes/rn-0004-asistencia-IA-vslices-docs-standard.md).

La nota propone que la IA puede apoyar producción, revisión, síntesis y conexión de artifacts documentales, pero solo si se mantiene subordinada a evidencia, intención documental, trazabilidad y revisión humana.

La pregunta aparece porque VSlices Docs Standard contiene varios puntos que podrían beneficiarse de asistencia de IA:

* Document artifacts
* Support Notes
* Continuity Paths
* Nexus artifacts
* Organizaciones documentales
* Diagramas documentales
* redacción de handoff
* revisión de claridad
* reducción de ruido
* detección de gaps
* generación de versiones redactadas o simplificadas

Sin embargo, todavía no sabemos cómo orientar la IA para que actúe dentro de límites metodológicos seguros.

## Problema observado

La IA puede producir documentación clara, estructurada y convincente.

Pero esa claridad puede ser engañosa si no existe trazabilidad.

La IA puede:

* completar vacíos con conocimiento implícito
* inventar relaciones plausibles
* suavizar incertidumbres
* transformar hipótesis en afirmaciones
* generar documentos demasiado pulidos
* producir diagramas visualmente atractivos pero ruidosos
* resumir perdiendo señal relevante
* agregar contenido que parece útil pero no responde la pregunta documental
* mezclar evidencia, interpretación y propuesta
* aumentar ceremonia documental
* exponer información sensible si se usa sin control

El problema no es solo usar o no usar IA.

El problema es orientar su uso para que mejore continuidad documental sin sustituir el criterio humano ni la evidencia del caso.

## Hipótesis inicial

La asistencia de IA podría ser útil para VSlices Docs Standard si se orienta mediante estructuras explícitas:

* artifact type
* pregunta documental principal
* estado del conocimiento
* evidencia disponible
* límites del caso
* tipo de salida esperada
* criterios de señal y ruido
* reglas de privacidad
* distinción entre evidencia, inferencia y propuesta
* revisión humana posterior

La hipótesis candidata es:

> Mientras más explícitos sean los artifacts, preguntas, relaciones y límites de VSlices Docs Standard, menor será el espacio donde la IA deba rellenar con conocimiento implícito no trazable.

## Qué busca observar esta pregunta

Esta pregunta busca observar:

* cómo preparar contexto para IA sin exponer información innecesaria
* cómo orientar la IA hacia una pregunta documental específica
* cómo evitar que la IA mezcle responsabilidades documentales
* cómo detectar si una salida aumentó señal o solo agregó texto
* cómo detectar si una salida redujo ruido o perdió señal relevante
* cómo revisar trazabilidad de una salida asistida por IA
* cómo distinguir evidencia, interpretación y sugerencia
* cómo evitar que una salida candidate parezca validated
* cómo usar IA sin aumentar ceremonia documental
* cómo usar IA en casos privados o redactados
* cómo Tooling podría estructurar mejor el uso de IA

También busca observar cuándo la IA no debería usarse.

## Mecanismo candidato

El mecanismo candidato no es un artifact de Docs Standard.

El mecanismo candidato es la **asistencia de IA orientada por Docs Standard**.

Esto significa que la IA podría actuar como apoyo para:

* redactar
* reescribir
* resumir
* revisar
* estructurar
* detectar gaps
* sugerir relaciones
* proponer paths
* proponer diagramas
* simplificar contenido
* transformar evidencia en artifacts
* preparar versiones redactadas
* revisar señal y ruido

Pero siempre bajo revisión humana y con trazabilidad hacia evidencia.

## Relación con señal y ruido

Esta RQ usa señal y ruido como lente conceptual candidato.

No se propone todavía como métrica formal.

### Aumentar señal

Cuando la IA se use para aumentar señal, debería agregar claridad, estructura, precisión o relaciones relevantes.

Como mínimo:

> Debe mantener el mismo nivel de ruido relativo.

Preferiblemente:

> Debe reducir el ruido relativo mientras aumenta la señal.

### Reducir ruido

Cuando la IA se use para reducir ruido, debería eliminar redundancia, ambigüedad, decoración o contenido que no responde la pregunta documental.

Como mínimo:

> Debe reducir la señal lo menos posible.

Preferiblemente:

> Debe mantener el nivel relativo de señal mientras reduce ruido.

### Regla candidata

La salida asistida por IA debería evaluarse así:

> La IA ayuda solo si mejora la relación señal/ruido sin debilitar evidencia, límites, trazabilidad ni responsabilidad documental.

## Relación con Documents

La IA puede ayudar a producir o revisar Document artifacts si se le entrega:

* tipo de documento
* pregunta principal
* target
* estado
* evidencia disponible
* límites
* artifacts relacionados
* nivel de detalle esperado

Puede apoyar:

* claridad
* estructura
* separación de responsabilidades
* reducción de contenido fuera de pregunta
* detección de secciones excesivas
* identificación de contenido que debería moverse a otro artifact

### Riesgo

La IA puede producir un documento que parece completo, pero que no responde a evidencia suficiente o mezcla responsabilidades.

## Relación con Support Notes

La IA puede ayudar a capturar conocimiento auxiliar en Support Notes.

Puede apoyar:

* transformar conversaciones en notas pequeñas
* separar draft, result, validation, risk, testing-spec y external
* conservar dudas
* registrar límites
* evitar documentos prematuros

### Riesgo

La IA puede hacer que una nota incompleta parezca más madura que la evidencia disponible.

## Relación con Continuity Paths

La IA puede sugerir posibles relaciones, rutas o gaps dentro de un Continuity Path.

Puede apoyar:

* detectar conceptos conectados
* proponer paths relacionados
* identificar artifacts existentes
* identificar posibles necesidades documentales
* simplificar recorridos

### Riesgo

La IA puede inventar continuidad.

Una relación sugerida por IA debe tratarse como candidata hasta ser revisada contra evidencia.

## Relación con Nexus

La IA puede sugerir composiciones candidatas entre artifacts.

Puede apoyar:

* identificar artifacts participantes
* distinguir composición de relación auxiliar
* detectar artifacts faltantes
* revisar duplicación
* simplificar un nexus excesivo

### Riesgo

La IA puede crear composiciones artificiales que se ven ordenadas pero no reducen fragmentación real.

## Relación con Organizaciones Documentales

La IA puede sugerir organizaciones, agrupaciones o proyecciones navegables.

Puede apoyar:

* detectar duplicación
* sugerir rutas de lectura
* agrupar artifacts por criterio
* identificar posibles fuentes de verdad
* revisar si una proyección copia contenido canónico

### Riesgo

La IA puede confundir organización con fuente de verdad o proponer estructuras difíciles de mantener.

## Relación con Diagramas Documentales

La IA puede generar o revisar diagramas.

Puede apoyar:

* Mermaid inicial
* leyendas
* nodos
* rutas principales y auxiliares
* simplificación de mapas
* detección de ruido visual
* representación de gaps
* representación de estados documentales

### Riesgo

La IA puede generar diagramas bonitos, pero visualmente ruidosos o metodológicamente ambiguos.

## Relación con Tooling

Tooling podría ser una pieza clave para orientar IA.

Puede ayudar a:

* preparar contexto mínimo
* generar prompts estructurados
* inyectar metadata relevante
* excluir campos sensibles
* listar artifacts relacionados
* marcar evidencia disponible
* marcar inferencias
* validar front-matter
* revisar campos derivados
* comparar salida contra reglas de Docs Standard
* detectar relaciones no existentes
* registrar qué fue generado, revisado o modificado con IA

La relación candidata es:

- Docs Standard define intención y responsabilidad documental
- Tooling prepara contexto, límites y validaciones
- IA asiste producción, revisión o síntesis
- Humanos verifican evidencia, sentido y privacidad

Esta relación todavía debe observarse.

## Relación con STU-005

[STU-005](../studies/stu-005-transferencia-conocimiento-ecosistema-asegurador-empresarial.md) puede ser el primer caso donde esta RQ aparezca con fuerza.

La transferencia de conocimiento puede usar IA para:

* estructurar handoff
* redactar documentos
* proponer paths
* simplificar diagramas
* preparar versiones redactadas
* revisar claridad
* detectar gaps
* sintetizar conocimiento disperso

Pero por ser un caso privado, la IA debe operar con restricciones estrictas.

En `STU-005`, esta RQ puede observar:

* si la IA acelera documentación sin perder señal
* si ayuda a reducir ruido en handoff
* si introduce inferencias no verificadas
* si permite redactar evidencia privada sin exponer contenido sensible
* si ayuda a preparar documentación más legible para lectores reales
* si requiere Tooling o prompts estructurados para ser confiable

## Evidencia inicial disponible

La evidencia inicial es conceptual y práctica, pero todavía informal.

Proviene de:

* uso de IA para estructurar artifacts de VSlices Research
* generación asistida de Research Notes, Research Questions y Studies
* revisión de conceptos candidatos de Docs Standard
* necesidad de preparar documentación de handoff en `STU-005`
* necesidad de manejar privacidad
* necesidad de reducir ruido documental
* necesidad de aumentar señal en artifacts pequeños
* aparición de señal, ruido y trazabilidad como criterios candidatos

Esta evidencia todavía no valida la RQ.

Solo justifica abrirla.

## Evidencia faltante

Todavía falta observar:

* qué tipo de prompt orienta mejor a la IA
* qué contexto mínimo necesita la IA
* qué contexto aumenta ruido
* qué reglas reducen alucinación
* qué salidas requieren más revisión humana
* qué artifacts son más asistibles por IA
* qué artifacts son riesgosos de asistir
* cómo medir si aumentó señal
* cómo medir si redujo ruido
* cómo registrar uso de IA en artifacts
* cómo controlar privacidad
* cómo distinguir salida IA, revisión humana y evidencia
* si Tooling puede mejorar la calidad de asistencia
* si lectores reales perciben mejora
* si IA reduce costo sin bajar calidad

## Posibles casos de estudio

Esta pregunta puede observarse en:

* `STU-005`, durante transferencia de conocimiento y handoff privado
* [STU-008](../studies/stu-008-construccion-producto-desde-cero-con-vslices-dominio-domestico.md), durante construcción progresiva de Domus Orbis
* [STU-009](../studies/stu-009-tooling-interno-para-generacion-mantenimiento-artifacts-documentales.md), al diseñar Tooling que prepare contexto y valide outputs
* [STU-010](../studies/stu-010-navegacion-documental-proyecciones-locales-mediante-surreal-atlas.md), al generar o revisar proyecciones, diagramas y navegación documental
* futuros studies de módulos nuevos, donde IA pueda asistir discovery, documentación e implementación

## Criterios iniciales de observación

La asistencia de IA podría considerarse útil si:

* reduce esfuerzo repetitivo
* mejora claridad del artifact
* mantiene evidencia visible
* mantiene límites explícitos
* distingue inferencia de observación
* evita inventar relaciones
* mejora señal sin aumentar ruido relativo
* reduce ruido sin perder señal relevante
* ayuda a detectar gaps reales
* respeta privacidad
* produce outputs revisables
* no convierte candidate en validated
* no reemplaza conversaciones necesarias

La asistencia de IA podría considerarse problemática si:

* produce contenido plausible sin evidencia
* agrega texto que no responde la pregunta documental
* mezcla responsabilidades de artifacts
* oculta incertidumbre
* elimina matices importantes
* inventa relaciones
* genera diagramas ruidosos
* aumenta ceremonia
* dificulta revisión humana
* depende de conocimiento implícito no trazable
* expone información sensible
* hace parecer suficiente una transferencia incompleta

## Riesgos metodológicos

### Riesgo de orientación insuficiente

Sin estructura clara, la IA puede completar vacíos con conocimiento implícito no verificable.

### Riesgo de señal aparente

Una salida puede parecer más informativa porque es más larga, más ordenada o más elegante, sin reducir incertidumbre real.

### Riesgo de pérdida de señal

Al resumir o simplificar, la IA puede eliminar matices, evidencia, límites o contradicciones importantes.

### Riesgo de ruido documental

La IA puede agregar secciones, relaciones, ejemplos o diagramas que aumentan carga cognitiva.

### Riesgo de sobreformalización

La IA puede convertir ideas inmaduras en artifacts demasiado pulidos.

### Riesgo de privacidad

El uso de IA en casos privados puede exponer información sensible si no existe redacción previa o control de contexto.

### Riesgo de validación circular

VSlices puede definir criterios, generar artifacts con IA y luego evaluar esos artifacts con los mismos supuestos.

### Riesgo de dependencia operativa

Si el equipo depende demasiado de IA, puede perder criterio documental propio.

## Límites del estudio

Esta pregunta no busca demostrar que la IA mejora Docs Standard.

No busca definir una metodología completa de AI-assisted documentation todavía.

No busca crear prompts oficiales.

No busca adoptar teoría de la información como métrica formal.

No busca reemplazar revisión humana.

No busca convertir IA en fuente de evidencia.

Su valor está en observar cómo podría orientarse la IA para asistir documentación bajo criterios de continuidad, trazabilidad, señal, ruido y privacidad.

## Resultado esperado

El resultado esperado no es una validación completa.

El resultado esperado es producir evidencia suficiente para derivar:

* Observations sobre asistencia de IA
* Tensions entre productividad, trazabilidad y privacidad
* Tensions entre señal, ruido y sobreformalización
* criterios candidatos de prompting
* criterios candidatos de revisión humana
* criterios candidatos para Tooling
* límites sobre uso de IA en casos privados
* posibles ajustes a Docs Standard
* posibles findings locales sobre qué artifacts son más o menos asistibles

## Relación con futuras decisiones de VSlices

Esta RQ podría afectar futuras decisiones sobre:

* VSlices Docs Standard
* VSlices Tooling
* prompts estructurados
* generación asistida de artifacts
* revisión asistida de documentación
* detección de ruido documental
* reducción de ceremony
* políticas de privacidad
* trazabilidad entre evidencia y salida generada
* Surreal Atlas como apoyo para navegación de conocimiento asistida

## Límite actual

Esta pregunta debe mantenerse en estado `candidate`.

Es una de las preguntas más exploratorias del bloque Docs Standard.

Antes de convertirla en práctica oficial, VSlices Research debe observar cómo orientar la IA en casos concretos, especialmente cuando existen restricciones de privacidad, evidencia incompleta, artifacts candidate y necesidad de revisión humana.

La pregunta central no es:

> ¿La IA ayuda a documentar?

La pregunta central es:

> ¿Cómo orientamos la IA para que aumente señal, reduzca ruido y preserve trazabilidad sin reemplazar evidencia ni criterio humano?
