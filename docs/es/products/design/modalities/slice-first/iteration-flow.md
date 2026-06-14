# Énfasis de etapas en Slice-First

_Slice-First_ da más atención a Building y *feedback*.

| Etapa           | Énfasis      | Objetivo                                                                         |
| --------------- | ------------ | -------------------------------------------------------------------------------- |
| Understanding   | Bajo / Medio | Entender solo lo suficiente para evitar implementación ciega.                    |
| Contextualizing | Bajo         | Definir el contexto mínimo necesario para una *slice* segura.                    |
| Planning        | Medio        | Elegir una pequeña *vertical slice* que pueda producir aprendizaje.              |
| Building        | Alto         | Construir, validar y usar *feedback* como mecanismo principal de<br/>descubrimiento. |

_Slice-First_ no requiere la base más amplia posible, solo la base responsable más pequeña que pueda sostener la *slice*.

# Understanding en _Slice-First_

## Objetivo

El objetivo de Understanding es identificar el conocimiento mínimo de dominio requerido para evitar implementación ciega.

El equipo no intenta analizar profundamente toda el área de negocio. Se enfoca en lo que debe entenderse antes de construir una pequeña *slice*.

Esta etapa se relaciona con la pirámide invertida, pero la excavación es intencionalmente superficial y estrecha. El equipo retira solo los granos que cubren directamente la *slice*. Luego pregunta:

* ¿Qué estamos intentando aprender?
* ¿Qué concepto mínimo de negocio debemos entender?
* ¿Quién es afectado por esta *slice*?
* ¿Qué lenguaje se requiere para evitar malentendidos?
* ¿Qué flujo existente toca esta *slice*?
* ¿Qué supuesto estamos probando?
* ¿Qué podría hacer insegura esta *slice*?
* ¿Qué decidimos no entender todavía de forma intencional?
* ¿Qué nos obligaría a detenernos y cambiar de modalidad?

El objetivo no es entender todo, sino saber lo suficiente para construir sin ser imprudentes.

## Artefactos comunes de apoyo

* objetivo de aprendizaje
* glosario mínimo
* lista de supuestos
* notas de actores
* notas de flujos afectados
* preguntas abiertas
* notas de límites de la *slice*
* notas de condiciones de detención

## Riesgo principal evitado

Construir a ciegas sin saber qué se supone que la *slice* debe enseñar.

## Foco de riesgo

Understanding en _Slice-First_ debería identificar explícitamente qué está siendo ignorado o postergado. El equipo debería hacer visibles:

* supuestos aceptados por velocidad
* desconocidos que siguen sin resolverse
* reglas de negocio todavía no exploradas
* flujos dejados intencionalmente fuera de la *slice*
* actores todavía no considerados
* riesgos que harían insegura la *slice*
* condiciones que requieren cambiar a Problem-First o Context-First

El objetivo no es eliminar esos riesgos. Es saber qué riesgos están siendo aceptados.

# Contextualizing en _Slice-First_

## Objetivo

El objetivo de Contextualizing es definir el contexto mínimo necesario para una *vertical slice* segura. El equipo organiza solo el contexto requerido para construir, validar y aprender desde la *slice*.

Este escenario debería ser intencionalmente pequeño, y puede describir:

* el actor involucrado
* el punto de entrada
* el resultado esperado
* el flujo mínimo tocado por la *slice*
* las dependencias inmediatas
* las restricciones circundantes
* el límite de la *slice*
* qué queda fuera de la *slice*

Contextualizing en _Slice-First_ no debería expandirse salvo que la *slice* se vuelva insegura o pierda significado sin más contexto. Entonces, el equipo pregunta:

* ¿Cuál es el contexto significativo más pequeño para esta *slice*?
* ¿Dónde empieza la *slice*?
* ¿Dónde termina la *slice*?
* ¿Qué flujo toca?
* ¿Qué responsabilidad prueba?
* ¿Qué dependencia debe estar presente?
* ¿Qué flujos adyacentes están excluidos intencionalmente?
* ¿Qué contexto haría demasiado grande la *slice*?
* ¿Qué contexto falta, pero es aceptable por ahora?

El objetivo no es construir una base completa. El objetivo es construir suficiente base para esta *slice*.

## Artefactos comunes de apoyo

* notas de contexto de la *slice*
* boceto de flujo mínimo
* notas de límites
* notas de dependencias
* notas de contexto excluido
* notas de actores
* notas de resultado esperado
* notas de validación

## Riesgo principal evitado

Permitir que la *slice* se expanda hasta dejar de ser lo suficientemente pequeña para validar rápidamente.

## Foco de riesgo

Contextualizing en _Slice-First_ debería mantener visible la presión de alcance. El equipo debería observar:

* dependencias ocultas
* límites en expansión
* puntos de entrada o salida poco claros
* flujos adyacentes siendo arrastrados hacia la *slice*
* contexto de validación faltante
* partes interesadas agregando expectativas no relacionadas
* contexto demasiado débil para hacer significativa la *slice*
* contexto demasiado amplio para mantener rápida la *slice*

Si el contexto mínimo se vuelve demasiado grande, _Slice-First_ puede dejar de ser la modalidad correcta.

# Planning en _Slice-First_

## Objetivo

El objetivo de Planning es elegir una pequeña *vertical slice* que pueda producir aprendizaje útil.

El equipo define qué se construirá, qué se validará y qué quedará fuera de la *slice*. Planning cambia la mentalidad:

> ¿Qué podemos aprender construyendo? -> ¿Cuál es la *slice* más pequeña que puede enseñarnos eso?

El equipo pregunta:

* ¿Cuál es el objetivo de aprendizaje?
* ¿Cuál es la *vertical slice* más pequeña que puede validarlo?
* ¿Qué debe incluirse de extremo a extremo?
* ¿Qué puede excluirse intencionalmente?
* ¿Qué supuestos probará esta *slice*?
* ¿Qué *feedback* esperamos?
* ¿Qué resultado invalidaría nuestra dirección?
* ¿Qué riesgos estamos aceptando?
* ¿Cuál es el costo de desechar esta *slice*?
* ¿Qué haría que esta *slice* se vuelva accidentalmente permanente?

La *slice* preferida no es la menor cantidad de código. Es el camino significativo más pequeño desde intención hasta *feedback*.

## Artefactos comunes de apoyo

* propuesta de *slice*
* notas de objetivo de aprendizaje
* notas de alcance
* notas de fuera de alcance
* notas de *tradeoff*
* notas de riesgo
* notas de supuestos
* criterios de validación
* notas de reversión
* notas de decisión de descarte

## Riesgo principal evitado

Construir una *slice* que es pequeña en código, pero insignificante para el aprendizaje.

## Foco de riesgo

Planning en _Slice-First_ debería definir explícitamente los límites de riesgo.

El equipo debería hacer visible:

* qué puede probar la *slice*
* qué no puede probar la *slice*
* qué supuestos están siendo probados
* qué supuestos permanecen sin probar
* qué riesgos se aceptan por velocidad
* qué requeriría reversión
* qué requeriría retrabajo
* qué requeriría cambiar de modalidad
* qué impediría que la *slice* se vuelva apta para producción

El equipo debería evitar tratar la *slice* como una decisión arquitectónica completa. Una *slice* es un instrumento de aprendizaje antes de ser una estructura final.

# Building en _Slice-First_

## Objetivo

El objetivo de Building es implementar la *slice*, validar el objetivo de aprendizaje y alimentar el resultado hacia la siguiente iteración. Building incluye desarrollo, integración, validación, entrega, observación y *feedback*.

En esta etapa, el equipo puede definir o implementar:

* una *feature* delgada
* un flujo mínimo
* una capacidad pequeña
* una integración temporal
* un modelo de dominio mínimo
* un camino estrecho de UI
* un solo *endpoint*
* una automatización pequeña de proceso
* una ruta limitada de despliegue
* errores esperados solo para la *slice*

En _Slice-First_, Building es el mecanismo principal de descubrimiento.

El equipo usa *feedback* de implementación para descubrir restricciones, riesgos, conceptos faltantes y mejores preguntas. El equipo pregunta:

* ¿La *slice* validó el objetivo de aprendizaje?
* ¿Qué reveló la implementación?
* ¿Qué supuestos sobrevivieron?
* ¿Qué supuestos fallaron?
* ¿Qué conceptos de dominio se volvieron más claros?
* ¿Qué restricciones técnicas aparecieron?
* ¿Qué flujos adyacentes se volvieron relevantes?
* ¿Qué necesita refactorizarse, descartarse o expandirse?
* ¿Deberíamos continuar con _Slice-First_?
* ¿Deberíamos cambiar a Problem-First o Context-First?

El resultado de Building produce *feedback*.

A veces ese *feedback* se vuelve valor de producción; a veces se vuelve aprendizaje. Ambos son útiles, pero no deberían confundirse.

## Artefactos comunes de apoyo

* notas de implementación
* notas de validación
* notas de *feedback*
* notas de restricciones aprendidas
* notas de decisión técnica
* notas de descarte
* notas de preparación para producción
* notas de refactorización
* notas de siguiente iteración

## Riesgo principal evitado

Confundir una *slice* funcional con una solución completamente entendida.

## Foco de riesgo

Building en _Slice-First_ debería mantener visible la naturaleza temporal o limitada de la *slice*. El equipo debería observar:

* permanencia accidental
* supuestos no validados convirtiéndose en arquitectura
* código de prototipo convirtiéndose en código de producción sin revisión
* manejo de errores faltante
* preocupaciones operacionales faltantes
* reglas de negocio ocultas descubiertas demasiado tarde
* sobreinterpretación de partes interesadas
* decisiones locales de implementación convirtiéndose en restricciones globales
* *feedback* ignorado porque la *slice* ya funciona

Si la *slice* funciona, el equipo todavía debería preguntar qué probó realmente. Una *slice* funcional no es automáticamente una decisión correcta de producto.
