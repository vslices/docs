# Fuentes de verdad y proyecciones navegables

## Propósito

Este documento define conceptos base para entender cómo VSlices Docs Standard separa:

* dónde vive el contenido canónico de un artifact
* cómo se ordenan artifacts documentales
* cómo se pueden proyectar organizaciones navegables sin duplicar contenido

Su objetivo es evitar que una organización documental sea confundida con una estructura obligatoria de carpetas.

VSlices Docs Standard no impone una única forma física de organizar documentos.

Define criterios para preservar continuidad sin duplicar conocimiento ni agregar ceremonia innecesaria.

## Fuente de verdad documental

Una fuente de verdad documental es el artifact canónico donde se mantiene el contenido principal de un documento, diagrama, mockup, nota, decisión, continuity path u otro artifact documental.

La fuente de verdad responde:

> ¿Dónde se mantiene el contenido que debe considerarse vigente?

Un artifact puede aparecer referenciado desde varias organizaciones documentales, pero su contenido principal debería mantenerse en una fuente de verdad clara.

La fuente de verdad puede estar determinada por:

* una ubicación física
* una pertenencia principal
* una convención de nombres
* metadata
* una estructura centralizada
* una decisión explícita del equipo

VSlices Docs Standard no exige una estrategia única.

La regla importante es que debe ser posible identificar dónde vive el contenido canónico.

## Organización documental

Una organización documental es una estrategia para ordenar artifacts según pertenencia, secuencia, estado, etapa, colección o narrativa mayor.

La organización documental responde:

> ¿Cómo se agrupan o recorren estos artifacts?

Una organización documental puede ordenar artifacts sin poseerlos físicamente.

Puede materializarse como:

* carpetas
* índices
* tablas de artifacts
* metadata
* referencias
* diagramas TreeView
* documentos de navegación
* una combinación de las anteriores

La organización documental no explica el contenido detallado de los artifacts.

Solo ayuda a ubicarlos, agruparlos o recorrerlos.

## Proyección navegable

Una proyección navegable es una vista que representa una organización documental mediante referencias a artifacts existentes.

La proyección navegable responde:

> ¿Cómo mostramos una forma de recorrer artifacts sin moverlos ni duplicarlos?

Una proyección navegable puede usar:

* un diagrama TreeView
* un índice
* una tabla de lectura
* un Navigation Document
* referencias entre artifacts
* metadata procesada por tooling

Una proyección navegable no debería duplicar el contenido principal de los artifacts que referencia.

Su responsabilidad es mostrar orden, recorrido o pertenencia.

No reemplaza la fuente de verdad documental.

## Diferencia entre fuente de verdad y proyección

| Concepto                    | Pregunta                                         | Responsabilidad                                   |
| --------------------------- | ------------------------------------------------ | ------------------------------------------------- |
| Fuente de verdad documental | ¿Dónde vive el contenido canónico?               | Mantener el contenido principal del artifact      |
| Organización documental     | ¿Cómo agrupamos o recorremos artifacts?          | Ordenar artifacts según una perspectiva           |
| Proyección navegable        | ¿Cómo mostramos esa organización?                | Representar una organización mediante referencias |
| Navigation Document         | ¿Cómo exploramos esta organización?              | Explicar el recorrido recomendado                 |
| Continuity Path             | ¿Cómo se conecta un concepto entre perspectivas? | Conectar artifacts, conceptos y superficies       |

## Qué pretende VSlices Docs Standard

VSlices Docs Standard pretende preservar continuidad documental sin imponer una arquitectura única de carpetas.

Para eso distingue entre:

* el lugar donde vive un artifact
* las organizaciones desde las que puede ser recorrido
* las proyecciones que muestran esas organizaciones
* los documentos que explican el conocimiento
* los paths que conectan continuidad

Esta separación permite que un artifact pueda participar en más de una organización sin ser copiado.

Por ejemplo, un Documento de Alcance puede ser relevante para:

* una iniciativa de software
* una iteración
* un milestone
* una colección navegable
* un continuity path

Pero su contenido principal debería mantenerse en una fuente de verdad clara.

## Regla semántica base

VSlices Docs Standard mantiene esta separación:

* Los documentos explican.
* Los continuity paths conectan.
* Los diagramas muestran.
* Los mockups representan.
* La organización documental ordena.
* Las proyecciones navegables representan organizaciones mediante referencias.
* Las fuentes de verdad preservan contenido canónico.

## Principio de no duplicación

Una organización documental no debería copiar el contenido principal de los artifacts que ordena.

Puede incluir:

* nombre del artifact
* tipo de artifact
* estado
* propósito breve
* referencia o link
* razón de aparición en la organización
* orden recomendado de lectura

Pero no debería repetir el contenido que pertenece al artifact canónico.

## Libertad de organización

Un equipo puede organizar sus artifacts de la forma que mejor preserve continuidad en su contexto.

VSlices Docs Standard no impone una estructura física obligatoria.

Sus recomendaciones buscan ayudar a decidir:

* dónde mantener fuentes de verdad
* cómo evitar duplicación
* cómo crear proyecciones navegables
* cómo separar orden documental de contenido documental
* cómo mantener artifacts recorribles a medida que el sistema evoluciona

## Relación con tooling futuro

Las proyecciones navegables pueden ser creadas manualmente al inicio.

En el futuro, VSlices Tooling podría ayudar a generarlas desde:

* metadata
* referencias
* identificadores documentales
* relaciones entre artifacts
* estados documentales
* continuity paths

Esto no debe asumirse como requisito inicial.

La prioridad es preservar claridad documental antes de automatizarla.

## Regla de cierre

Una fuente de verdad mantiene contenido.

Una organización documental ordena artifacts.

Una proyección navegable muestra una organización.

Si una organización empieza a duplicar contenido, deja de ordenar y comienza a competir con los documentos que debería referenciar.
