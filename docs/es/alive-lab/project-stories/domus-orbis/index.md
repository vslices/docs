# Domus Orbis

*Documentar el hogar como sistema vivo*

## Qué es Domus Orbis

**Domus Orbis** es un proyecto experimental orientado a reducir fricción en la gestión cotidiana del hogar.

El proyecto parte de una idea simple:

> El hogar no es solamente un lugar donde ocurren tareas. Es un sistema vivo compuesto por decisiones, compras, pagos, consumo, rutinas, olvidos, prioridades y responsabilidades que deben sostenerse en el tiempo.

Domus Orbis explora cómo el software puede ayudar a preservar claridad doméstica sin convertir el hogar en una fuente adicional de ruido, ansiedad o dependencia tecnológica.

## Por qué está en Alive Lab

Domus Orbis forma parte de **Alive Lab** porque funciona como un laboratorio real para validar VSlices en un dominio cotidiano, no solamente técnico.

Este proyecto permite observar cómo VSlices Method, VSlices Docs Standard, VSlices Design y eventualmente VSlices Framework pueden ayudar a pasar desde una necesidad real hacia una solución pequeña, documentada, evolutiva y validable.

El objetivo no es demostrar una arquitectura ideal. El objetivo es observar qué documentación, decisiones, artifacts y límites aparecen cuando se intenta resolver un problema real con bajo nivel de ceremonia.

## Tipo de problema que representa

Domus Orbis representa problemas donde la dificultad no está necesariamente en la complejidad técnica, sino en la continuidad.

Ejemplos de tensiones propias del proyecto:

* compras que deben hacerse antes de que el dinero se disperse
* listas que se repiten, pero se reconstruyen manualmente
* tareas simples que fallan porque dependen de memoria, energía o foco
* procesos domésticos que parecen pequeños, pero generan estrés cuando no se sostienen
* información que existe en aplicaciones externas, pero no como intención propia del hogar

Estos problemas son útiles para VSlices porque obligan a separar con cuidado:

* necesidad real
* proceso actual
* solución pequeña
* artifact inicial
* mejora futura
* automatización prematura

## Qué queremos validar

Con Domus Orbis queremos validar cómo aplicar todas las metodologias que tenemos en VSlices Method.

En particular, nos interesa observar si la forma que ofrecemos, puede:

* preservar intención antes de construir una aplicación completa
* reducir fricción real sin automatizar todo el proceso
* evitar sobreingeniería
* producir documentación útil para retomar el trabajo después
* generar artifacts pequeños que puedan sobrevivir a futuras iteraciones
* adaptarse a la evolución del mismo producto sin cambiar escenacia

La hipótesis principal es que las metodologias deben poder adaptarse a las circunstancias y resolviendo los problemas que vayan saliendo del contexto cotidiano del día a día del hogar, sin necesitar resolver mediante un sistema completo, pero que eventualmente pueda llegar a serlo.

A la vez permite validar elementos como celulas paralelas, en un mismo contexto:

- Una que elabore mediante Slice-First soluciones practicas y utiles a dolores especificos
- Una que resuelva con Problem-First tareas que requieran más investigación, sin comprometer una solución eficiente
- Una que vaya descubriendo más elementos construya una base fuerte para un SAAS futuro mediante Context-first

## Productos de VSlices involucrados:

Este Project Story ha hecho uso de estos productos:

- __[VSlices Method](../../../products/method/index.md)__
    - Hizo uso de la guia de contexto de [Escenario "no digitalizado"](../../../products/method/context-guides/scenarios/non-digitalized-scenario.md) en:
        - un caso pequeño
        - un entorno más relajado

- __[VSlices Docs Standard](../../../products/docs-standard/index.md)__
    - Mostró cómo seleccionar documentos, nombrarlos según responsabilidad.
    - Ayudo a observar como los diagramas se relacionan con algunos documentos.

- __[VSlices Design](../../../products/design/index.md)__:
    - Hizo uso de analisis de necesidades, procesos, límites y evolución sin partir desde la solución técnica.
    - Ayudo a observar cómo emplear la metodología [Slice-First](../../../products/design/modalities/slice-first/index.md) en:
        - un caso pequeño
        - un entorno más relajado

- __[VSlices Framework](../../../products/framework/index.md)__:
    - Refuerzó la idea de documentación colocalizada con el proyecto para habilitar tooling futuro.

## Cómo leer este Project Story

Este Project Story no debe leerse como una receta universal.

Domus Orbis muestra cómo un proyecto real eligió documentos, artifacts y pasos según su propio alcance. Otro proyecto podría necesitar menos documentación, más documentación o documentos distintos.

La intención es mostrar una aplicación concreta de VSlices Method para extraer aprendizajes reutilizables.

## Estado

Este Project Story está en evolución.

La primera documentación se centra en Iteration 0 de Domus Orbis. Futuras iteraciones podrán mostrar cómo el artifact inicial se transforma en comportamiento estable, tooling, validación y posible integración con VSlices Framework.

