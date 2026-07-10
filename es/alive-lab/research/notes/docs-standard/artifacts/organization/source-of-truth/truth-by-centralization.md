# Fuente de verdad centralizada

## Propósito

Este documento define el modelo de fuente de verdad centralizada.

Este modelo ocurre cuando los artifacts documentales viven en un lugar canónico común y las organizaciones documentales los referencian mediante índices, diagramas, metadata, Navigation Documents o proyecciones navegables.

Su objetivo es separar claramente:

* dónde vive el contenido canónico
* cómo se agrupan artifacts
* cómo se recorren desde distintas perspectivas

## Definición

La fuente de verdad centralizada es un modelo donde el contenido principal de los artifacts vive en una ubicación común o canónica, independiente de las organizaciones documentales que los referencian.

En este modelo, las organizaciones documentales no poseen necesariamente los artifacts.

Los ordenan mediante referencias.

Por ejemplo:

```text
artifacts/
  context.vslices-tooling.md
  scope.vslices-tooling.md
  viability.technical.vslices-tooling.md
  decision.template-language.md
  support-note.template-validation-result.md

organizations/
  initiative.vslices-tooling.md
  project.vslices-tooling-cli.md
  release.v0.1.md
```

En este caso, los documentos viven en `artifacts/`.

Las organizaciones viven en `organizations/` y referencian los artifacts relevantes.

## Qué pretende resolver

Este modelo ayuda cuando un mismo artifact puede aparecer en múltiples organizaciones documentales.

Por ejemplo, un Scope Document puede ser relevante para:

* una iniciativa de software
* una iteración
* un milestone
* un release
* una colección navegable
* un continuity path

En vez de copiar el documento en cada organización, se mantiene una sola fuente de verdad y se proyecta desde distintas vistas.

## Cómo se ve

Una fuente centralizada puede tener artifacts nombrados de forma estable.

```text
artifacts/
  context.docs-standard-organizations.md
  scope.docs-standard-organizations.md
  decision.source-of-truth-model.md
  update.organization-documents.md
```

Una organización puede referenciarlos mediante una proyección navegable.

```text
organizations/
  docs-standard-organizations.navigation.md
```

La proyección puede mostrarse con un TreeView.

```mermaid
tree
  "Organizaciones documentales"
    "Contexto"
      "context.docs-standard-organizations.md"
    "Alcance"
      "scope.docs-standard-organizations.md"
    "Decisiones"
      "decision.source-of-truth-model.md"
    "Actualizaciones"
      "update.organization-documents.md"
```

Este TreeView no contiene el conocimiento principal.

Solo muestra cómo recorrer artifacts existentes.

## Ventajas

* Reduce duplicación de contenido.
* Permite que un artifact aparezca en múltiples organizaciones.
* Separa fuente de verdad de navegación.
* Facilita proyecciones por iniciativa, proyecto, dominio, release o colección.
* Favorece nombres e identidades documentales estables.
* Puede facilitar tooling futuro.
* Permite generar índices, mapas o TreeViews desde metadata o referencias.
* Reduce el riesgo de que una carpeta se convierta en la única forma de entender el sistema documental.

## Desventajas

* Puede sentirse menos natural para navegación manual.
* Requiere nombres claros o identificadores estables.
* Puede volverse demasiado abstracto si todo queda plano.
* Necesita buenos índices o Navigation Documents para ser recorrible.
* Puede dificultar encontrar artifacts si no existe una estrategia de búsqueda.
* Puede empujar prematuramente hacia tooling.
* Puede separar demasiado el artifact de su contexto natural.

## Riesgos

| Riesgo                                                | Consecuencia                                                         |
| ----------------------------------------------------- | -------------------------------------------------------------------- |
| Crear una bodega documental plana                     | Los artifacts existen, pero nadie sabe cómo recorrerlos              |
| Depender demasiado de naming perfecto                 | Cualquier inconsistencia vuelve difícil encontrar documentos         |
| Reemplazar navegación humana por estructura abstracta | El sistema documental se vuelve correcto pero poco usable            |
| Forzar centralización antes de necesitarla            | Se agrega complejidad antes de que exista un problema real           |
| Confundir referencia con posesión                     | Una organización parece contener artifacts que solo está proyectando |
| Duplicar contenido en proyecciones                    | La proyección empieza a competir con la fuente de verdad             |

## Relación con proyecciones navegables

Este modelo funciona especialmente bien con proyecciones navegables.

Una misma fuente de verdad puede aparecer en distintas vistas.

```mermaid
tree
  "Iniciativa de software"
    "Alcance"
      "scope.docs-standard-organizations.md"
    "Decisión"
      "decision.source-of-truth-model.md"
  "Release v0.1"
    "Alcance"
      "scope.docs-standard-organizations.md"
    "Actualización"
      "update.organization-documents.md"
```

En este ejemplo, `scope.docs-standard-organizations.md` aparece en más de una organización.

Pero el contenido canónico sigue viviendo en un solo artifact.

## Relación con Navigation Documents

Cuando se usa una fuente de verdad centralizada, los Navigation Documents se vuelven especialmente importantes.

La centralización responde:

> ¿Dónde vive el contenido canónico?

Pero no responde por sí sola:

> ¿Por dónde conviene empezar?
> ¿Qué artifacts son principales?
> ¿Qué artifacts son auxiliares?
> ¿Qué recorrido preserva mejor continuidad?

Eso pertenece al Navigation Document.

Una fuente centralizada sin navegación puede ser correcta, pero difícil de usar.

## Relación con metadata

La fuente de verdad centralizada puede apoyarse en metadata para permitir proyecciones.

Por ejemplo, un artifact podría declarar o derivar:

* tipo documental
* scope
* target
* estado
* relaciones
* organizaciones sugeridas
* continuity paths asociados

Esto puede permitir que tooling futuro genere índices o TreeViews.

Sin embargo, esta metadata no debería ser obligatoria al inicio si agrega ceremonia innecesaria.

## Límites del modelo

Este modelo no debería convertirse en una obligación para todos los proyectos.

No todos los equipos necesitan una zona centralizada de artifacts.

No todos los sistemas documentales tienen suficiente volumen o transversalidad para justificarla.

Si una organización física simple preserva suficiente claridad, centralizar puede ser sobreingeniería.

## Cuándo puede ser suficiente

Este modelo puede ser suficiente cuando:

* existen muchas vistas transversales
* varios artifacts participan en múltiples organizaciones
* se quiere evitar duplicación
* se espera generar navegación desde referencias o metadata
* los nombres documentales ya son relativamente estables
* el equipo necesita proyectar la misma fuente desde distintas perspectivas

## Reglas recomendadas

* Mantener una única fuente de verdad por artifact.
* Usar proyecciones para mostrar organizaciones.
* Evitar copiar contenido canónico dentro de las proyecciones.
* Usar nombres estables o identificadores claros.
* Acompañar la centralización con Navigation Documents o índices.
* No centralizar solo por elegancia.
* No exigir tooling antes de que exista una necesidad real.
* Mantener las proyecciones legibles para humanos.

## Anti-patrón

Este modelo se usa mal cuando todos los artifacts se mueven a una zona común, pero no existe ninguna forma clara de recorrerlos.

El resultado es una bodega documental:

```text
artifacts/
  doc-001.md
  doc-002.md
  doc-003.md
  doc-004.md
```

Sin navegación, sin propósito visible y sin relaciones claras.

Centralizar sin navegación no preserva continuidad.

Solo cambia el lugar donde se pierde.

## Regla de cierre

La fuente de verdad centralizada favorece proyecciones navegables y reduce duplicación.

Es útil cuando los artifacts necesitan ser recorridos desde varias organizaciones.

Debe evitar convertirse en una bodega abstracta de documentos sin recorridos humanos claros.
