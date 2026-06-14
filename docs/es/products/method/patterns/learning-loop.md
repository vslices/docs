# Bucle de Aprendizaje

El Bucle de Aprendizaje (_Learning Loop_ en ingles) explica cómo el _feedback_ del trabajo real vuelve al entendimiento. En _VSlices Method_, construir algo no es el final de una iteración. Construir crea evidencia.

Esa evidencia puede confirmar la dirección actual, refinar el contexto, desafiar una decisión o revelar una nueva línea de trabajo.

## Idea central

Una iteración de _VSlices Method_ sigue el flujo compartido de _VSlices Design_:

```text
_Understanding_
-> _Contextualizing_
-> _Planning_
-> _Building_
-> _Understanding_
```

El retorno final a _Understanding_ es intencional.

Un equipo no vuelve a _Understanding_ porque la iteración falló. Un equipo vuelve porque construir, validar y usar software cambia lo que se sabe.

El resultado de una iteración no debería ser solo software funcionando. También debería ser mejor entendimiento.

## Qué puede crear aprendizaje

El aprendizaje puede venir de distintas fuentes.

* implementación, cuando las restricciones técnicas revelan supuestos ocultos
* revisión, cuando el comportamiento esperado es cuestionado
* testing, cuando los errores esperados o casos borde se vuelven visibles
* uso, cuando las personas interactúan con el sistema de forma distinta a la esperada
* operación, cuando el comportamiento en producción expone nuevos riesgos
* soporte, cuando problemas repetidos revelan workflows o conceptos poco claros
* _feedback_ de negocio, cuando el comportamiento entregado cambia prioridades

Lo importante no es de dónde viene el _feedback_. Lo importante es si cambia lo que el equipo debería entender, preservar o hacer después.

## Resultados de aprendizaje

Después de _Building_, el _feedback_ puede producir distintos resultados.

* **Confirmado** significa que la evidencia sostiene el entendimiento o decisión actual.
* **Refinado** significa que la dirección fue útil, pero algunos detalles necesitan ajuste.
* **Desafiado** significa que la evidencia contradice un supuesto, decisión o modelo.
* **Segmentado** significa que el feedback revela una Work Line o preocupación separada.
* **Superado** significa que el conocimiento previo ya no representa suficientemente la realidad actual.

Cada resultado debería influir en lo que ocurre después.

* Un resultado __confirmado__ puede permitir que el equipo continúe.
* Un resultado __refinado__ puede actualizar un documento o detalle de implementación.
* Un resultado __desafiado__ puede requerir volver a _Planning_ o _Contextualizing_.
* Un resultado __segmentado__ puede abrir una nueva _Work Line_.
* Un resultado __superado__ puede requerir actualizar o reemplazar conocimiento previo.

## Qué debería preservarse

El _Learning Loop_ no requiere que cada señal de _feedback_ se convierta en documentación. Preserva feedback cuando afecta el trabajo futuro.

El conocimiento útil a preservar puede incluir:

* una decisión que fue confirmada o desafiada
* un comportamiento que funcionó de forma distinta a la esperada
* un error esperado que faltaba
* una excepción de workflow que se volvió visible
* un término de dominio cuyo significado cambió
* una restricción técnica que afecta el diseño
* un nuevo riesgo descubierto durante la implementación u operación
* una posible nueva _Work Line_

El objetivo no es registrarlo todo. Es evitar redescubrir el mismo aprendizaje más adelante.

## Soporte documental

Distintos documentos pueden apoyar el _Learning Loop_.

* **_Validation Notes_** preservan evidencia y aprendizaje.
* **_Decision Records_** preservan decisiones que fueron confirmadas, desafiadas o cambiadas.
* **_Use Case Documents_** preservan comportamiento que se volvió más claro después de construir.
* **_Capability Documents_** preservan capacidades estables reveladas o refinadas por la iteración.
* **_Context Documents_** preservan cambios en el escenario circundante.
* **_Process Documents_** preservan cambios de _workflow_, excepciones o _handoffs_.
* **_Support Notes_** preservan observaciones inciertas o locales que todavía no están maduras.

Usa el documento más ligero que preserve el aprendizaje del que depende el trabajo futuro.

## Decidir el siguiente movimiento

Después de reunir aprendizaje, el equipo debería decidir cuál es el siguiente movimiento responsable. Los movimientos posibles incluyen:

* continuar la dirección actual
* actualizar documentación existente
* registrar una _Validation Note_
* revisar un _Decision Record_
* refinar el _Use Case_ o _Capability_ actual
* volver a _Contextualizing_
* volver a _Planning_
* cambiar de modalidad de diseño
* abrir una nueva _Work Line_
* detener la iteración porque ya se entregó suficiente valor

El siguiente movimiento debería basarse en lo que la evidencia cambió.

## Riesgos comunes

Los loops de aprendizaje pueden romperse de varias formas.

* **_Feedback_ sin preservación** hace que los equipos repitan los mismos descubrimientos.
* **Validación sin decisiones** crea observaciones que nunca afectan la dirección.
* **Implementación sin reflexión** trata construir como finalización en vez de aprendizaje.
* **Documentación sin actualización** deja activo conocimiento obsoleto.
* **Éxito sin revisión** omite lo que debería reutilizarse o fortalecerse.
* **Fallo sin aprendizaje** convierte la evidencia en culpa en vez de entendimiento.

El _Learning Loop_ existe para hacer que el feedback sea útil antes de que desaparezca.

## Principio guía

La realidad es parte del método.

Usa el _feedback_ para mejorar el entendimiento compartido del trabajo. Preserva solo el aprendizaje del que podrían depender decisiones, documentación, diseño o implementación futuros.
