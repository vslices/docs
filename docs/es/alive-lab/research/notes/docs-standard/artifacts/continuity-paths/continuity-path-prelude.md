# Prelude de Continuity Paths

## Propósito

Este documento introduce el concepto de **Continuity Path** dentro de VSlices Docs Standard.

Su objetivo es preparar la lectura de esta familia de artifacts sin reemplazar la definición específica de cada path.

Los Continuity Paths existen para preservar continuidad cuando un target aparece a través de distintas perspectivas, artifacts, decisiones o superficies del sistema.

## Problema que resuelven

Un mismo elemento puede aparecer:

* en una situación de negocio
* en un contexto de dominio
* en una decisión
* en una iniciativa de software
* en un producto
* en un servicio consumible
* en una estructura técnica
* en feedback o validaciones
* en cambios de alcance
* en artifacts posteriores

Cuando esas conexiones no son visibles, el conocimiento se fragmenta.

Podemos saber qué se implementó y aun así perder:

* por qué importaba
* dónde apareció
* qué significado tenía
* qué decisión lo transformó
* qué alcance cambió
* dónde se materializó
* qué impacto produjo
* quién lo sostiene

## Qué es un Continuity Path

Un Continuity Path es un artifact que conecta y orienta continuidad alrededor de un target.

Declara:

* una pregunta de continuidad
* el foco que intenta preservar
* los artifacts o paths conectados
* el rol que cumple cada conexión

Definición compacta:

> Un Continuity Path conecta un target a través de perspectivas relevantes para preservar continuidad.

No reemplaza los artifacts conectados.

El path orienta el recorrido.

Los artifacts preservan el detalle.

## Qué no es

Un Continuity Path no es:

* una explicación completa del target
* una matriz de trazabilidad obligatoria
* una estructura de carpetas
* un proceso de gestión
* una lista exhaustiva de documentos
* una regla para documentar cada nodo
* un grafo vivo obligatorio
* una auditoría formal
* un Nexus
* un Navigation Document

## Separación de responsabilidades

VSlices Docs Standard mantiene esta separación:

* Los Documents explican.
* Las Support Notes apoyan, registran o referencian.
* Los Nexus componen.
* Los Continuity Paths conectan y orientan continuidad.
* Los diagramas muestran.
* Los mockups representan.
* La organización documental ordena.
* Las proyecciones navegables muestran organizaciones.
* Los Navigation Documents explican recorridos.

Un Continuity Path puede ser mostrado mediante un diagrama.

Eso no convierte al diagrama en el path completo.

## Cómo se lee

Un Continuity Path se lee como un mapa de continuidad.

Ayuda a identificar:

* por dónde comenzar
* qué pregunta seguir
* qué artifacts revisar
* qué relaciones son principales
* qué elementos ya están documentados
* qué elementos solo necesitan visibilidad
* qué elementos podrían requerir documentación
* cuándo cambiar de perspectiva
* cuándo detenerse

La metáfora útil es una ciudad:

* el path identifica rutas
* los artifacts son lugares consultables
* el diagrama muestra el mapa
* el Navigation Document explica cómo recorrerlo
* la organización documental ordena barrios o colecciones

## Semántica visual

Los diagramas pueden usar esta semántica inicial:

| Forma       | Significado                                           |
| ----------- | ----------------------------------------------------- |
| `[[texto]]` | Elemento documentado                                  |
| `[texto]`   | Pregunta u orientación                                |
| `>texto]`   | Elemento identificado sin necesidad documental actual |
| `{{texto}}` | Elemento con posible necesidad documental             |

> `{{texto}}` no obliga a documentar inmediatamente.
> Señala una necesidad que debe evaluarse.

Las relaciones pueden distinguir intención:

| Relación | Significado                                        |
| -------- | -------------------------------------------------- |
| `-->`    | Camino principal o relación directa                |
| `-.->`   | Camino auxiliar, contextual, secundario u opcional |

## Categorías de Continuity Paths

Los Continuity Paths se agrupan inicialmente en tres categorías.

| Categoría  | Responsabilidad                                     |
| ---------- | --------------------------------------------------- |
| Core       | Observar perspectivas principales de continuidad    |
| Supporting | Observar preocupaciones transversales               |
| Contextual | Preservar continuidad ante una situación específica |

Estas categorías orientan el uso.

No constituyen una taxonomía cerrada.

## Core Continuity Paths

| Path                | Perspectiva            |
| ------------------- | ---------------------- |
| Business Scenario   | Escenario de negocio   |
| Business Driver     | Motivación de negocio  |
| Domain Context      | Contexto de dominio    |
| Viability           | Viabilidad             |
| Evolution           | Evolución              |
| Software Initiative | Iniciativa de software |
| Client Product      | Producto al cliente    |
| Consumable Service  | Servicio consumible    |

## Supporting Continuity Paths

| Path             | Perspectiva          |
| ---------------- | -------------------- |
| Software Project | Proyecto de software |
| Ownership        | Responsabilidad      |
| Impact           | Impacto              |
| Traceability     | Trazabilidad         |

Los Supporting Continuity Paths no reemplazan a los Core.

Los complementan cuando necesitamos seguir materialización técnica, responsabilidad, impacto o trazabilidad.

## Contextual Continuity Paths

Los Contextual Continuity Paths aparecen frente a una situación concreta.

Primer candidato:

| Path              | Situación                                         |
| ----------------- | ------------------------------------------------- |
| Knowledge Handoff | Transferencia o pérdida potencial de conocimiento |

Un path contextual no necesita convertirse en Core por ser valioso.

## Cómo elegir un path

La elección depende de la pregunta actual.

| Necesidad                                                 | Path sugerido       |
| --------------------------------------------------------- | ------------------- |
| Entender dónde ocurre el trabajo                          | Business Scenario   |
| Entender por qué importa intervenir                       | Business Driver     |
| Entender lenguaje, reglas o límites del dominio           | Domain Context      |
| Evaluar si algo puede sostenerse                          | Viability           |
| Seguir cambios sin perder intención                       | Evolution           |
| Entender qué esfuerzo de software aborda el trabajo       | Software Initiative |
| Entender la experiencia visible                           | Client Product      |
| Entender qué consume otro sistema                         | Consumable Service  |
| Entender la materialización técnica                       | Software Project    |
| Entender quién sostiene el conocimiento o responsabilidad | Ownership           |
| Entender qué se ve afectado                               | Impact              |
| Reconstruir origen y materialización                      | Traceability        |
| Preservar conocimiento durante una transferencia          | Knowledge Handoff   |

No necesitamos recorrer todos los paths.

Elegimos el que reduce la incertidumbre actual.

## Relación con otros artifacts

Un Continuity Path puede conectar:

* Documents
* Support Notes
* Nexus
* otros Continuity Paths
* diagramas
* mockups
* referencias externas
* artifacts técnicos

No obliga a crear artifacts nuevos.

Puede conectar artifacts existentes o señalar una necesidad documental candidata.

La pregunta correcta no es:

> ¿Qué documentos exige este path?

La pregunta correcta es:

> ¿Qué artifacts ayudan a preservar esta continuidad?

## Viability y Evolution

Viability preserva continuidad entre una intención y las condiciones que permiten o impiden sostenerla.

Puede conectarse con:

* Viability Document
* Scope Document
* Decision Record
* Support Note `validation`
* Support Note `risk`

Evolution preserva continuidad entre estados de un mismo elemento.

Puede conectarse con:

* Update Document
* Decision Record
* Feedback Document
* Scope Document
* Impact
* Traceability

Evolution no reemplaza al Update Document.

Evolution conecta la historia del cambio.

Update Document explica qué debe actualizarse.

## Software Initiative y Software Project

Software Initiative observa el esfuerzo organizado de software:

* qué intenta cubrir
* qué capacidades necesita
* qué productos o servicios participan
* qué proyectos puede originar

Software Project observa su materialización técnica:

* estructura
* implementación
* dependencias
* adapters
* decisiones técnicas
* evolución del código

> Software Initiative mira la cobertura del esfuerzo.
> Software Project mira la materialización técnica.

## Cuándo detenerse

Conviene detener el recorrido cuando:

* la pregunta inicial ya fue respondida
* los artifacts relevantes ya están identificados
* no existe pérdida real de continuidad
* una relación no aporta orientación, decisión ni aprendizaje
* documentar más agregaría ceremonia
* el target solo necesitaba visibilidad

## Riesgos comunes

| Riesgo                               | Consecuencia                           |
| ------------------------------------ | -------------------------------------- |
| Usar paths como checklist            | Documentación prematura                |
| Recorrer todos los paths siempre     | Pérdida de foco                        |
| Confundir path con explicación       | Duplicación de contenido               |
| Convertir cada nodo en artifact      | Inflación de la taxonomía              |
| Confundir Nexus con path             | Mezcla entre composición y continuidad |
| Confundir navegación con continuidad | Solapamiento de responsabilidades      |
| Automatizar antes de validar         | Complejidad prematura                  |
| Documentar necesidades futuras       | Resolver Iteración 5 en Iteración 1    |

## Estado de validación

Esta familia debe entenderse como candidata.

Surge de observaciones sobre continuidad entre negocio, dominio, documentación, arquitectura e implementación.

Debe validarse mediante:

* proyectos reales
* casos de VSlices Research
* uso aplicado
* aprendizaje dentro de Domus Orbis y otros laboratorios

Hasta reunir suficiente evidencia, los Continuity Paths no deben tratarse como una taxonomía cerrada u obligatoria.

## Principio de continuidad

!!! principle "Principio de Continuidad"

```
Los Continuity Paths deberían preservar conexiones relevantes entre intención, contexto, dominio, viabilidad, evolución, software, producto, servicio y evidencia sin convertir la documentación en una obligación exhaustiva.
```
