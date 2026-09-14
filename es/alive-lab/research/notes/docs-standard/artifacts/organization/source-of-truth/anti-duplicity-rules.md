# Reglas anti-duplicación documental

## Propósito

Este documento define reglas para evitar duplicación de contenido entre fuentes de verdad documentales, organizaciones documentales y proyecciones navegables.

Su objetivo es preservar claridad sobre:

* dónde vive el contenido canónico
* qué artifacts pueden ser referenciados desde varias organizaciones
* qué puede incluir una proyección navegable
* qué debería evitarse para no crear fuentes de verdad competidoras

VSlices Docs Standard busca permitir múltiples recorridos documentales sin multiplicar copias del mismo conocimiento.

## Problema

Un artifact puede ser relevante para varias organizaciones documentales.

Por ejemplo, un Documento de Alcance puede aparecer en:

* una iniciativa de software
* una iteración
* un milestone
* una colección navegable
* un continuity path

El riesgo aparece cuando cada organización copia el contenido del artifact en vez de referenciar su fuente de verdad.

Eso produce:

* versiones divergentes
* pérdida de autoridad documental
* navegación confusa
* actualizaciones incompletas
* esfuerzo de mantenimiento innecesario

## Regla principal

Un artifact puede aparecer en múltiples organizaciones documentales, pero su contenido principal debería mantenerse en una fuente de verdad clara.

Una organización documental puede ordenar artifacts.

Una proyección navegable puede referenciarlos.

Ninguna de las dos debería duplicar el contenido canónico del artifact.

## Fuente de verdad única o identificable

Cada artifact debería tener una fuente de verdad única o claramente identificable.

Esto no significa que todos los artifacts deban vivir en una única carpeta central.

Significa que debe ser posible responder:

> ¿Dónde se mantiene el contenido vigente de este artifact?

La respuesta puede depender de:

* ubicación física
* pertenencia primaria
* nombre estable
* metadata
* referencia explícita
* decisión documental

Lo importante es evitar que varias copias parezcan igualmente oficiales.

## Qué puede incluir una proyección navegable

Una proyección navegable puede incluir información mínima para orientar el recorrido.

Puede incluir:

* nombre del artifact
* tipo de artifact
* estado documental
* referencia o link
* propósito breve
* razón de aparición en la organización
* orden recomendado de lectura
* agrupación conceptual
* relación con otros artifacts
* señales de navegación

Ejemplo:

```mermaid
tree
  "Iniciativa de software: VSlices Tooling"
    "Contexto"
      "context.vslices-tooling.md"
    "Alcance"
      "scope.vslices-tooling.md"
    "Decisiones"
      "decision.template-language.md"
```

La proyección muestra orden.

No reemplaza los documentos referenciados.

## Qué no debería incluir una proyección navegable

Una proyección navegable no debería copiar el contenido principal de los artifacts que referencia.

Debería evitar:

* repetir secciones completas de documentos
* copiar decisiones completas
* duplicar reglas de dominio
* reescribir comportamiento esperado
* mantener versiones paralelas de alcance
* copiar resultados o validaciones completas
* explicar en detalle lo que ya explica otro artifact
* convertirse en documento canónico alternativo

Si una proyección necesita explicar demasiado, probablemente debería apoyarse en un Navigation Document o referenciar mejor los artifacts existentes.

## Diferencia entre referencia, resumen y duplicación

| Forma              | Uso esperado                                   | Riesgo   |
| ------------------ | ---------------------------------------------- | -------- |
| Referencia         | Apuntar al artifact canónico                   | Bajo     |
| Propósito breve    | Explicar por qué aparece en el recorrido       | Bajo     |
| Resumen contextual | Orientar sin reemplazar el artifact            | Medio    |
| Extracto parcial   | Citar una parte específica con intención clara | Medio    |
| Copia de contenido | Repetir contenido principal del artifact       | Alto     |
| Versión reescrita  | Mantener una variante del contenido original   | Muy alto |

La referencia es segura.

El resumen puede ser útil si no compite con el artifact.

La copia crea riesgo de divergencia.

## Regla sobre resúmenes

Un resumen dentro de una organización o proyección debería responder:

> ¿Por qué este artifact importa en este recorrido?

No debería responder:

> ¿Qué dice completamente este artifact?

Si el lector necesita el contenido completo, debería ir a la fuente de verdad.

## Regla sobre extractos

Un extracto puede usarse cuando una parte específica del artifact es necesaria para orientar el recorrido.

Pero debería cumplir estas condiciones:

* indicar claramente que es un extracto
* mantener referencia al artifact original
* no reemplazar el contenido completo
* evitar reinterpretar el texto como nueva fuente de verdad
* actualizarse o eliminarse si deja de ser útil

Si el extracto empieza a requerir mantenimiento propio, probablemente está duplicando contenido.

## Regla sobre cambios

Cuando un artifact cambia, las proyecciones que lo referencian no deberían necesitar actualizar contenido duplicado.

Idealmente, solo deberían actualizar:

* referencia
* estado
* orden de lectura
* propósito breve
* relación con otros artifacts

Si un cambio obliga a editar muchas proyecciones con contenido repetido, hay duplicación excesiva.

## Regla sobre artifacts transversales

Cuando un artifact pertenece a varias organizaciones, no debería copiarse en cada una.

Debería elegirse una fuente de verdad y referenciarlo desde las demás.

Ejemplo:

```text
domains/
  docs-standard/
    vocabulary.md

initiatives/
  organization-documents/
    navigation.md
    organization.tree.md
```

La iniciativa puede referenciar `domains/docs-standard/vocabulary.md`.

No necesita copiarlo.

## Regla sobre organizaciones físicas

Una organización física puede contener fuentes de verdad.

Pero cuando un artifact físico es relevante para otra organización, esa otra organización debería referenciarlo.

No debería copiarlo salvo que exista una razón explícita para crear un artifact distinto.

Si se crea un artifact distinto, debería tener identidad e intención propia.

## Regla sobre proyecciones múltiples

Un mismo artifact puede aparecer en varias proyecciones navegables.

Eso no implica duplicación si todas las proyecciones apuntan a la misma fuente de verdad.

Ejemplo:

```mermaid
tree
  "Iteración 1"
    "Alcance"
      "scope.vslices-tooling.md"
  "Release v0.1"
    "Alcance"
      "scope.vslices-tooling.md"
```

El mismo artifact aparece en dos recorridos.

El contenido sigue viviendo en un solo lugar.

## Señales de duplicación peligrosa

Puede existir duplicación peligrosa cuando:

* el mismo contenido aparece copiado en varios lugares
* no está claro cuál versión está vigente
* una organización explica más que los artifacts que referencia
* una actualización exige modificar muchas copias
* dos documentos responden la misma pregunta principal sobre el mismo tema
* una proyección contiene decisiones completas
* un índice empieza a tener contenido sustantivo propio
* un resumen cambia el significado del artifact original
* un artifact transversal fue copiado porque no se sabía dónde ponerlo

## Duplicación aceptable

No toda repetición es mala.

Puede ser aceptable repetir:

* nombres de artifacts
* títulos
* IDs
* estados
* links
* una frase de propósito
* etiquetas de navegación
* criterios breves de recorrido
* advertencias de lectura
* referencias cruzadas

Esta repetición ayuda a navegar.

No compite con la fuente de verdad.

## Duplicación no aceptable

Debería evitarse repetir:

* contenido completo de documentos
* reglas de dominio completas
* decisiones completas
* comportamiento esperado completo
* criterios de alcance completos
* evaluaciones de viabilidad completas
* resultados completos
* validaciones completas
* feedback completo
* segmentos enteros que deban mantenerse sincronizados

Esta repetición compite con la fuente de verdad y aumenta mantenimiento accidental.

## Relación con documentos

Los documentos explican conocimiento desde una pregunta principal.

Si una organización necesita explicar el contexto, alcance, comportamiento, consistencia, decisión o viabilidad, debería referenciar el documento correspondiente.

La organización no debería absorber esa explicación.

## Relación con continuity paths

Los continuity paths conectan conceptos entre perspectivas.

Si una organización necesita mostrar continuidad entre negocio, dominio, software, producto, servicio, evolución o impacto, debería referenciar el path correspondiente.

La organización no debería convertirse en matriz de trazabilidad completa.

## Relación con Navigation Documents

Un Navigation Document puede explicar cómo recorrer una organización.

Puede incluir más orientación que una proyección TreeView.

Aun así, debería evitar duplicar el contenido principal de los artifacts recorridos.

Su responsabilidad es orientar la lectura, no reemplazar los documentos.

## Relación con Update Documents

Un Update Document puede indicar qué debe actualizarse en un artifact.

No debería usarse para mantener copias paralelas de contenido.

Cuando una actualización se aplica, el cambio debería terminar en la fuente de verdad correspondiente.

El Update Document preserva la intención y momento de aplicación.

No reemplaza el artifact actualizado.

## Riesgos principales

| Riesgo                                         | Consecuencia                                  |
| ---------------------------------------------- | --------------------------------------------- |
| Copiar contenido en varias organizaciones      | Aparecen fuentes de verdad competidoras       |
| Usar proyecciones como documentos explicativos | Se rompe la separación semántica del estándar |
| No identificar la fuente de verdad             | Nadie sabe qué versión mantener               |
| Crear resúmenes demasiado largos               | El resumen empieza a competir con el artifact |
| Mantener extractos sin control                 | Se desactualizan fragmentos importantes       |
| Resolver pertenencia copiando archivos         | Se multiplica mantenimiento accidental        |
| Convertir índices en documentos sustantivos    | Se mezclan navegación y explicación           |

## Reglas recomendadas

* Mantener una fuente de verdad clara por artifact.
* Referenciar artifacts en vez de copiarlos.
* Usar proyecciones para mostrar organización, no para explicar contenido completo.
* Usar Navigation Documents para orientar recorridos complejos.
* Mantener resúmenes breves y orientados al recorrido.
* Evitar extractos salvo que tengan una intención clara.
* No duplicar decisiones, reglas, alcance, comportamiento o validaciones completas.
* Revisar duplicación cuando una actualización exige cambios en varios lugares.
* Crear un artifact nuevo solo si responde una pregunta o intención distinta.
* Preferir referencias explícitas antes que copias convenientes.

## Anti-patrón

Una organización documental se usa mal cuando se convierte en una segunda versión de los documentos que ordena.

Ejemplo problemático:

```text
initiative.vslices-tooling.md
  Contexto completo copiado desde context.vslices-tooling.md
  Alcance completo copiado desde scope.vslices-tooling.md
  Decisiones copiadas desde varios Decision Records
```

En ese caso, la organización dejó de ordenar.

Ahora compite con las fuentes de verdad.

## Regla de cierre

Una organización documental puede hacer visible un artifact en muchos recorridos.

Eso no significa que deba copiar su contenido.

La continuidad se preserva mejor cuando cada artifact tiene una fuente de verdad clara y cada proyección sabe que su responsabilidad es ordenar, no reemplazar.
