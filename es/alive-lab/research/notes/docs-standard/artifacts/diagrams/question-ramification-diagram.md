# Diagrama de ramificación de consultas

## Propósito

Un "Diagrama de ramificación de consultas" es una estructura visual usada para organizar preguntas derivadas desde una pregunta documental principal.

Su objetivo es orientar cómo organizar un artifact, no definir obligatoriamente cómo debe verse.

El diagrama ayuda a responder:

* qué preguntas debe cubrir el artifact
* qué ramas son principales
* qué ramas son de apoyo
* qué tan costoso parece incorporar una rama
* qué partes conviene documentar ahora
* qué partes pueden quedar identificadas para una evolución futura

## Idea central

Una pregunta documental principal puede abrirse en preguntas derivadas.

Estas preguntas derivadas orientan la organización del artifact.

La ramificación no prescribe una forma concreta de materialización.

Una rama puede terminar representada como:

* heading
* tabla
* lista
* metadata
* diagrama
* nota
* callout
* ejemplo
* sección narrativa
* cualquier otra forma que preserve mejor el conocimiento

La regla importante es:

> La ramificación organiza el conocimiento.
> No impone el formato del documento.

## Lectura de los nodos

Cada nodo representa una rama de organización.

Un nodo puede contener:

* el nombre conceptual de la rama
* la pregunta que esa rama responde

Ejemplo:

```mermaid
flowchart LR
    ROOT["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]
    BRANCH1["Terminología<br/><small>¿Qué términos usamos?</small>"]
    BRANCH2["Regla de uso<br/><small>¿Cuándo usar este vocabulario?</small>"]

    ROOT --> BRANCH1 & BRANCH2
```

En este caso:

* `Vocabulario de dominio` representa el artifact o estructura principal
* `¿Cómo hablamos?` representa la pregunta documental principal
* `Terminología` representa una rama de organización
* `¿Qué términos usamos?` representa la pregunta que esa rama responde
* `Regla de uso` representa otra rama de organización
* `¿Cuándo usar este vocabulario?` representa la pregunta que esa rama responde

## Reglas iniciales

### 1. La pregunta principal define la identidad del artifact

La raíz del diagrama representa la pregunta documental principal.

Ejemplo:

```mermaid
flowchart LR
    ROOT["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]
```

La pregunta principal no obliga a documentar todo en profundidad.

Solo define la intención central del artifact.

### 2. Las ramificaciones organizan preguntas derivadas

Cada rama responde una pregunta derivada de la pregunta principal.

Ejemplo:

```mermaid
flowchart LR
    ROOT["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]
    BRANCH1["Terminología<br/><small>¿Qué términos usamos?</small>"]

    ROOT --> BRANCH1
```

La rama `Terminología` existe porque ayuda a responder cómo hablamos desde una pregunta más específica:

> ¿Qué términos usamos?

### 3. Las líneas expresan relevancia o naturaleza de la relación

La relevancia entre ramificaciones se marca mediante diferencias en la línea que conecta los nodos.

Semántica inicial:

| Línea  | Significado                                                  |
| ------ | ------------------------------------------------------------ |
| `-->`  | Rama principal del contenido                                 |
| `-.->` | Rama de apoyo, mantenimiento, gobernanza o contexto auxiliar |

Ejemplo:

```mermaid
flowchart LR
    ROOT["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]

    BRANCH1["Terminología<br/><small>¿Qué términos usamos?</small>"]
    BRANCH2["Regla de uso<br/><small>¿Cuándo usar este vocabulario?</small>"]
    BRANCH3["Mantenimiento<br/><small>¿Quién mantiene este documento?</small>"]

    ROOT --> BRANCH1 & BRANCH2
    ROOT -.-> BRANCH3
```

Lectura:

* `Terminología` y `Regla de uso` son ramas principales del contenido
* `Mantenimiento` es una rama de apoyo o gobernanza del artifact

### 4. Las formas de los nodos expresan esfuerzo

La forma del nodo puede usarse para comunicar cuánto esfuerzo implica incorporar o mantener una rama.

Esto permite separar importancia de costo.

Una rama puede ser importante, pero demasiado costosa para incorporarse en la iteración actual.

Semántica inicial candidata:

| Forma              | Significado                                            |
| ------------------ | ------------------------------------------------------ |
| Rectángulo         | Esfuerzo bajo                                          |
| Bordes redondeados | Esfuerzo medio                                         |
| Forma destacada    | Esfuerzo alto                                          |
| Forma alternativa  | Esfuerzo variable o dependiente de información externa |

La forma exacta puede cambiar según las limitaciones visuales de Mermaid o las convenciones que adopte Docs Standard.

Lo importante es la regla:

> La línea expresa relevancia o naturaleza.
> La forma expresa esfuerzo o costo de incorporación.

### 5. Importancia no significa incorporación inmediata

Una rama puede ser:

* importante pero costosa
* simple pero secundaria
* principal pero postergable
* auxiliar pero necesaria para mantener continuidad

El diagrama ayuda a decidir qué documentar ahora y qué dejar como evolución futura.

### 6. El diagrama no reemplaza el contenido

El Diagrama de ramificación orienta la organización del artifact.

No reemplaza la explicación, evidencia, reglas, vocabulario, decisiones o contenido que el artifact debe preservar.

## Ejemplo actual

```mermaid
flowchart LR
    ROOT["Vocabulario de dominio<br/><small>¿Cómo hablamos?</small>"]

    BRANCH1["Terminología<br/><small>¿Qué términos usamos?</small>"]
    BRANCH2["Regla de uso<br/><small>¿Cuándo usar este vocabulario?</small>"]
    BRANCH3["Mantenimiento<br/><small>¿Quién mantiene este documento?</small>"]

    ROOT --> BRANCH1 & BRANCH2
    ROOT -.-> BRANCH3
```

Este diagrama indica que el artifact `Vocabulario de dominio` se organiza inicialmente alrededor de tres preguntas:

* ¿Qué términos usamos?
* ¿Cuándo usar este vocabulario?
* ¿Quién mantiene este documento?

Las dos primeras preguntas forman parte del contenido principal.

La tercera pregunta corresponde a mantenimiento o gobernanza del artifact.

## Puntos que pueden cambiar

Esta definición todavía es candidata.

Pueden cambiar:

* el nombre final de `Diagrama de ramificación`
* la semántica exacta de cada tipo de línea
* la semántica exacta de cada forma de nodo
* la cantidad de niveles de ramificación recomendados
* si las ramas de mantenimiento deberían aparecer siempre o solo cuando aporten valor
* si algunas preguntas deberían materializarse como metadata en vez de contenido visible
* si los diagramas deberían usar siempre `flowchart LR` o permitir otras direcciones
* si Docs Standard define una leyenda común para todos los diagramas de ramificación
* si Tooling debería validar estas convenciones en el futuro

## Regla de prudencia

El Diagrama de ramificación debe ayudar a reducir complejidad, no aumentarla.

Si el diagrama exige más esfuerzo que el artifact que intenta organizar, probablemente está agregando ceremonia prematura.

Primero debe servir para pensar.

Después, si el uso real lo justifica, puede convertirse en convención, plantilla o regla validable por tooling.
