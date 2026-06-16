# Conclusiones de la Iteración 0

## Propósito

Este documento resume los aprendizajes obtenidos durante Iteration 0 de Domus Orbis y explica cómo esos aprendizajes pueden influir en la evolución de VSlices.

No busca repetir el paso a paso de la iteración. Su objetivo es extraer conclusiones metodológicas, documentales, de diseño y de tooling a partir de un caso real.

## Uso de IA durante la iteración

La IA fue usada como contraparte de trabajo.

Ayudó a:

* ordenar el problema;
* detectar sobrealcance;
* proponer documentos;
* redactar versiones iniciales;
* revisar si una solución pertenecía a Iteration 0 o a una evolución futura;
* transformar conversación en documentación;
* mantener foco en la necesidad actual.

La IA no reemplazó la observación del dominio. La necesidad real vino del uso cotidiano del hogar.

En este caso, la IA funcionó como apoyo para preservar continuidad, no como fuente automática de verdad.

### Preguntas abiertas

* ¿Cómo podríamos generar un agente de IA que apoye directamente la aplicación de Method?
* ¿Sería posible generar un agente de IA que ayude a observar qué cosas pueden extender nuestros productos?

## Qué se descubrió

Iteration 0 dejó varios aprendizajes.

Primero, el problema real no era automatizar compras. Era que la lista mensual debía existir antes del pago.

Segundo, una solución pequeña podía aportar valor sin convertirse todavía en aplicación.

Tercero, la documentación debía vivir cerca del proyecto porque su objetivo era ayudar a retomar el trabajo después.

Cuarto, los documentos necesarios dependían del alcance. No todas las fases necesitaron la misma cantidad de documentos.

Quinto, el *artifact* inicial debía ser pequeño, pero no desechable. Aunque luego aparezcan herramientas, integraciones o automatización, la lista centralizada sigue siendo una pieza útil.

## Qué podría hacerse distinto según el contexto

Este caso fue pequeño, personal y urgente.

Por eso, algunos documentos fueron notas livianas y algunos *artifacts* fueron suficientes sin guía formal. En otro contexto, podría cambiar.

Un proyecto con más personas podría necesitar:

* decisiones explícitas
* guías de uso
* validaciones más formales
* diagramas adicionales
* revisión de stakeholders
* criterios de aceptación más estrictos

Un proyecto con más riesgo técnico podría necesitar:

* pruebas de integración
* spikes técnicos
* decisiones de arquitectura
* validación de proveedores externos
* estrategia de rollback

Un proyecto con mayor impacto económico podría requerir:

* controles de autorización
* auditoría
* trazabilidad
* confirmaciones humanas
* límites operativos

Domus Orbis no define una receta universal. Muestra cómo se eligió el conjunto documental mínimo útil para este alcance.

### Preguntas abiertas

* ¿Cómo afecta el impacto económico a los productos de VSlices?
* ¿Cómo afecta el riesgo técnico?
* ¿Cómo afecta el tamaño del equipo?
* ¿Cómo afecta el plazo del proyecto?

## Selección de documentos

Una de las reglas más importantes observadas fue:

> Ninguna fase de VSlices Method tiene una cantidad fija de documentos.

Los documentos se eligen según el alcance, el riesgo, la incertidumbre y la responsabilidad de la fase.

En Domus Orbis, dado su carácter más casual y personal, una sola persona cumplía varios roles al mismo tiempo. Ese contexto no exigía documentar límites de forma constante.

Esto se menciona porque otro proyecto puede requerir mayor énfasis en los límites si tiene más involucrados, más conceptos en juego o un perfil menos casual y más formal.

### Preguntas abiertas

* ¿Qué características de los proyectos afectan a qué partes de la documentación?

## Uso de la metodología

Domus Orbis mostró que Slice-First puede partir desde un problema cotidiano y pequeño sin perder valor metodológico.

El aprendizaje central fue:

> El primer slice no debe imitar una versión miniatura del sistema futuro. Debe proteger la necesidad actual con la menor cantidad de contexto suficiente.

En este caso, el sistema futuro podría incluir automatización, mercados, pagos o inventario. Pero la primera necesidad era mucho más pequeña:

> La lista mensual debe existir antes del pago.

Ese fue el punto de partida.

## Diagramas según responsabilidad

Los diagramas se usaron donde ayudaban a cumplir la responsabilidad del documento.

El documento de proceso usó un diagrama de flujo porque necesitaba mostrar pasos y fricción.

La propuesta de solución usó una versión modificada del flujo para mostrar la intervención mínima propuesta.

Esto llevó a una regla futura para VSlices Docs Standard:

> Cada documento puede definir las vistas o diagramas que necesita según la pregunta que debe responder.

Los diagramas no son obligatorios por defecto, pero tampoco son decoración cuando ayudan a entender más rápido.

### Preguntas abiertas

* ¿Cómo los diagramas harán evolucionar VSlices Docs Standard, considerando sus responsabilidades actuales y futuras?

## Documentación colocalizada

La documentación de Domus Orbis vive dentro del [mismo proyecto](https://github.com/HernanFAR/DomumOrbis), bajo una carpeta [Docs](https://github.com/HernanFAR/DomumOrbis/tree/master/Docs).

Esto fue intencional. Cuando la documentación está cerca de la implementación, se vuelve más fácil preservar continuidad entre:

* contexto
* scope
* vocabulario
* procesos
* propuestas
* *artifacts*
* validaciones
* código futuro

### Preguntas abiertas

* ¿Cómo facilita esto la integración con el CLI futuro y otras iteraciones de los productos?

## Qué productos de VSlices pueden evolucionar

### VSlices Method

Este caso refuerza que Iteration 0 puede usarse para documentar la realidad actual antes de definir el primer Slice-First.

También refuerza que ninguna fase tiene un conjunto fijo de documentos. Las fases guían el razonamiento, pero los *artifacts* y la documentación dependen del contexto.

### VSlices Docs Standard

#### Confirmaciones de utilidad de ideas

Este caso confirma la utilidad de varias ideas:

* naming convention con segmentos como `context.scenario.md`, usando una forma cercana a `<tipo>.<nombre-corto>`;
* vocabulario selectivo, sin llenar todos los slots cuando no aportan valor.

#### Nueva taxonomía: Diagramas

Este caso confirma la necesidad de que VSlices Docs Standard considere una nueva taxonomía para diagramas.

| Contexto                                 | Diagrama relacionado                        |
| ---------------------------------------- | ------------------------------------------- |
| Definiendo scope del escenario           | Diagrama de casos de uso                    |
| Definiendo scope de la iteración         | Diagrama de casos de uso                    |
| Escribiendo un documento de proceso      | Diagrama de flujo, diagrama de carriles     |
| Escribiendo un documento de caso de uso  | Diagrama de flujo, comportamiento o estados |
| Escribiendo un documento de capacidad    | Mapa de dependencias                        |
| Escribiendo el vocabulario de un dominio | Diagrama de flujo                           |

En caso de que abramos una línea de Diagramas, hay que considerar:

* qué significado daremos a cada pieza o contenedor;
* cuándo recomendamos usar estos diagramas según contexto;
* cómo estos diagramas se relacionan con un documento específico.

#### Nuevos documentos

Esta iteración abrió un punto importante: las notas de soporte, como tal, pueden funcionar como versiones primitivas de documentos más específicos.

Muchos de estos documentos más específicos todavía no tienen un equivalente directo dentro de VSlices Docs Standard.

Por ejemplo:

| Documento                                                                                                                            | Posible derivado                  |
| ------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- |
| [improvement.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/improvement.solution.md) | Documento de mejoras continuas L0 |
| [proposal.solution](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/planning/proposal.solution.md)       | Documento de propuesta L0         |
| [scope.iteration](https://github.com/HernanFAR/DomumOrbis/blob/master/Docs/Iteraci%C3%B3n%200/understanding/scope.iteration.md)      | Documento de alcance L0           |

Cada documento tendría una responsabilidad específica y diferenciada de otros documentos.

#### Uso de Support Note

El concepto de Support Note ha demostrado ser muy útil para definir documentos más complejos de forma simple.

Sin embargo, también ha demostrado ser demasiado genérico para funcionar como equivalente 1:1 de versiones específicas L0.

Esto significa que debemos considerar la opción de generar una versión L0 de cada documento dentro de los templates.

No es descabellado, ya que la naturaleza de las Support Notes obliga a agregar nuevos párrafos o segmentos cuando se usan para representar documentos más específicos, como un Documento de contexto L0.

Para las Support Notes, esto significa que ya no necesariamente representan un documento L0. Representan una idea general de algo, que puede o no ser oficial, y que puede o no convertirse en un documento L0 con nuevos segmentos por defecto en una entrega futura.

### VSlices Design

Este caso ayuda a enseñar separación entre:

* necesidad actual
* proceso actual
* solución propuesta
* *artifact* inicial
* mejora futura
* automatización prematura

También muestra cómo un problema cotidiano puede revelar límites de dominio importantes.

### VSlices Framework

Este caso refuerza que la documentación colocalizada puede ser importante para tooling futuro.

Si los documentos viven cerca del proyecto, un CLI podría descubrir *artifacts*, validar relaciones, generar scaffolding o revisar continuidad entre documentación e implementación.

#### Preguntas abiertas

* ¿Cómo funcionaría el tooling de autogeneración de código con VSlices Docs Standard?
