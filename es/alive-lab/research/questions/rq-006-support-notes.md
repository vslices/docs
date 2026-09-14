---
type: research-question
state: candidate
code: RQ-006

related_questions:
* RQ-001
* RQ-004

related_notes:
* RN-0001
* RN-0002

related_synthesis:
* SYN-0001

related_studies: []

affects:
* VSlices Research
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
---

# RQ-006 — Notas de Soporte

## Pregunta

¿En qué condiciones las Support Notes ayudan a preservar conocimiento auxiliar, incompleto o temporal sin promoverlo prematuramente a Document artifact ni convertirse en un contenedor genérico de información no clasificada?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0002-vslices-docs-standard.md).

Inicialmente, las Support Notes aparecían como mecanismo auxiliar dentro de Docs Standard.

Sin embargo, su responsabilidad es suficientemente distinta de los Document artifacts como para requerir una pregunta de investigación propia.

Las Support Notes no explican una pregunta documental principal.

Apoyan, registran o referencian conocimiento auxiliar.

## Problema observado

Durante el trabajo de software aparece conocimiento que conviene preservar, pero que todavía no merece convertirse en documento principal.

Por ejemplo:

* una idea incompleta
* una hipótesis
* un resultado observado
* una validación preliminar
* un riesgo
* una referencia externa
* una especificación de prueba
* una duda abierta
* una evidencia auxiliar
* una condición temporal
* una interpretación pendiente

Si este conocimiento no se registra, puede perderse.

Si se formaliza demasiado pronto como Document artifact, puede generar burocracia, falsa madurez o documentos difíciles de mantener.

## Hipótesis inicial

Las Support Notes podrían ayudar a preservar continuidad al ofrecer una zona documental liviana para conocimiento auxiliar, incompleto o temporal.

Su valor estaría en evitar pérdida de conocimiento sin promoverlo prematuramente a documento principal.

Su riesgo estaría en convertirse en un contenedor genérico para información no clasificada.

## Qué busca observar esta pregunta

Esta pregunta busca observar si las Support Notes ayudan a:

* capturar conocimiento incompleto
* preservar resultados observados
* separar resultado de interpretación
* registrar validaciones frente a criterios
* documentar riesgos sin crear documentos mayores
* referenciar artifacts externos
* derivar testing desde comportamiento esperado
* mantener evidencia auxiliar disponible
* evitar documentos prematuros
* decidir cuándo promover una nota a Document artifact

También busca observar cuándo una Support Note deja de ser útil.

## Mecanismo candidato

El mecanismo candidato es la **Support Note**.

Tipos candidatos iniciales:

| Support Note | Pregunta                                            |
| ------------ | --------------------------------------------------- |
| draft        | ¿Qué estamos esbozando?                             |
| result       | ¿Qué obtuvimos?                                     |
| validation   | ¿Qué significa lo obtenido frente a un criterio?    |
| testing-spec | ¿Cómo probaremos este comportamiento?               |
| risk         | ¿Qué podría salir mal?                              |
| external     | ¿Dónde vive el artifact externo y cómo debe usarse? |

Una Support Note:

* apoya un artifact, concepto o elemento principal
* puede contener conocimiento incompleto
* no reemplaza un Document artifact
* no reemplaza un Nexus
* no reemplaza un Continuity Path
* puede promoverse a Document si empieza a responder una pregunta documental principal

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [RQ-004](../questions/rq-004-documents.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* el modelo candidato de Docs Standard
* los templates candidatos de Support Notes
* la separación candidata entre Result, Validation y Feedback
* la regla candidata de promoción desde Support Note hacia Document artifact

## Evidencia faltante

Todavía falta observar:

* si las Support Notes evitan pérdida de conocimiento auxiliar
* si reducen documentación prematura
* si las personas distinguen draft, result, validation, testing-spec, risk y external
* si una Support Note tiene siempre un objeto soportado claro
* si las Support Notes se mantienen livianas
* si se sabe cuándo promover una nota a Document artifact
* si se sabe cuándo eliminar, cerrar o superseder una Support Note
* si se convierten en cajón de información no clasificada
* si ayudan a preservar evidencia durante iteraciones reales

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde aparezca conocimiento útil pero inmaduro.

Posibles escenarios:

* una hipótesis de dominio en Domus Orbis
* una clasificación candidata de productos domésticos
* un resultado observado al usar un artifact YAML
* una validación de comportamiento esperado
* una especificación de prueba derivada de un Behavior Document
* un riesgo asociado a una decisión documental
* una referencia externa usada para consumir un servicio
* una nota de handoff durante transición de conocimiento

## Riesgos metodológicos

### Riesgo de convertir Support Note en cajón de sastre

Si todo conocimiento no clasificado termina como Support Note, la familia pierde intención.

### Riesgo de evitar documentos necesarios

Una Support Note no debe usarse para postergar indefinidamente un Document artifact que ya es necesario.

### Riesgo de confundir Result, Validation y Feedback

Registrar lo ocurrido, interpretar frente a criterio y capturar respuesta externa son responsabilidades distintas.

### Riesgo de acumular notas sin ciclo de vida

Las Support Notes necesitan criterios para mantenerse, promoverse, cerrarse, reemplazarse o descartarse.

## Relación con Docs Standard

Esta pregunta puede afectar:

* definición de Support Notes
* tipos candidatos de Support Note
* reglas de promoción a Document
* relación entre Support Notes y Evidence
* relación entre Result, Validation y Feedback
* relación con Behavior Documents y testing-spec
* relación con Continuity Paths
* relación con Nexus
* futura validación por Tooling

## Relación con RQ-004

[RQ-004](../questions/rq-004-documents.md) investiga Document artifacts.

RQ-006 investiga Support Notes.

La relación entre ambas preguntas es importante porque una Support Note puede convertirse en Document artifact si crece hasta responder una pregunta documental principal.

Esta relación debe observarse con cuidado para evitar dos fallas:

* promover conocimiento auxiliar demasiado temprano
* mantener como nota algo que ya necesita explicación documental principal

## Límite actual

Esta pregunta no asume que las Support Notes funcionan.

Solo propone investigarlas como mecanismo candidato para preservar conocimiento auxiliar, incompleto o temporal sin sobreformalizarlo.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.

Con esto ya tenemos el bloque Docs Standard separado en mecanismos investigables. El siguiente paso natural sería mapear los 3 studies contra estas 5 RQs, para que cada caso observe una combinación pequeña y no intentemos probar todo el estándar de una sola vez.
