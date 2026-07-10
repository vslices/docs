---
type: research-question
state: candidate
code: RQ-004

related_questions:
* RQ-001

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

# RQ-004 — Documentos

## Pregunta

¿En qué condiciones los Document artifacts definidos por preguntas principales ayudan a preservar conocimiento sin imponer plantillas rígidas ni documentación excesiva?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0002-vslices-docs-standard.md).

Docs Standard propone que los Document artifacts no se definan principalmente por formato, sino por la pregunta documental principal que responden.

La idea aparece como respuesta candidata a un problema común: muchos documentos mezclan contexto, comportamiento, decisiones, estructura, alcance, feedback y validación sin una responsabilidad clara.

## Problema observado

En proyectos de software, la documentación puede fallar de dos formas opuestas.

Puede ser insuficiente, dejando conocimiento importante implícito o disperso.

También puede ser excesiva, generando plantillas rígidas, secciones obligatorias y documentos que nadie mantiene.

Cuando un documento no tiene una pregunta principal clara, puede mezclar responsabilidades como:

* explicar contexto
* describir comportamiento
* registrar decisiones
* definir alcance
* documentar estructura
* capturar feedback
* preservar reglas
* evaluar viabilidad
* orientar navegación

Esta mezcla puede dificultar la continuidad porque no queda claro qué intención documental debe mantenerse.

## Hipótesis inicial

Los Document artifacts definidos por preguntas principales podrían preservar mejor continuidad porque cada documento tendría una responsabilidad explícita.

Su valor estaría en ayudar a decidir qué conocimiento pertenece al documento, qué debe vivir en otro artifact y qué puede omitirse.

Su riesgo estaría en convertir cada pregunta derivada en sección obligatoria o usar el mapa completo como plantilla rígida.

## Qué busca observar esta pregunta

Esta pregunta busca observar si los Document artifacts ayudan a:

* preservar intención documental
* elegir el tipo de documento correcto
* separar responsabilidades
* evitar documentos ambiguos
* activar solo los segmentos necesarios
* evitar plantillas excesivas
* preservar conocimiento suficiente con baja ceremonia
* distinguir cuerpo, metadata y relaciones
* evitar duplicación entre artifacts

También busca observar cuándo un Document artifact no aporta valor o introduce costo innecesario.

## Mecanismo candidato

El mecanismo candidato es el **Document artifact**.

Document artifacts candidatos iniciales:

* Navigation Document
* Domain Vocabulary
* Context Document
* Structure Document
* Behavior Document
* Consistency Document
* Scope Document
* Viability Document
* Update Document
* Feedback Document
* Decision Record

Cada Document artifact responde una pregunta documental principal.

Ejemplos:

| Document artifact    | Pregunta principal  |
| -------------------- | ------------------- |
| Context Document     | ¿Dónde existe?      |
| Behavior Document    | ¿Qué debe ocurrir?  |
| Structure Document   | ¿Cómo se organiza?  |
| Consistency Document | ¿Qué debe respetar? |
| Scope Document       | ¿Hasta dónde llega? |
| Decision Record      | ¿Qué se decidió?    |

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* el modelo candidato de Docs Standard
* el índice candidato de Document artifacts
* los templates candidatos de Document artifacts
* la regla de que la pregunta principal define la identidad documental

## Evidencia faltante

Todavía falta observar:

* si la pregunta principal ayuda realmente a escribir documentos más claros
* si los usuarios distinguen tipos documentales por pregunta y no por plantilla
* si los documentos mínimos preservan suficiente continuidad
* si el mapa completo de preguntas se usa como referencia y no como obligación
* si los segmentos recomendados reducen ceremonia
* si el front-matter ayuda o estorba la autoría manual
* si los documentos se mantienen vivos durante evolución real
* si los documents evitan duplicación con Support Notes, Nexus o Continuity Paths

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde una necesidad documental concreta deba materializarse con bajo costo.

Posibles escenarios:

* documentar un contexto doméstico en Domus Orbis
* preservar vocabulario de dominio surgido desde clasificación de productos
* describir comportamiento esperado de una lista mensual de compra
* registrar decisiones de diseño documental
* documentar estructura de un artifact sin explicar implementación
* capturar feedback o actualización de alcance en una iteración

## Riesgos metodológicos

### Riesgo de confundir documento con plantilla

El tipo documental define una pregunta principal, no una estructura rígida de secciones.

### Riesgo de usar el mapa Full como obligación

El mapa completo de preguntas debe servir como espacio de investigación, no como artifact final obligatorio.

### Riesgo de crear documentos por taxonomía

No debe crearse un Document artifact solo porque existe un tipo disponible.

### Riesgo de ignorar soluciones más pequeñas

A veces una Support Note, referencia o comentario puede preservar suficiente intención.

## Relación con Docs Standard

Esta pregunta puede afectar:

* definición de Document artifacts
* catálogo inicial de documentos
* reglas de pregunta principal
* diagramas de ramificación
* selección de segmentos recomendados
* relación entre front-matter y cuerpo
* regla de no duplicar fuentes de verdad
* futuros templates
* validación de Tooling

## Límite actual

Esta pregunta no asume que los Document artifacts funcionan.

Solo propone investigarlos como mecanismo candidato para preservar conocimiento mediante preguntas documentales principales.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.
