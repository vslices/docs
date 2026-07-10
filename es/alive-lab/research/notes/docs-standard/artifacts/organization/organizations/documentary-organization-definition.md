# Organización documental

## Propósito

Este documento define qué es una organización documental dentro de VSlices Docs Standard.

Su objetivo es separar la idea de organización documental de:

* una estructura obligatoria de carpetas
* una fuente de verdad documental
* una proyección navegable
* un documento explicativo
* un continuity path
* una matriz de trazabilidad
* una metodología de gestión

La organización documental existe para ordenar artifacts.

No existe para explicar todo el conocimiento que esos artifacts contienen.

## Definición

Una organización documental es una estrategia para ordenar artifacts documentales según un criterio de pertenencia, secuencia, estado, etapa, colección o narrativa mayor.

Responde:

> ¿Cómo se agrupan o recorren estos artifacts?

Una organización documental ayuda a ubicar, agrupar o recorrer artifacts sin imponer una estructura física obligatoria.

Puede existir como carpeta, índice, tabla, metadata, diagrama TreeView, Navigation Document, proyección navegable o combinación de varias formas.

## Responsabilidad

La responsabilidad de una organización documental es ordenar artifacts.

Puede ayudar a responder:

* dónde conviene ubicar un artifact
* desde qué conjunto puede recorrerse
* qué artifacts pertenecen a una misma agrupación
* qué artifacts deberían verse juntos
* qué recorrido documental puede preservar mejor continuidad
* qué artifacts forman parte de una narrativa mayor

Una organización documental no debería intentar explicar en detalle el contenido de los artifacts que ordena.

## Qué ordena

Una organización documental puede ordenar distintos tipos de artifacts, por ejemplo:

* documentos
* continuity paths
* diagramas
* mockups
* support notes
* decision records
* navigation documents
* update documents
* feedback documents
* proyecciones navegables
* referencias a artifacts externos

El criterio de organización depende del problema de orden documental que se quiere resolver.

## Criterios de organización

Una organización documental puede ordenar artifacts según distintos criterios.

| Criterio        | Pregunta                                                             |
| --------------- | -------------------------------------------------------------------- |
| Pertenencia     | ¿A qué conjunto pertenece este artifact?                             |
| Secuencia       | ¿En qué orden conviene recorrer estos artifacts?                     |
| Estado          | ¿Cuál es la vigencia o madurez de este artifact?                     |
| Etapa           | ¿En qué momento del trabajo apareció o se usa este artifact?         |
| Colección       | ¿Qué artifacts deben verse juntos aunque vivan en lugares distintos? |
| Narrativa mayor | ¿Qué historia, iniciativa, caso o recorrido agrupa estos artifacts?  |

Estos criterios pueden combinarse.

La combinación no obliga a crear carpetas específicas.

Puede materializarse mediante referencias, índices o proyecciones navegables.

## Formas de materialización

Una organización documental puede materializarse de distintas formas.

Puede ser:

* una estructura física de carpetas
* un índice Markdown
* una tabla de artifacts
* una convención de nombres
* un conjunto de referencias
* metadata procesable
* un diagrama TreeView
* un Navigation Document
* una proyección navegable generada manualmente
* una proyección navegable generada por tooling futuro

La forma elegida debe preservar continuidad sin agregar ceremonia innecesaria.

## Organización física

Una organización documental puede coincidir con una estructura de carpetas.

Ejemplo:

```text
initiatives/
  docs-standard-organizations/
    context.md
    scope.md
    decisions/
```

En este caso, la carpeta ayuda a ordenar artifacts físicamente.

Pero esta no es la única forma válida de organización.

## Organización referencial

Una organización documental también puede existir como una vista que referencia artifacts ubicados en otra parte.

Ejemplo:

```text
artifacts/
  context.docs-standard-organizations.md
  scope.docs-standard-organizations.md
  decision.source-of-truth-model.md

organizations/
  docs-standard-organizations.md
```

La organización no posee necesariamente los artifacts.

Solo los agrupa o presenta como parte de un recorrido.

## Proyección navegable

Una organización documental puede representarse mediante una proyección navegable.

Ejemplo:

```mermaid
tree
  "Organización documental: Docs Standard Organizations"
    "Contexto"
      "context.docs-standard-organizations.md"
    "Alcance"
      "scope.docs-standard-organizations.md"
    "Decisiones"
      "decision.source-of-truth-model.md"
```

La proyección muestra cómo recorrer artifacts.

No reemplaza sus fuentes de verdad.

## Relación con fuente de verdad documental

Una organización documental puede ordenar artifacts sin ser su fuente de verdad.

La fuente de verdad documental responde:

> ¿Dónde vive el contenido canónico?

La organización documental responde:

> ¿Cómo agrupamos o recorremos artifacts?

Un artifact puede aparecer en varias organizaciones documentales, pero debería tener una fuente de verdad clara.

## Relación con documentos

Los documentos explican conocimiento desde una pregunta principal.

La organización documental no debería reemplazar esa explicación.

Si una organización necesita explicar contexto, alcance, estructura, comportamiento, consistencia, viabilidad, decisión, actualización o feedback, debería referenciar el documento correspondiente.

La organización puede indicar que un documento importa.

No debería copiar su contenido principal.

## Relación con continuity paths

Los continuity paths conectan conceptos entre perspectivas.

La organización documental no debería reemplazar esa conexión.

Puede agrupar artifacts relacionados con un path o mostrar que un path forma parte de un recorrido, pero no debería convertirse en una matriz de trazabilidad completa.

Si el problema principal es entender cómo un concepto mantiene continuidad entre negocio, dominio, software, producto, servicio, impacto o evolución, probablemente corresponde usar un continuity path.

## Relación con diagramas

Los diagramas muestran relaciones, estructuras, flujos o caminos.

Una organización documental puede usar diagramas para representar orden.

Por ejemplo, un TreeView puede mostrar una organización documental.

Pero el diagrama no convierte la organización en una estructura obligatoria de carpetas.

Solo muestra una forma de recorrer o agrupar artifacts.

## Relación con mockups

Los mockups representan superficies, vistas o experiencias de producto.

Una organización documental puede agrupar mockups junto a documentos, feedback o decisiones.

Pero no reemplaza el mockup ni explica por sí misma la experiencia representada.

## Relación con Navigation Documents

Un Navigation Document explica cómo explorar una organización, colección, path, iteración, proyecto, concepto o caso.

La organización documental define el criterio de orden.

El Navigation Document explica el recorrido recomendado.

Una organización simple puede no necesitar Navigation Document.

Una organización compleja o transversal probablemente sí lo necesita.

## Relación con metadata

La metadata puede ayudar a materializar organizaciones documentales.

Puede indicar o derivar:

* tipo de artifact
* scope
* target
* estado
* relaciones
* pertenencia primaria
* organizaciones sugeridas
* paths asociados

La metadata no debería duplicar contenido explicativo.

Su responsabilidad es clasificar, relacionar o facilitar navegación.

## Relación con tooling futuro

VSlices Tooling podría generar organizaciones documentales o proyecciones navegables desde metadata, referencias o convenciones.

Por ejemplo:

* TreeViews
* índices
* tablas de artifacts
* mapas de navegación
* vistas por estado
* vistas por iniciativa
* vistas por release
* vistas por dominio

Esto no debe ser requisito inicial.

La organización documental debe ser útil incluso sin tooling.

## Libertad de organización

VSlices Docs Standard no impone una organización única.

Un equipo puede organizar sus artifacts de la forma que mejor preserve continuidad en su contexto.

VSlices Docs Standard puede describir estrategias recomendadas, sus ventajas, riesgos y límites.

VSlices Method puede sugerir estrategias según el tipo de trabajo.

Pero la organización final pertenece al equipo y al contexto.

## Riesgos

| Riesgo                                            | Consecuencia                                           |
| ------------------------------------------------- | ------------------------------------------------------ |
| Tratar la organización como carpetas obligatorias | Se pierde flexibilidad y aparece ceremonia innecesaria |
| Copiar contenido dentro de la organización        | Se crean fuentes de verdad competidoras                |
| Usar la organización como documento explicativo   | Se rompe la separación semántica del estándar          |
| Convertirla en matriz de trazabilidad             | Se agrega complejidad antes de necesitarla             |
| Organizar todo por una sola perspectiva           | Se ocultan recorridos válidos desde otras perspectivas |
| Crear demasiadas organizaciones                   | La documentación se vuelve difícil de mantener         |
| Confundir proyección con fuente de verdad         | No queda claro dónde vive el contenido vigente         |

## Señales de buena organización

Una organización documental está funcionando bien cuando:

* ayuda a encontrar artifacts relevantes
* permite recorrer conocimiento sin duplicarlo
* deja clara la fuente de verdad de cada artifact
* no obliga a documentar más de lo necesario
* puede convivir con otras organizaciones
* reduce pérdida de intención
* mantiene bajo el costo de navegación
* no compite con documentos ni continuity paths

## Señales de sobreingeniería

Una organización documental probablemente está agregando complejidad prematura cuando:

* exige mover artifacts constantemente
* necesita tooling para ser entendida
* obliga a crear documentos que aún no aportan valor
* duplica contenido de otros artifacts
* requiere mantener muchas vistas manuales
* convierte estados o metadata en carpetas innecesarias
* transforma cada concepto en una colección propia
* intenta resolver trazabilidad completa desde el inicio

## Reglas recomendadas

* Usar organizaciones para ordenar, no para explicar.
* Mantener clara la fuente de verdad de cada artifact.
* Preferir referencias antes que copias.
* Permitir que un artifact aparezca en varias organizaciones.
* No convertir una organización en estructura física obligatoria.
* Usar proyecciones navegables cuando ayuden a recorrer artifacts sin moverlos.
* Usar Navigation Documents cuando el recorrido necesite explicación.
* Mantener la organización lo más simple posible.
* Evolucionar la organización cuando el volumen o la complejidad lo justifiquen.
* Evitar resolver problemas futuros antes de observarlos en uso real.

## Regla de cierre

Una organización documental no existe para producir más documentación.

Existe para que los artifacts puedan encontrarse, agruparse y recorrerse sin perder continuidad.

Si una organización empieza a explicar contenido, duplicar documentos o imponer estructura innecesaria, dejó de ordenar y empezó a generar complejidad accidental.
