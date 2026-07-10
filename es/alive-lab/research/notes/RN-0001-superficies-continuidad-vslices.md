---
type: research-note
state: candidate
code: RN-0001

related_questions:
* RQ-001 

related_synthesis:
* SYN-0001

related_studies:
* STU-001
* STU-002
* STU-003
* STU-004

affects:
* VSlices Research
* VSlices Design
* VSlices Docs Standard
* VSlices Method
* VSlices Framework
---

# RN-0001 — Superficies de continuidad en VSlices

## Tipo

research-note

## Estado

candidate

## Propósito

Esta nota registra una idea conceptual emergente para VSlices Research:

> VSlices puede entenderse como una suite compuesta por distintas superficies que intentan preservar continuidad de conocimiento en momentos diferentes del trabajo de software.

La nota no propone todavía una taxonomía oficial, una decisión de producto ni una conclusión validada.

Su propósito es ordenar una intuición útil que apareció al conectar `RQ-001` con los elementos principales de la suite: VSlices Design, VSlices Docs Standard, VSlices Method y VSlices Framework.

## Pregunta relacionada

[RQ-001 — Problema fundacional de VSlices Research](../questions/rq-001-problema-fundacional-vslices.md)

La pregunta fundacional estudia qué problema práctico dio origen a VSlices y cómo ese problema puede transformarse en una línea de investigación aplicada sobre continuidad de conocimiento sin perder su raíz práctica.

Esta nota ayuda a explorar cómo ese problema fundacional podría expresarse en distintas partes de la suite.

## Síntesis relacionada

[SYN-0001 — Escenarios iniciales de ruptura o escape de continuidad de conocimiento](../synthesis/syn-0001-escenarios-iniciales-ruptura-escape-continuidad-conocimiento.md)

`SYN-0001` propone, en estado `candidate`, que la continuidad de conocimiento puede verse comprometida en al menos cuatro escenarios iniciales:

* pérdida histórica
* dispersión activa
* concentración personal
* escape inicial

Esta nota no reemplaza esa síntesis. La usa como punto de partida para observar qué tipo de respuesta intenta ofrecer cada superficie de VSlices frente al problema de continuidad.

## Idea central

VSlices no responde al problema de continuidad desde una sola capa.

En cambio, parece distribuir distintas responsabilidades de continuidad entre varias superficies:

| Superficie            | Tipo de continuidad que intenta preservar                                                        |
| --------------------- | ------------------------------------------------------------------------------------------------ |
| VSlices Design        | Continuidad en el razonamiento, el modelado, el descubrimiento y las decisiones conceptuales     |
| VSlices Docs Standard | Continuidad en la documentación, la intención, el lenguaje, las relaciones y los artifacts vivos |
| VSlices Method        | Continuidad en la forma de recorrer el trabajo, evolucionar conocimiento y conectar etapas       |
| VSlices Framework     | Continuidad en el código, el comportamiento, las capacidades explícitas y la estructura técnica  |

Esta formulación debe tratarse como candidata.

Todavía no demuestra que estas superficies funcionen, que estén correctamente separadas ni que cubran todos los escenarios posibles de ruptura o escape de continuidad.

## Superficie 1: VSlices Design

VSlices Design puede entenderse como la superficie encargada de preservar continuidad en la forma de pensar, descubrir y modelar un proyecto de software.

Su aporte principal no sería imponer una arquitectura única, sino entregar lenguaje conceptual para razonar sobre:

* el estado del proyecto
* el nivel de incertidumbre
* el tipo de problema observado
* las decisiones de diseño disponibles
* el momento adecuado para introducir complejidad
* las formas de recorrer el trabajo según el contexto

Desde esta perspectiva, conceptos como etapas del proyecto, modalidades y criterios de diseño progresivo pueden investigarse como mecanismos candidatos para preservar continuidad antes de que existan decisiones técnicas estables.

### Pregunta que abre

¿Cómo ayuda VSlices Design a preservar continuidad durante el descubrimiento, el modelado y la toma progresiva de decisiones de diseño?

### Riesgo

VSlices Design podría convertirse en teoría de proceso demasiado abstracta si sus conceptos no se validan contra casos concretos.

## Superficie 2: VSlices Docs Standard

VSlices Docs Standard puede entenderse como la superficie encargada de preservar continuidad mediante documentación viva, mínima y conectada.

Su aporte principal no sería producir más documentos, sino ayudar a que el conocimiento relevante no quede aislado, implícito o desconectado de las decisiones que lo originaron.

Desde esta perspectiva, documentos de contexto, documentos de comportamiento, documentos de estructura y caminos de continuidad pueden investigarse como mecanismos candidatos para preservar:

* intención
* lenguaje de dominio
* decisiones
* relaciones
* límites
* comportamiento esperado
* evolución de conceptos
* trazabilidad entre comprensión y construcción

Un camino de continuidad no debería entenderse solo como una fábrica de documentos.

Debe entenderse como una perspectiva que ayuda a producir comprensión, conceptos y relaciones, documentándolos cuando corresponde.

### Pregunta que abre

¿Cuándo la documentación mínima y conectada ayuda a preservar continuidad, y cuándo empieza a convertirse en ceremonia?

### Riesgo

VSlices Docs Standard podría agregar burocracia si documenta más de lo que el contexto necesita o si convierte cada intuición en artifact permanente demasiado pronto.

## Superficie 3: VSlices Method

VSlices Method puede entenderse como la superficie encargada de preservar continuidad durante el recorrido del trabajo.

Su aporte principal no sería reemplazar Scrum, XP, Lean, DDD u otras prácticas, sino articular cómo se conectan el entendimiento del dominio, las decisiones de diseño, la documentación, la arquitectura, la implementación y la validación durante una iteración o evolución del sistema.

Desde esta perspectiva, Method puede investigarse como un mecanismo candidato para evitar que el conocimiento se pierda entre etapas como:

* entender
* contextualizar
* planificar
* construir
* validar
* evolucionar

También puede ayudar a observar cuándo una idea debe permanecer como observación, cuándo puede convertirse en finding y cuándo podría afectar a un producto de VSlices.

### Pregunta que abre

¿Cómo puede VSlices Method sostener continuidad entre etapas e iteraciones sin convertirse en una metodología pesada o cerrada?

### Riesgo

VSlices Method podría formalizarse demasiado temprano si intenta resolver demasiados problemas de proceso antes de validar sus mecanismos en casos pequeños.

## Superficie 4: VSlices Framework

VSlices Framework puede entenderse como la superficie encargada de expresar continuidad en código, patrones técnicos, primitivas y abstracciones reutilizables.

Su aporte principal no sería implementar directamente todo lo que aparece en Design, Docs Standard o Method, sino materializar solo aquellas ideas que han madurado lo suficiente para justificar soporte técnico.

Desde esta perspectiva, conceptos como comportamiento explícito, errores explícitos, capacidades explícitas, composición funcional, orientación a vertical slices y arquitectura progresiva pueden investigarse como mecanismos candidatos para preservar continuidad entre:

* intención de dominio
* comportamiento esperado
* estructura técnica
* implementación
* evolución del sistema

El Framework debería ser una consecuencia de aprendizaje validado, no el punto de partida obligatorio de VSlices.

### Pregunta que abre

¿Cuándo una idea observada en Design, Docs Standard o Method tiene suficiente madurez para expresarse como abstracción técnica dentro del Framework?

### Riesgo

VSlices Framework podría introducir complejidad prematura si convierte ideas candidatas en primitivas técnicas antes de contar con evidencia suficiente.

## Relación candidata entre superficies

Una forma inicial de entender la relación entre superficies es:

```text
Continuidad de conocimiento
  ├─ Design
  │   └─ continuidad en razonamiento, modelado y decisiones conceptuales
  ├─ Docs Standard
  │   └─ continuidad en documentación, intención y relaciones explícitas
  ├─ Method
  │   └─ continuidad en el recorrido del trabajo y evolución del conocimiento
  └─ Framework
      └─ continuidad en código, comportamiento y estructura técnica
```

Esta relación no debe tratarse todavía como arquitectura oficial de la suite.

Debe tratarse como una hipótesis de organización útil para abrir nuevas preguntas de investigación.

## Interpretación inicial

Esta nota sugiere que el problema fundacional de VSlices no se expresa en una sola dimensión.

La continuidad puede romperse en el pensamiento, en la documentación, en el proceso, en el código o entre esas superficies.

Por eso, una línea de investigación aplicada sobre continuidad podría necesitar observar no solo si existe documentación o si existe arquitectura, sino cómo se preserva el vínculo entre:

* lo que se descubre
* lo que se entiende
* lo que se decide
* lo que se documenta
* lo que se implementa
* lo que se valida
* lo que se aprende durante la evolución

## Evidencia inicial disponible

Esta nota se apoya inicialmente en:

* la formulación de `RQ-001`
* los escenarios integrados en `SYN-0001`
* la existencia de cuatro superficies principales dentro de VSlices
* los studies fundacionales `STU-001`, `STU-002`, `STU-003` y `STU-004`
* la necesidad de evitar que ideas candidatas se conviertan prematuramente en producto oficial

## Evidencia faltante

Para fortalecer esta nota, todavía falta observar:

* cómo cada superficie aparece en casos vivos de Alive Lab
* qué superficie ayuda realmente en cada tipo de ruptura o escape de continuidad
* qué mecanismos concretos preservan continuidad y cuáles solo agregan estructura
* qué ocurre cuando dos superficies se solapan
* qué ideas deberían permanecer en Research y cuáles podrían madurar hacia producto
* cómo Domus Orbis y Surreal Atlas tensionan esta división
* si hay superficies adicionales no consideradas todavía, como Tooling o Validation

## Riesgos metodológicos

### Riesgo de convertir el mapa en teoría oficial

Esta nota podría malinterpretarse como una definición estable de la suite.

Por ahora, solo debe usarse como orientación candidata.

### Riesgo de sobrediseñar la investigación

La división en superficies puede tentar a abrir demasiadas RQs al mismo tiempo.

La investigación debería avanzar con preguntas pequeñas y observables.

### Riesgo de confirmar la suite en vez de investigarla

La nota no debe usarse para demostrar que VSlices está bien diseñado.

Debe usarse para preguntar dónde ayuda, dónde falla, dónde falta evidencia y dónde podría estar agregando complejidad innecesaria.

### Riesgo de acoplar Research al producto

VSlices Research debe poder cuestionar estas superficies.

No debe existir solo para justificarlas.

## Posibles preguntas futuras

Esta nota podría abrir preguntas como:

* ¿Qué tipo de continuidad intenta preservar cada superficie de VSlices?
* ¿Qué mecanismos concretos ayudan a preservar continuidad en cada superficie?
* ¿Cuándo una ruptura de continuidad requiere documentación, método, diseño o soporte técnico?
* ¿Cómo se evita que VSlices Framework implemente ideas todavía candidatas?
* ¿Cómo se valida que un camino de continuidad preservó comprensión y no solo produjo documentos?
* ¿Qué señales indican que una idea observada en Alive Lab debería avanzar hacia VSlices Design, Docs Standard, Method, Framework o Tooling?
* ¿Dónde se solapan Design, Docs Standard y Method al intentar preservar continuidad?
* ¿Qué superficie responde mejor a cada escenario de `SYN-0001`?

## Puede afectar a

* VSlices Research
* VSlices Design
* VSlices Docs Standard
* VSlices Method
* VSlices Framework
* VSlices Tooling

## Límite actual

Esta nota no demuestra que VSlices preserve continuidad.

Tampoco demuestra que Design, Docs Standard, Method y Framework estén correctamente separados.

Solo propone una forma candidata de observar la suite desde el problema fundacional de continuidad de conocimiento.

Su valor actual está en ayudar a formular preguntas más pequeñas, trazables y validables desde una base conceptual común.
