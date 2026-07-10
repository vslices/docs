# Fuentes de verdad y proyecciones navegables

## Propósito

Este documento define los conceptos usados para separar:

* dónde vive el contenido canónico de un artifact
* según qué criterio se ordenan artifacts
* cómo se muestra ese orden sin mover ni duplicar contenido
* cómo se explica un recorrido recomendado

Su objetivo es evitar que una organización documental se confunda con una estructura obligatoria de carpetas.

VSlices Docs Standard no impone una arquitectura física universal.

Define criterios para preservar continuidad, reducir duplicación y mantener los artifacts navegables con baja ceremonia.

## Fuente de verdad documental

Una fuente de verdad documental es el lugar canónico donde se mantiene el contenido vigente de un artifact.

Responde:

> ¿Dónde se mantiene el contenido que debe considerarse canónico?

Un artifact puede aparecer en múltiples organizaciones o proyecciones, pero debería tener una fuente de verdad identificable.

La fuente de verdad puede determinarse mediante:

* ubicación física
* pertenencia primaria
* convención de nombres
* metadata
* almacenamiento centralizado
* decisión explícita del equipo

VSlices Docs Standard no exige una estrategia única.

La regla importante es que podamos identificar dónde debe mantenerse el contenido.

## Organización documental

Una organización documental es un criterio para ordenar artifacts.

Responde:

> ¿Según qué perspectiva o criterio se relacionan estos artifacts?

Puede ordenar según:

* pertenencia
* secuencia
* estado
* etapa
* colección
* tema
* narrativa
* responsabilidad
* evolución

Una organización documental puede incluir artifacts que viven en distintas fuentes de verdad.

No necesita poseerlos físicamente.

Tampoco define por sí sola cómo se mostrará o recorrerá el orden resultante.

## Proyección navegable

Una proyección navegable es una representación concreta de una organización documental mediante referencias a artifacts existentes.

Responde:

> ¿Cómo mostramos esta organización sin mover ni duplicar sus artifacts?

Puede materializarse mediante:

* carpetas
* índices
* tablas de artifacts
* diagramas TreeView
* referencias
* enlaces
* metadata procesada
* Navigation Documents
* una combinación de estas formas

Una proyección navegable no debería copiar el contenido principal de los artifacts que referencia.

Su responsabilidad es mostrar:

* orden
* pertenencia
* relación
* ubicación
* recorrido posible

No reemplaza la fuente de verdad documental.

## Navigation Document

Un Navigation Document explica cómo recorrer una organización, proyección o colección de artifacts.

Responde:

> ¿Cómo conviene explorar este conjunto?

Puede explicar:

* por dónde comenzar
* qué artifacts son principales
* qué artifacts son auxiliares
* en qué orden conviene leerlos
* por qué aparecen en la proyección
* cuándo cambiar de perspectiva
* cuándo detener el recorrido

La proyección muestra una organización.

El Navigation Document explica cómo recorrerla.

## Diferencias principales

| Concepto                    | Pregunta                                          | Responsabilidad                           |
| --------------------------- | ------------------------------------------------- | ----------------------------------------- |
| Fuente de verdad documental | ¿Dónde vive el contenido canónico?                | Mantener el contenido vigente             |
| Organización documental     | ¿Según qué criterio ordenamos artifacts?          | Definir el orden conceptual               |
| Proyección navegable        | ¿Cómo mostramos esa organización?                 | Representar el orden mediante referencias |
| Navigation Document         | ¿Cómo exploramos esta organización?               | Explicar el recorrido recomendado         |
| Continuity Path             | ¿Cómo preservamos continuidad entre perspectivas? | Conectar y orientar continuidad           |
| Nexus                       | ¿Qué artifacts explican juntos este elemento?     | Declarar composición                      |

## Ejemplo

Un Scope Document puede tener como fuente de verdad:

```text
initiatives/
  monthly-shopping/
    scope.md
```

El mismo artifact puede participar en:

* una organización por iniciativa
* una organización por iteración
* una organización por release
* una colección de cambios de alcance

Una proyección por release podría mostrarlo así:

```text
releases/
  v0.1/
    navigation.md
    initiative-scope -> initiatives/monthly-shopping/scope.md
```

La proyección referencia el Scope Document.

No crea una segunda copia de su contenido.

## Participación múltiple

Un artifact puede participar en varias organizaciones al mismo tiempo.

Por ejemplo, un Decision Record puede ser relevante para:

* una capability
* una iniciativa de software
* un proyecto
* una release
* un Continuity Path de Evolution
* un Nexus

Esta participación múltiple no implica múltiples fuentes de verdad.

Cada organización ofrece una perspectiva distinta sobre el mismo artifact canónico.

## Regla semántica

VSlices Docs Standard mantiene esta separación:

* Los Documents explican.
* Las Support Notes apoyan, registran o referencian.
* Los Nexus componen.
* Los Continuity Paths conectan y orientan continuidad.
* Los diagramas muestran.
* Los mockups representan.
* Las organizaciones documentales ordenan.
* Las proyecciones navegables representan organizaciones.
* Las fuentes de verdad mantienen contenido canónico.

## Principio de no duplicación

Una proyección navegable puede incluir:

* nombre del artifact
* tipo
* estado
* propósito breve
* referencia
* razón de aparición
* rol dentro de la organización
* orden recomendado

No debería repetir el contenido que pertenece al artifact canónico.

Una organización o proyección deja de cumplir su responsabilidad cuando comienza a competir con la fuente de verdad.

## Libertad de organización

Un equipo puede organizar sus artifacts de la forma que mejor preserve continuidad en su contexto.

VSlices Docs Standard no obliga a usar:

* una estructura específica de carpetas
* un índice central
* una organización única
* una proyección generada automáticamente
* una relación uno a uno entre ubicación y pertenencia

La solución más pequeña que permita identificar, mantener y recorrer los artifacts es suficiente.

## Relación con Tooling

Las organizaciones y proyecciones pueden crearse manualmente.

VSlices Tooling podrá ayudar a generarlas desde:

* identidad de artifacts
* metadata
* referencias
* relaciones
* estados documentales
* composición de Nexus
* conexiones de Continuity Paths
* convenciones de ubicación

Tooling no debería definir por sí solo qué organización es correcta.

Debe materializar o validar una intención documental ya definida.

## Regla de cierre

Una fuente de verdad mantiene contenido.

Una organización documental define un criterio de orden.

Una proyección navegable muestra ese orden.

Un Navigation Document explica cómo recorrerlo.

Si una proyección duplica el contenido canónico, deja de orientar y comienza a crear una segunda fuente de verdad.
