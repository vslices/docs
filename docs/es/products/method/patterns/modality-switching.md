# Cambio de modalidad

Cambio de modalidad (_Modality Switching_ en inglés) explica cuándo y por qué un equipo puede moverse de una modalidad de _VSlices Design_ a otra.

Una modalidad no es una etiqueta permanente para una iteración. Es un énfasis que ayuda al equipo a reducir la incertidumbre que más importa ahora.

Cuando la incertidumbre cambia, puede que la modalidad también necesite cambiar.

## Idea central

Cambia de modalidad cuando la modalidad actual ya no está reduciendo la incertidumbre dominante. 

La pregunta no es: _¿Tenemos permitido cambiar de modalidad?_, si no 
_¿Cambió el tipo de incertidumbre?_.

_VSlices Method_ usa el cambio de modalidad para mantener al equipo alineado con la realidad, en vez de forzar que el trabajo continúe bajo el énfasis incorrecto.

## Por qué importa cambiar de modalidad

Cada modalidad protege al equipo de un riesgo distinto.

| Modalidad         | Ayuda a evitar                                         | Puede volverse riesgosa cuando                                                         |
| ----------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------------- |
| **_Context-First_** | Construir desde un contexto<br/>mal entendido.             | El equipo sigue expandiendo entendimiento sin<br/>decidir qué validar.                     |
| **_Problem-First_** | Resolver síntomas en vez de<br/>problemas.                 | El equipo aísla el problema del contexto más amplio<br/>que le da significado.             |
| **_Slice-First_**   | Diseñar demasiado antes de<br/>aprender desde la realidad. | El equipo construye sin suficiente entendimiento de<br/>intención, riesgo o consecuencias. |

Cambiar de modalidad ayuda a evitar que un énfasis útil se convierta en complejidad accidental.

## Cambios comunes

Un cambio no significa que la modalidad anterior estuviera mal. Significa que la modalidad anterior produjo suficiente aprendizaje como para que el trabajo necesite un énfasis distinto.

| Cambio                             | Usar cuando                                                                                                      | Propósito                                                                 |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| **_Context-First_ -> _Problem-First_** | El equipo entiende suficiente del<br/>escenario como para enfocarse en<br/>un dolor, oportunidad o decisión<br/>concreta.    | Estrechar un contexto amplio<br/>hacia un problema que vale la<br/>pena resolver. |
| **_Context-First_ -> _Slice-First_**   | El equipo entiende lo suficiente<br/>como para validar una parte<br/>pequeña y reversible del sistema.                   | Convertir aprendizaje<br/>contextual en evidencia<br/>práctica.                   |
| **_Problem-First_ -> _Context-First_** | El problema depende de _workflows_,<br/>actores, lenguaje o restricciones<br/>circundantes que todavía no están<br/>claros.    | Recuperar el contexto<br/>necesario para evitar<br/>optimización local.           |
| **_Problem-First_ -> _Slice-First_**   | El problema está lo suficientemente<br/>claro como para que una entrega<br/>pequeña pueda probar la mejora<br/>esperada.     | Validar si la dirección<br/>propuesta funciona en la<br/>realidad.                |
| **_Slice-First_ -> _Problem-First_**   | Una _slice_ construida revela que<br/>el problema original estaba<br/>incompleto, mal ubicado o mal<br/>enmarcado.             | Reencuadrar el problema<br/>usando evidencia de la<br/>entrega.                   |
| **_Slice-First_ -> _Context-First_**   | Construir revela contexto de<br/>dominio faltante, actores ocultos,<br/>límites poco claros o consecuencias<br/>inesperadas. | Reconstruir entendimiento<br/>antes de continuar la<br/>implementación.           |

## Señales de que puede necesitarse un cambio

Un equipo debería considerar cambiar de modalidad cuando el modo actual deja de ayudar. Señales comunes incluyen:

* aparecen nuevos conceptos de dominio durante la implementación
* el equipo sigue debatiendo sin aprender nada nuevo
* una _slice_ pequeña funciona técnicamente, pero no mejora la situación real
* un problema parece claro, pero depende de workflows que nadie entiende
* la documentación sigue expandiéndose, pero ninguna decisión se vuelve más segura
* el _feedback_ de entrega contradice un supuesto
* la misma pregunta vuelve a aparecer en distintas etapas
* el equipo no puede explicar por qué el trabajo actual importa

Estas señales no requieren automáticamente un cambio. Indican que el equipo debería reevaluar la incertidumbre dominante.

## Cambiar sin ceremonia

El cambio de modalidad debería ser ligero.

* Un equipo no necesita reiniciar la iteración.
* Un equipo solo necesita reconocer qué cambió.

Preguntas útiles incluyen:

* ¿Qué aprendimos?
* ¿Qué incertidumbre es dominante ahora?
* ¿Nuestra modalidad actual todavía está ayudando?
* ¿Cuál es el siguiente movimiento más pequeño que reduce esta incertidumbre?
* ¿Qué conocimiento debería preservarse antes de avanzar?

El cambio puede ser tan simple como cambiar la siguiente conversación, actualizar un documento, acotar la siguiente _slice_ o reabrir una decisión.

## Soporte documental

Los documentos pueden ayudar a preservar por qué cambió una modalidad. Usa documentación solo cuando el cambio afecta trabajo futuro.

* **_Support Notes_** pueden preservar observaciones tempranas o incertidumbre.
* **_Validation Notes_** pueden preservar evidencia que causó el cambio.
* **_Decision Records_** pueden preservar cambios importantes de dirección.
* **_Context Documents_** pueden preservar nuevo contexto circundante descubierto.
* **_Use Case Documents_** pueden preservar comportamiento aclarado después del cambio.
* **_Process Documents_** pueden preservar conocimiento de workflow revelado por el cambio.

El objetivo no es documentar cada cambio. Es evitar perder el aprendizaje que hizo necesario el cambio.

## Errores comunes

_Modality Switching_ puede fallar cuando el equipo trata las modalidades como etapas de proceso.

* Cambiar demasiado seguido puede impedir profundidad útil.
* Rehusarse a cambiar puede mantener al equipo resolviendo la incertidumbre equivocada.
* Cambiar sin preservar aprendizaje puede hacer que el equipo repita la misma confusión.
* Tratar los cambios como fallas puede desalentar el feedback.
* Tratar los cambios como etapas obligatorias puede crear ceremonia innecesaria.

Un cambio es útil cuando hace más segura la siguiente decisión.

## Principio guía

Deja que la incertidumbre actual elija la modalidad. Cuando la incertidumbre cambie, cambia el énfasis.

El método debería seguir el aprendizaje. No debería forzarse el trabajo para que calce con el método.
