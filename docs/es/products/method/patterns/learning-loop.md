# Ciclo de aprendizaje

El Ciclo de aprendizaje explica cómo el feedback del trabajo real vuelve al entendimiento. En VSlices Method, construir algo no es el final de una iteración. Construir crea evidencia.

Esa evidencia puede confirmar la dirección actual, refinar el contexto, cuestionar una decisión o revelar una nueva línea de trabajo.

## Idea central

Una iteración de VSlices Method sigue el flujo compartido de VSlices Design:

{% include-markdown "shared/simple-design-iteration-flow.md" %}

El retorno final a Understanding es intencional.

Un equipo no vuelve a Understanding porque la iteración falló. Un equipo vuelve porque construir, validar y usar software cambia lo que se sabe.

El resultado de una iteración no debería ser solo software funcionando. También debería ser mejor entendimiento.

## Qué puede generar aprendizaje

El aprendizaje puede venir de distintas fuentes.

* implementación, cuando las restricciones técnicas revelan supuestos ocultos
* revisión, cuando el comportamiento esperado se cuestiona
* pruebas, cuando errores esperados o casos borde se vuelven visibles
* uso, cuando las personas interactúan con el sistema de forma distinta a la esperada
* operación, cuando el comportamiento en producción expone nuevos riesgos
* soporte, cuando problemas repetidos revelan workflows o conceptos poco claros
* feedback de negocio, cuando el comportamiento entregado cambia prioridades

Lo importante no es de dónde viene el feedback. Lo importante es si cambia lo que el equipo debería entender, preservar o hacer después.

## Resultados del aprendizaje

Después de Building, el feedback puede producir distintos resultados.

* **Confirmado** significa que la evidencia sostiene el entendimiento o la decisión actual.
* **Refinado** significa que la dirección fue útil, pero algunos detalles necesitan ajuste.
* **Cuestionado** significa que la evidencia contradice un supuesto, decisión o modelo.
* **Dividido** significa que el feedback revela una work line o preocupación separada.
* **Reemplazado** significa que el conocimiento anterior ya no representa la realidad actual.

Cada resultado debería influir en lo que ocurre después.

- Un resultado confirmado puede permitir que el equipo continúe.
- Un resultado refinado puede actualizar un documento o detalle de implementación.
- Un resultado cuestionado puede requerir volver a Planning o Contextualizing.
- Un resultado dividido puede abrir una nueva Work Line.
- Un resultado reemplazado puede requerir actualizar o sustituir conocimiento previo.

## Qué debería preservarse

El Ciclo de aprendizaje no requiere que cada señal de feedback se convierta en documentación. Preserva feedback cuando afecte trabajo futuro.

El conocimiento útil a preservar puede incluir:

* una decisión que fue confirmada o cuestionada
* un comportamiento que funcionó distinto a lo esperado
* un error esperado que faltaba
* una excepción de workflow que se volvió visible
* un término del dominio cuyo significado cambió
* una restricción técnica que afecta el diseño
* un nuevo riesgo descubierto durante implementación u operación
* una posible nueva Work Line

El objetivo no es registrarlo todo. Es evitar redescubrir el mismo aprendizaje más adelante.

## Apoyo documental

Distintos documentos pueden apoyar el Ciclo de aprendizaje.

* **[Validation Notes](../../docs-standard/taxonomy/validation-note.md)** preservan evidencia y aprendizaje.
* **[Decision Records](../../docs-standard/taxonomy/decision-record.md)** preservan decisiones que fueron confirmadas, cuestionadas o cambiadas.
* **[Use Case Documents](../../docs-standard/taxonomy/use-case-document.md)** preservan comportamiento que se volvió más claro después de construir.
* **[Capability Documents](../../docs-standard/taxonomy/capability-document.md)** preservan habilidades estables reveladas o refinadas por la iteración.
* **[Context Documents](../../docs-standard/taxonomy/context-document.md)** preservan cambios en el escenario circundante.
* **[Process Documents](../../docs-standard/taxonomy/process-document.md)** preservan cambios de workflow, excepciones o handoffs.
* **[Support Notes](../../docs-standard/taxonomy/support-note.md)** preservan observaciones inciertas o locales que todavía no están maduras.

Usa el documento más liviano que preserve el aprendizaje del que depende el trabajo futuro.

## Decidir el siguiente movimiento

Después de reunir aprendizaje, el equipo debería decidir cuál es el siguiente movimiento responsable. Algunos movimientos posibles incluyen:

* continuar con la dirección actual
* actualizar documentación existente
* registrar una Validation Note
* revisar un Decision Record
* refinar el Use Case o Capability actual
* volver a Contextualizing
* volver a Planning
* cambiar de modalidad de diseño
* abrir una nueva Work Line
* detener la iteración porque ya se entregó suficiente valor

El siguiente movimiento debería basarse en lo que la evidencia cambió.

## Riesgos comunes

Los ciclos de aprendizaje pueden romperse de varias formas.

* **Feedback sin preservación**: hace que los equipos repitan los mismos descubrimientos.
* **Validación sin decisiones**: crea observaciones que nunca afectan la dirección.
* **Implementación sin reflexión**: trata la construcción como finalización en vez de aprendizaje.
* **Documentación sin actualización**: deja activo conocimiento obsoleto.
* **Éxito sin revisión**: pierde lo que debería reutilizarse o fortalecerse.
* **Falla sin aprendizaje**: convierte la evidencia en culpa en vez de entendimiento.

El Ciclo de aprendizaje existe para hacer útil el feedback antes de que desaparezca.

## Principio guía

La realidad es parte del método.

Usa el feedback para mejorar el entendimiento compartido del trabajo. Preserva solo el aprendizaje del que futuras decisiones, documentación, diseño o implementación puedan depender.
