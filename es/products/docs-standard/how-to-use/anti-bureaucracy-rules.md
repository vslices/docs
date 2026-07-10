# Reglas anti burocracia

VSlices Docs Standard debería ayudar a los equipos a preservar conocimiento útil sin convertir la documentación en ceremonia.

Un documento es valioso cuando apoya el entendimiento, las decisiones, la implementación, la validación o la evolución.

Un documento se convierte en desperdicio cuando existe solo porque un proceso, plantilla o estándar lo hizo parecer obligatorio.

!!! principle "Principio de Documentación"

    Crea la documentación más pequeña útil que preserve el conocimiento del que depende el trabajo futuro.


## Regla 1: Ningún documento es obligatorio por defecto

VSlices Docs Standard define estructuras de documento disponibles.

No exige que cada equipo cree cada documento. Un documento debe crearse solo cuando ayuda a preservar conocimiento del que depende el trabajo actual o futuro.

Antes de crear un documento, el equipo debería preguntar:

* ¿Qué conocimiento preserva este documento?
* ¿Qué decisión apoya?
* ¿Qué riesgo reduce?
* ¿Qué confusión previene?
* ¿Quién lo usará después?

Si esas preguntas no revelan suficiente valor, el documento quizá no sea necesario.

## Regla 2: Usa la versión más pequeña útil

La versión por defecto de un documento debería ser la versión más pequeña que siga ayudando.

Un documento corto que preserva el conocimiento correcto es mejor que un documento largo que repite información obvia.

| Prefiere...             | Antes que...                       |
| ----------------------- | ---------------------------------- |
| Nota                    | Documento formal prematuro         |
| Documento mínimo        | Documento ampliado                 |
| Conocimiento específico | Explicación genérica               |
| Contenido útil          | Secciones completas sin valor real |

Un documento debería crecer porque el dominio lo requiere, no porque la plantilla lo permita.

## Regla 3: No confundas volumen con entendimiento

Más documentación no significa mejor entendimiento.

Un equipo puede producir muchos documentos y aun así no entender el dominio.

También puede preservar un entendimiento sólido con un pequeño conjunto de documentos enfocados.

La calidad de la documentación depende de si ayuda al equipo a explicar:

* qué está pasando
* por qué importa
* qué decisión se tomó
* qué conocimiento respalda esa decisión
* qué incertidumbre permanece
* qué cambió después de la implementación

!!! risk "Riesgo a evitar"

    La documentación debe crear claridad, no ruido.


## Regla 4: No documentes más allá de lo que se sabe

Un documento no debe fingir que el equipo sabe más de lo que realmente sabe.

Lo desconocido, los supuestos, los riesgos y las preguntas abiertas deben permanecer visibles.

| Marca         | Significado                                                      |
| ------------- | ---------------------------------------------------------------- |
| known       | Fue validado con expertos del dominio u observado en el sistema. |
| assumed     | Parece verdadero, pero todavía necesita validación.              |
| unclear     | Todavía no se entiende lo suficiente.                            |
| invalidated | Se creía antes, pero evidencia posterior lo refutó.              |

!!! risk "Riesgo a evitar"

    La certeza falsa es más peligrosa que un documento incompleto.


## Regla 5: Evita la completitud falsa

Un documento que parece completo no siempre es útil.

Puede contener muchas secciones y aun así no preservar el conocimiento importante.

El equipo no debería llenar secciones con texto débil solo para que el documento parezca completo.

| Marca            | Significado                                      |
| ---------------- | ------------------------------------------------ |
| unknown        | El equipo aún no sabe esto.                      |
| not applicable | Esta sección no importa para este caso.          |
| deferred       | Esto puede importar después, pero no ahora.      |
| superseded     | Esto fue reemplazado por conocimiento más nuevo. |

Un documento útil no es el que tiene todas las secciones llenas. Es el que preserva el conocimiento del que depende el trabajo futuro.

## Regla 6: Mantén los documentos cerca de las decisiones

La documentación no debería alejarse de las decisiones que apoya.

* Cuando un documento influye en una decisión, esa relación debería ser visible.
* Cuando una decisión afecta la implementación, esa relación debería ser visible.
* Cuando la implementación produce aprendizaje, ese aprendizaje debería volver a la documentación.

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

La documentación desactualizada puede crear falsa confianza.

Un documento que ya no refleja la realidad no debería seguir activo silenciosamente.

| Estado       | Significado                                                           |
| ------------ | --------------------------------------------------------------------- |
| draft      | El documento todavía se está moldeando.                               |
| active     | El documento representa conocimiento compartido útil.                 |
| superseded | El documento fue reemplazado por conocimiento más nuevo.              |
| archived   | El documento ya no está activo, pero sigue siendo útil como historia. |

Un documento no necesita vivir para siempre.

## Regla 8: Divide solo cuando mejore la claridad

Un documento debería dividirse cuando la división mejore la claridad, la reutilización, la propiedad o la trazabilidad.

No debería dividirse solo porque el estándar tiene muchos tipos de documento posibles.

El equipo debería dividir cuando:

* un documento mezcla conocimiento no relacionado
* distintas partes evolucionan a distintas velocidades
* distintas personas son propietarias de distintas partes
* el documento es demasiado grande para mantenerse con seguridad
* la misma sección se reutiliza en varios documentos

Si dividir hace que la documentación sea más difícil de entender, mantenla unida.

## Regla 9: La documentación debe justificar su costo

La documentación tiene un costo.

Toma tiempo crearla, leerla, revisarla y mantenerla.

Ese costo es aceptable cuando el documento reduce más costo futuro del que introduce.

El equipo debería preguntar:

* ¿Qué pasa si no escribimos esto?
* ¿Qué pasa si alguien lo malinterpreta después?
* ¿Qué pasa si este documento se vuelve obsoleto?
* ¿Una nota de soporte es suficiente por ahora?
* ¿El documento nos ayuda a avanzar?

La documentación debe apoyar el juicio de ingeniería. No debe reemplazarlo.

## Resumen

La documentación debería hacer que el trabajo de software sea más seguro, más claro y más conectado.

Cuando deja de hacer eso, se ha convertido en ceremonia.

!!! principle "Principio de Documentación"

    Crea la documentación más pequeña útil que preserve el conocimiento del que depende el trabajo futuro.
