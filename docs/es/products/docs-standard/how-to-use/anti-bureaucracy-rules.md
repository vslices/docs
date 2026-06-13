# Reglas contra la burocracia

VSlices Docs Standard debería ayudar a los equipos a preservar conocimiento útil sin convertir la documentación en ceremonia.

> Un documento es valioso cuando apoya el entendimiento, las decisiones, la implementación, la validación o la evolución.
>
> Un documento es desperdicio cuando existe solo porque un proceso, plantilla o estándar lo hizo parecer obligatorio.

## Regla 1: Ningún documento es obligatorio por defecto

VSlices Docs Standard define estructuras de documento disponibles.

No exige que cada equipo cree cada documento. Un documento debe crearse solo cuando ayuda a preservar conocimiento del que depende el trabajo actual o futuro.

El equipo debería preguntar:

- ¿Qué conocimiento preserva este documento?
- ¿Qué decisión apoya?
- ¿Qué riesgo reduce?
- ¿Qué confusión previene?
- ¿Quién lo usará después?

Si esas preguntas no revelan suficiente valor, el documento quizá no sea necesario.

## Regla 2: Usa la versión más pequeña útil

La versión por defecto de un documento debería ser la versión más pequeña que siga ayudando.

Un documento corto que preserva el conocimiento correcto es mejor que un documento largo que repite información obvia.

El equipo debería preferir:

- __nota antes que documento__: captura conocimiento temprano de forma ligera antes de darle estructura formal.
- __mínimo antes que ampliado__: empieza con la versión de documento más pequeña útil.
- __específico antes que genérico__: preserva conocimiento concreto antes de escribir explicaciones amplias.
- __útil antes que completo__: llena lo que importa, no todas las secciones posibles.

Un documento debería crecer porque el dominio lo requiere, no porque la plantilla lo permita.

## Regla 3: No confundas volumen con entendimiento

Más documentación no significa mejor entendimiento.

> Un equipo puede producir muchos documentos y aun así no entender el dominio.
>
> Un equipo también puede preservar un entendimiento sólido con un pequeño conjunto de documentos enfocados.

La calidad de la documentación depende de si ayuda al equipo a explicar:

- qué está pasando.
- por qué importa.
- qué decisión se tomó.
- qué conocimiento respalda esa decisión.
- qué incertidumbre permanece.
- qué cambió después de la implementación.

La documentación debe crear claridad, no ruido.

## Regla 4: No documentes más allá de lo que se sabe

Un documento no debe fingir que el equipo sabe más de lo que realmente sabe.

Lo desconocido, los supuestos, los riesgos y las preguntas abiertas deben permanecer visibles. El equipo debería preferir incertidumbre honesta antes que precisión falsa. Ejemplos:

- __known__: esto fue validado con expertos del dominio u observado en el sistema.
- __assumed__: esto parece verdadero, pero todavía necesita validación.
- __unclear__: esto todavía no se entiende lo suficiente.
- __invalidated__: esto se creía antes, pero la evidencia posterior lo refutó.

La certeza falsa es más peligrosa que un documento incompleto.

## Regla 5: Evita la completitud falsa

Un documento que parece completo no siempre es útil; puede contener muchas secciones y aun así no preservar el conocimiento importante.

El equipo no debería llenar secciones con texto débil solo para que el documento parezca completo. Usa marcas simples cuando sea necesario:

- __unknown__: el equipo aún no sabe esto.
- __not applicable__: esta sección no importa para este caso.
- __deferred__: esto puede importar después, pero no ahora.
- __superseded__: esto fue reemplazado por conocimiento más nuevo.

Un documento útil no es el que tiene todas las secciones llenas. Es el que preserva el conocimiento del que depende el trabajo futuro.

## Regla 6: Mantén los documentos cerca de las decisiones

La documentación no debería alejarse de las decisiones que apoya.

- Cuando un documento influye en una decisión, esa relación debería ser visible.
- Cuando una decisión afecta la implementación, esa relación debería ser visible.
- Cuando la implementación produce aprendizaje, ese aprendizaje debería volver a la documentación.

Las referencias simples son suficientes:

```text
Contexto relacionado:
- context.order-fulfillment

Decisión relacionada:
- decision.payment-validation-boundary

Validación relacionada:
- validation.payment-rules-feedback
```

El objetivo es trazabilidad sin un proceso pesado.

## Regla 7: Trata la documentación obsoleta como un riesgo

La documentación desactualizada puede crear falsa confianza. Un documento que ya no refleja la realidad no debería seguir activo silenciosamente.

El equipo debería actualizarlo, reemplazarlo o archivarlo. Estados sugeridos:

- __draft__: el documento todavía se está moldeando.
- __active__: el documento actualmente representa conocimiento compartido útil.
- __superseded__: el documento fue reemplazado por conocimiento más nuevo.
- __archived__: el documento ya no está activo, pero sigue siendo útil como historia.

Un documento no necesita vivir para siempre.

## Regla 8: Divide solo cuando mejore la claridad

> Un documento debería dividirse cuando la división mejore la claridad, la reutilización, la propiedad o la trazabilidad.
>
> Un documento no debería dividirse solo porque el estándar tiene muchos tipos de documento posibles.

El equipo debería dividir cuando:

- un documento mezcla conocimiento no relacionado.
- distintas partes evolucionan a distintas velocidades.
- distintas personas son propietarias de distintas partes.
- el documento es demasiado grande para mantenerse con seguridad.
- la misma sección se reutiliza en varios documentos.

Si dividir hace que la documentación sea más difícil de entender, mantenla unida.

## Regla 9: La documentación debe justificar su costo

La documentación tiene un costo. Toma tiempo crearla, leerla, revisarla y mantenerla.

Ese costo es aceptable cuando el documento reduce más costo futuro del que introduce. El equipo debería preguntar:

- ¿Qué pasa si no escribimos esto?
- ¿Qué pasa si alguien lo malinterpreta después?
- ¿Qué pasa si este documento se vuelve obsoleto?
- ¿Una nota de soporte es suficiente por ahora?
- ¿El documento nos ayuda a avanzar?

La documentación debe apoyar el juicio de ingeniería. No debe reemplazarlo.

## Resumen

VSlices Docs Standard sigue un principio simple contra la burocracia:

> Crea la documentación más pequeña útil que preserve el conocimiento del que depende el trabajo futuro.

La documentación debería hacer que el trabajo de software sea más seguro, más claro y más conectado. Cuando la documentación deja de hacer eso, se ha convertido en ceremonia.
