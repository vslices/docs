---
type: research-question
state: candidate
code: RQ-003

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
* VSlices Tooling
* Surreal Atlas
---

# RQ-003 — Nexos Documentales

## Pregunta

¿En qué condiciones los Nexos Documentales ayudan a preservar continuidad alrededor de elementos compuestos sin duplicar contenido ni crear documentos monolíticos?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0002-vslices-docs-standard.md).

Docs Standard propone los Nexus como artifacts que componen otros artifacts alrededor de un elemento compuesto.

La idea aparece como respuesta candidata a un problema frecuente: algunos elementos relevantes no viven naturalmente en un solo documento, pero crear un documento gigante puede mezclar responsabilidades y duplicar contenido.

## Problema observado

En software, algunos elementos importantes aparecen distribuidos en varios artifacts.

Por ejemplo, una capacidad puede requerir entender:

* qué cubre
* qué debe ocurrir
* cómo se organiza
* qué reglas respeta
* si es viable
* qué decisiones la delimitan
* qué riesgos o validaciones existen
* qué feedback la cambió o confirmó

Un servicio consumible puede requerir entender:

* dónde vive su especificación externa
* qué capacidad ofrece
* cómo debe consumirse
* qué comportamiento se espera
* qué reglas o garantías respeta
* qué errores comunica
* qué decisiones explican su forma de consumo
* qué conceptos de dominio expone

Si todo esto se mezcla en un documento monolítico, se duplican responsabilidades.

Si todo queda separado sin composición visible, se fragmenta la comprensión.

## Hipótesis inicial

Los Nexos Documentales podrían preservar continuidad cuando un elemento compuesto necesita varios artifacts para entenderse y la composición reduce fragmentación real.

Su valor estaría en declarar qué artifacts explican juntos un elemento y qué rol cumple cada uno.

Su riesgo estaría en agregar una capa documental innecesaria cuando un solo documento o una referencia simple ya preserva suficiente intención.

## Qué busca observar esta pregunta

Esta pregunta busca observar si los Nexus ayudan a:

* reducir fragmentación entre artifacts relacionados
* evitar documentos monolíticos
* orientar lectura de elementos compuestos
* declarar roles de composición
* conectar artifacts sin duplicar contenido
* hacer visible qué falta para entender una capability o servicio
* permitir composición parcial sin exigir completitud

También busca observar cuándo un Nexus no aporta valor.

## Mecanismo candidato

El mecanismo candidato es el **Nexus artifact**.

Nexus candidatos iniciales:

* Capability Nexus
* Service Consumption Nexus

Un Nexus:

* compone artifacts alrededor de un target compuesto
* declara artifacts participantes
* declara roles de composición
* no reemplaza los artifacts compuestos
* no duplica su contenido
* puede partir incompleto
* no obliga a crear todos los artifacts posibles

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* el modelo candidato de Docs Standard
* la definición candidata de Nexus artifacts
* los artifacts candidatos `Capability Nexus` y `Service Consumption Nexus`

## Evidencia faltante

Todavía falta observar:

* si un Nexus reduce fragmentación real
* si las personas entienden la diferencia entre Nexus, Document, Navigation Document y Continuity Path
* si un Nexus permite leer mejor una capacidad
* si un Nexus permite leer mejor el consumo de un servicio
* si la composición declarada es suficiente sin duplicar contenido
* si el Nexus puede mantenerse manualmente
* si el Nexus requiere tooling para ser útil
* si los roles de composición son comprensibles
* si el Nexus se usa solo cuando un documento simple no basta

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde un elemento compuesto aparezca distribuido entre varios artifacts.

Posibles escenarios:

* una capability de Domus Orbis que requiere scope, behavior, structure, consistency y decisions
* un servicio consumible con especificación externa y reglas de dominio no evidentes
* una feature que necesita articular comportamiento, testing, validación y feedback
* un conjunto de artifacts que queda fragmentado sin un punto de composición
* una visualización de Surreal Atlas que permite recorrer composición documental

## Riesgos metodológicos

### Riesgo de crear Nexus por estética

Un Nexus debe existir porque reduce fragmentación, no porque el modelo permite crearlo.

### Riesgo de convertir Nexus en documento monolítico

El Nexus compone artifacts.

No debe absorber el contenido de los artifacts compuestos.

### Riesgo de convertir todo concepto compuesto en Nexus

No toda capability, servicio, feature o cambio necesita un Nexus.

### Riesgo de depender demasiado de Tooling

Un Nexus debería tener valor documental entendible antes de automatizarlo.

## Relación con Docs Standard

Esta pregunta puede afectar:

* definición de Nexus artifacts
* roles de composición
* Capability Nexus
* Service Consumption Nexus
* reglas anti-monolito
* reglas para decidir cuándo no crear Nexus
* relación entre Nexus y Continuity Paths
* relación entre Nexus y Surreal Atlas
* futura generación o visualización por Tooling

## Límite actual

Esta pregunta no asume que los Nexus preservan continuidad.

Solo propone investigarlos como mecanismo candidato para componer artifacts relacionados sin duplicar contenido.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.
