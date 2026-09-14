# Fuente de verdad por organización física

## Propósito

Este documento define el modelo de fuente de verdad por organización física.

Este modelo ocurre cuando los artifacts viven físicamente dentro de la organización documental que los agrupa.

Su objetivo es ofrecer una forma simple y directa de mantener documentos cuando existe una organización dominante y no hay demasiadas vistas transversales.

## Definición

La fuente de verdad por organización física es un modelo donde el contenido canónico de un artifact vive dentro de la estructura física que representa su organización documental principal.

La ubicación física del artifact comunica su pertenencia principal.

Por ejemplo, si una iniciativa de software contiene sus documentos directamente, esos documentos pueden vivir dentro de la carpeta de la iniciativa.

```text
initiatives/
  vslices-tooling/
    context.md
    scope.md
    viability.md
    decisions/
      template-language.md
```

En este modelo, la organización documental y la ubicación física están fuertemente alineadas.

## Qué pretende resolver

Este modelo ayuda cuando se necesita una forma sencilla de responder:

> ¿Dónde vive este artifact?

También ayuda cuando la mayoría de los artifacts pertenecen claramente a una sola organización principal.

Reduce la necesidad inicial de índices, metadata avanzada o proyecciones navegables.

## Cómo se ve

Una organización física puede materializarse como carpetas, subcarpetas y archivos.

Ejemplo por iniciativa:

```text
initiatives/
  monthly-shopping-automation/
    navigation.md
    context.md
    scope.md
    viability.md
    decisions/
      initial-yaml-artifact.md
    support/
      first-real-use-result.md
```

Ejemplo por proyecto:

```text
projects/
  vslices-tooling-cli/
    navigation.md
    context.md
    structure.md
    decisions/
      template-loading.md
```

Estos ejemplos son materializaciones posibles.

No son estructuras obligatorias.

## Ventajas

* Es fácil de entender.
* Es cómoda para navegación manual.
* Requiere poca infraestructura.
* Funciona bien en proyectos pequeños o medianos.
* Hace visible la pertenencia principal de cada artifact.
* Reduce la necesidad inicial de tooling.
* Permite empezar rápido sin diseñar un sistema documental complejo.

## Desventajas

* Escala peor cuando un artifact pertenece a varias organizaciones.
* Puede incentivar duplicación si el mismo artifact parece necesario en más de un lugar.
* Puede acoplar demasiado la documentación a una única forma de recorrido.
* Reorganizar carpetas puede romper enlaces o referencias.
* Puede generar discusiones sobre dónde debería vivir un artifact transversal.
* Puede esconder relaciones que cruzan iniciativas, proyectos, dominios o releases.

## Riesgos

| Riesgo                                                      | Consecuencia                                                             |
| ----------------------------------------------------------- | ------------------------------------------------------------------------ |
| Confundir ubicación física con pertenencia conceptual única | Se asume que un artifact solo pertenece a la carpeta donde vive          |
| Duplicar artifacts en varias organizaciones                 | Aparecen múltiples fuentes de verdad para el mismo contenido             |
| Usar carpetas como única forma de navegación                | Se pierden recorridos transversales importantes                          |
| Reorganizar estructura sin preservar referencias            | Se rompen links, historia o continuidad                                  |
| Encerrar conocimiento transversal                           | Un documento útil para varias organizaciones queda escondido en una sola |

## Cuándo puede ser suficiente

Este modelo puede ser suficiente cuando:

* el volumen documental es bajo
* una organización domina claramente
* los artifacts tienen pertenencia principal evidente
* el equipo necesita navegación simple
* todavía no existen muchas relaciones transversales
* el costo de una estructura más flexible no se justifica

No requiere que el equipo renuncie a proyecciones navegables futuras.

Una organización física puede evolucionar hacia modelos más referenciales si el sistema documental crece.

## Relación con proyecciones navegables

Aunque el artifact viva dentro de una organización física, puede aparecer referenciado desde otras proyecciones.

Por ejemplo:

```text
initiatives/
  vslices-tooling/
    scope.md

releases/
  v0.1/
    navigation.md
```

El release puede referenciar `initiatives/vslices-tooling/scope.md` sin copiarlo.

En ese caso:

* la fuente de verdad vive en la iniciativa
* la proyección de release solo referencia el artifact
* el contenido no se duplica

## Límites del modelo

Este modelo no debería usarse para afirmar que un artifact solo pertenece conceptualmente a una organización.

La ubicación física indica dónde se mantiene el contenido.

No necesariamente indica todas las perspectivas desde las que ese artifact puede ser recorrido.

Si un artifact empieza a aparecer en muchas organizaciones, puede ser señal de que conviene usar proyecciones navegables o una fuente de verdad por pertenencia primaria.

## Reglas recomendadas

* Mantener una fuente de verdad clara por artifact.
* Evitar copiar el mismo contenido en varias carpetas.
* Usar referencias cuando un artifact sea útil desde otra organización.
* No convertir la carpeta en explicación del contenido.
* No asumir que la ubicación física reemplaza un Navigation Document.
* Mantener la estructura simple mientras sea suficiente.
* Evolucionar hacia modelos más flexibles solo cuando exista necesidad real.

## Anti-patrón

Este modelo se usa mal cuando se intenta resolver toda relación documental moviendo archivos entre carpetas.

Mover un artifact no debería ser la única forma de expresar que pertenece a otra organización.

Si el mismo artifact necesita aparecer en varios recorridos, es preferible referenciarlo desde proyecciones navegables.

## Regla de cierre

La fuente de verdad por organización física favorece simplicidad.

Es útil cuando una organización principal basta para mantener claridad.

Debe evitar convertirse en una prisión conceptual donde la carpeta define todas las pertenencias posibles del artifact.
