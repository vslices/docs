# Cambio de modalidad

El cambio de modalidad explica cuándo y por qué un equipo puede pasar de una modalidad de VSlices Design a otra.

Una modalidad no es una etiqueta permanente para una iteración. Es un énfasis que ayuda al equipo a reducir la incertidumbre que más importa ahora.

Cuando la incertidumbre cambia, la modalidad también puede necesitar cambiar.

## Idea central

Cambia de modalidad cuando la modalidad actual ya no está reduciendo la incertidumbre dominante.

La pregunta no es: _¿Tenemos permitido cambiar de modalidad?_

La pregunta es: _¿Cambió el tipo de incertidumbre?_

VSlices Method usa el cambio de modalidad para mantener al equipo alineado con la realidad, en vez de forzar que el trabajo continúe bajo el énfasis equivocado.

## Por qué importa cambiar

Cada modalidad protege al equipo de un riesgo distinto.

| Modalidad | Ayuda a evitar | Puede volverse riesgosa cuando |
| --- | --- | --- |
| __[Context-First](../../design/modalities/context-first/index.md)__ | Construir desde un contexto mal entendido. | El equipo sigue expandiendo entendimiento sin decidir qué validar. |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ | Resolver síntomas en vez de problemas. | El equipo aísla el problema del contexto más amplio que le da significado. |
| __[Slice-First](../../design/modalities/slice-first/index.md)__ | Diseñar demasiado antes de aprender desde la realidad. | El equipo construye sin suficiente entendimiento de intención, riesgo o consecuencias. |

Cambiar de modalidad ayuda a evitar que un énfasis útil se convierta en complejidad accidental.

## Cambios comunes

Un cambio no significa que la modalidad anterior estaba mal. Significa que la modalidad anterior produjo suficiente aprendizaje como para que el trabajo necesite un énfasis diferente.

| Cambio | Usar cuando | Propósito |
| --- | --- | --- |
| __[Context-First](../../design/modalities/context-first/index.md)__ -> __[Problem-First](../../design/modalities/problem-first/index.md)__ | El equipo entiende suficiente del escenario como para enfocarse en un dolor, oportunidad o decisión concreta. | Acotar el contexto amplio hacia un problema que vale la pena resolver. |
| __[Context-First](../../design/modalities/context-first/index.md)__ -> __[Slice-First](../../design/modalities/slice-first/index.md)__ | El equipo entiende suficiente como para validar una parte pequeña y reversible del sistema. | Convertir aprendizaje contextual en evidencia práctica. |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ -> __[Context-First](../../design/modalities/context-first/index.md)__ | El problema depende de workflows, actores, lenguaje o restricciones circundantes que todavía no están claros. | Recuperar el contexto necesario para evitar optimización local. |
| __[Problem-First](../../design/modalities/problem-first/index.md)__ -> __[Slice-First](../../design/modalities/slice-first/index.md)__ | El problema está lo suficientemente claro como para que una entrega pequeña pruebe la mejora esperada. | Validar si la dirección propuesta funciona en la realidad. |
| __[Slice-First](../../design/modalities/slice-first/index.md)__ -> __[Problem-First](../../design/modalities/problem-first/index.md)__ | Una slice construida revela que el problema original estaba incompleto, mal ubicado o mal formulado. | Reformular el problema usando evidencia de la entrega. |
| __[Slice-First](../../design/modalities/slice-first/index.md)__ -> __[Context-First](../../design/modalities/context-first/index.md)__ | Construir revela contexto de dominio faltante, actores ocultos, límites poco claros o consecuencias inesperadas. | Reconstruir entendimiento antes de continuar con la implementación. |

## Señales de que puede hacer falta cambiar

Un equipo debería considerar cambiar de modalidad cuando el modo actual deja de ayudar. Algunas señales comunes incluyen:

* aparecen nuevos conceptos del dominio durante la implementación
* el equipo sigue debatiendo sin aprender nada nuevo
* una slice pequeña funciona técnicamente pero no mejora la situación real
* un problema parece claro pero depende de workflows que nadie entiende
* la documentación sigue expandiéndose pero ninguna decisión se vuelve más segura
* el feedback de entrega contradice un supuesto
* la misma pregunta vuelve una y otra vez entre etapas
* el equipo no puede explicar por qué importa el trabajo actual

Estas señales no requieren automáticamente un cambio. Indican que el equipo debería reevaluar la incertidumbre dominante.

## Cambiar sin ceremonia

El cambio de modalidad debería ser liviano.

- Un equipo no necesita reiniciar la iteración.
- Un equipo solo necesita reconocer qué cambió.

Algunas preguntas útiles son:

* ¿Qué aprendimos?
* ¿Qué incertidumbre domina ahora?
* ¿La modalidad actual sigue ayudando?
* ¿Cuál es el siguiente movimiento más pequeño que reduce esta incertidumbre?
* ¿Qué conocimiento debería preservarse antes de avanzar?

El cambio puede ser tan simple como cambiar la siguiente conversación, actualizar un documento, acotar la siguiente slice o reabrir una decisión.

## Apoyo documental

Los documentos pueden ayudar a preservar por qué cambió una modalidad. Usa documentación solo cuando el cambio afecte trabajo futuro.

* **[Support Notes](../../docs-standard/taxonomy/support-note.md)** pueden preservar observaciones tempranas o incertidumbre.
* **[Validation Notes](../../docs-standard/taxonomy/validation-note.md)** pueden preservar evidencia que causó el cambio.
* **[Decision Records](../../docs-standard/taxonomy/decision-record.md)** pueden preservar cambios importantes de dirección.
* **[Context Documents](../../docs-standard/taxonomy/context-document.md)** pueden preservar nuevo contexto circundante descubierto.
* **[Use Case Documents](../../docs-standard/taxonomy/use-case-document.md)** pueden preservar comportamiento aclarado después del cambio.
* **[Process Documents](../../docs-standard/taxonomy/process-document.md)** pueden preservar conocimiento de workflow revelado por el cambio.

El objetivo no es documentar cada cambio. Es evitar perder el aprendizaje que hizo necesario el cambio.

## Errores comunes

El cambio de modalidad puede fallar cuando el equipo trata las modalidades como etapas de proceso.

* Cambiar demasiado seguido puede impedir profundidad útil.
* Negarse a cambiar puede mantener al equipo resolviendo la incertidumbre equivocada.
* Cambiar sin preservar aprendizaje puede hacer que el equipo repita la misma confusión.
* Tratar los cambios como fallas puede desincentivar el feedback.
* Tratar los cambios como etapas obligatorias puede crear ceremonia innecesaria.

Un cambio es útil cuando vuelve más segura la siguiente decisión.

## Principio guía

Deja que la incertidumbre actual elija la modalidad. Cuando la incertidumbre cambia, cambia el énfasis.

El método debería seguir el aprendizaje. No debería forzarse el aprendizaje para que encaje en el método.
