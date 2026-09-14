---
type: research-question
state: candidate
code: RQ-005

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

# RQ-005 — Organizaciones Documentales

## Pregunta

¿En qué condiciones separar fuente de verdad, organización documental, proyección navegable y navegación ayuda a preservar continuidad sin duplicar contenido ni imponer una estructura física única?

## Estado

candidate

## Origen

Esta pregunta surge desde [RN-0002 — VSlices Docs Standard como superficie de continuidad documental](../notes/RN-0001-superficies-continuidad-vslices.md).

Docs Standard propone separar conceptos que suelen mezclarse cuando se organiza documentación:

* fuente de verdad documental
* organización documental
* proyección navegable
* Navigation Document

La idea aparece como respuesta candidata a un problema frecuente: los equipos suelen confundir dónde vive un documento con cómo se ordena, cómo se muestra y cómo se recorre.

## Problema observado

La documentación puede perder continuidad cuando su organización depende exclusivamente de carpetas físicas o índices manuales.

Un mismo artifact puede ser relevante para varias perspectivas:

* una capability
* una iniciativa de software
* un proyecto
* una release
* una decisión
* un Continuity Path
* un Nexus
* un caso de investigación
* una evolución de alcance

Si se copia el artifact para cada organización, se duplican fuentes de verdad.

Si se deja en un solo lugar sin proyecciones, puede perder visibilidad desde otras perspectivas.

## Hipótesis inicial

Separar fuente de verdad, organización documental, proyección navegable y navegación podría preservar continuidad al permitir que un artifact mantenga contenido canónico único y participe en múltiples recorridos.

Su valor estaría en hacer navegable el conocimiento sin mover ni duplicar artifacts.

Su riesgo estaría en crear proyecciones que terminen compitiendo con la fuente de verdad o en imponer una arquitectura documental demasiado compleja.

## Qué busca observar esta pregunta

Esta pregunta busca observar si la separación entre estos conceptos ayuda a:

* mantener una fuente canónica clara
* organizar artifacts desde distintas perspectivas
* mostrar recorridos sin duplicar contenido
* hacer visible conocimiento relacionado
* evitar estructuras físicas rígidas
* permitir participación múltiple de un artifact
* mejorar navegación documental
* conectar Docs Standard con Surreal Atlas
* facilitar proyecciones manuales o asistidas por tooling

También busca observar cuándo esta separación agrega complejidad innecesaria.

## Mecanismos candidatos

Los mecanismos candidatos son:

### Fuente de verdad documental

Lugar canónico donde se mantiene el contenido vigente de un artifact.

### Organización documental

Criterio conceptual para ordenar artifacts.

Puede ordenar por:

* producto
* proyecto
* iteración
* etapa
* concepto
* dominio
* capability
* servicio
* release
* estudio
* experimento
* estado documental
* colección navegable

### Proyección navegable

Representación concreta de una organización mediante referencias.

Puede materializarse como:

* carpetas
* índices
* tablas
* TreeView
* enlaces
* metadata procesada
* Navigation Documents
* visualizaciones

### Navigation Document

Document artifact que explica cómo recorrer una organización, proyección o colección.

## Evidencia inicial disponible

La evidencia inicial es conceptual.

Proviene de:

* [RQ-001](../questions/rq-001-problema-fundacional-vslices.md)
* [RN-0001](../notes/RN-0001-superficies-continuidad-vslices.md)
* [RN-0002](../notes/RN-0002-vslices-docs-standard.md)
* el modelo candidato de Docs Standard
* el documento candidato sobre fuente de verdad y proyecciones navegables
* la necesidad de Surreal Atlas de mostrar relaciones sin duplicar documentos
* la regla candidata de que una proyección no debe competir con la fuente de verdad

## Evidencia faltante

Todavía falta observar:

* si esta separación es entendible por usuarios reales
* si reduce duplicación documental
* si mejora navegación
* si permite múltiples perspectivas sin perder fuente canónica
* si Navigation Document aporta guía real
* si una proyección puede mantenerse manualmente
* si Surreal Atlas puede materializar proyecciones sin absorber la responsabilidad del contenido
* si la separación sigue siendo útil en proyectos pequeños
* si tooling simplifica o complica la organización

## Posibles casos de estudio

Esta pregunta puede observarse en casos donde un mismo artifact necesite aparecer en más de una organización.

Posibles escenarios:

* artifacts de Domus Orbis organizados por dominio, iteración y capability
* documentos de Surreal Atlas proyectados como grafo, TreeView o colección navegable
* una decisión que participa en un Continuity Path, un Nexus y una iniciativa
* una release que referencia artifacts cuya fuente de verdad vive en otra carpeta
* una navegación documental que necesita orientar lectura sin copiar contenido

## Riesgos metodológicos

### Riesgo de duplicar contenido mediante proyecciones

Si una proyección repite contenido canónico, deja de orientar y se convierte en segunda fuente de verdad.

### Riesgo de imponer estructura física

Docs Standard no debería forzar una arquitectura universal de carpetas.

### Riesgo de confundir navegación con continuidad

Una proyección navegable puede mejorar exploración sin preservar intención.

### Riesgo de depender demasiado de Surreal Atlas

Surreal Atlas puede ayudar a visualizar organizaciones, pero no debe ser necesario para que el concepto tenga sentido documental.

## Relación con Docs Standard

Esta pregunta puede afectar:

* reglas de organización documental
* definición de fuente de verdad
* definición de proyección navegable
* definición de Navigation Document
* relación con Continuity Paths
* relación con Nexus
* criterios de no duplicación
* futura integración con Surreal Atlas
* futura generación por Tooling

## Límite actual

Esta pregunta no asume que las organizaciones documentales preservan continuidad.

Solo propone investigar si separar fuente de verdad, organización, proyección y navegación ayuda a mantener conocimiento navegable sin duplicación.

Mientras no existan casos analizados, su estado debe mantenerse como `candidate`.
