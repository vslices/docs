# Camino de continuidad "Motivación de negocio" de <tema>

## Propósito del recorrido

<!--
¿Para qué necesitamos recorrer este path?

Explicar qué continuidad de negocio se busca preservar.
No explicar todavía el contexto completo del negocio; eso pertenece a un Documento de Contexto.
-->

Este path busca preservar continuidad entre `<tema>` y la situación de negocio que lo origina, justifica o afecta.

Ayuda a evitar que el concepto se entienda solo como una solución, artifact, decisión técnica o comportamiento aislado, perdiendo la necesidad, dolor, oportunidad, restricción o consecuencia de negocio que le da sentido.

## Punto de entrada

<!--
¿Por dónde empieza este camino?

Indicar el concepto, necesidad, dolor, oportunidad, decisión, iniciativa o situación de negocio desde donde parte el recorrido.
-->

## Diagrama de continuidad

<!--
¿Qué mapa vamos a recorrer?

Incluir el Diagrama de Camino de Continuidad asociado al Business Driver.
El diagrama debe mostrar preguntas de orientación, conceptos relacionados y estado documental de los conceptos conectados.
-->

```mermaid
flowchart LR
    CR[["<b>Business Driver</b><br/>[Motivación de negocio]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Business Driver Path</a></small>"]]

    CR --> P1["¿Qué situación de negocio lo origina?"]
    CR --> P2["¿Qué dolor, necesidad u oportunidad intenta responder?"]
    CR --> P3["¿Qué consecuencia aparece si no se atiende?"]
    CR --> P4["¿Qué restricción condiciona la respuesta?"]
    CR --> P5["¿Qué decisión o iniciativa se justifica por esto?"]

    P1 --> S1[["<b>Business Scenario</b><br/>[Escenario observado]<br/><small><a href='link'>Context Document</a><br/><a href='link'>Business Scenario Path</a></small>"]]

    P2 --> N1{{"<b>Business Need</b><br/>[Necesidad, dolor u oportunidad]<br/><small>Context Document<br/>Scope Document</small>"}}

    P3 --> C1>"<b>Business Consequence</b><br/>[Consecuencia identificada]"]
    P3 --> C2{{"<b>Relevant Consequence</b><br/>[Consecuencia que condiciona prioridad]<br/><small>Viability Document<br/>Decision Record</small>"}}

    P4 --> R1>"<b>Business Constraint</b><br/>[Restricción identificada]"]
    P4 --> R2{{"<b>Viability Constraint</b><br/>[Restricción que condiciona viabilidad]<br/><small>Viability Document</small>"}}

    P5 --> D1[["<b>Decision</b><br/>[Decisión relacionada]<br/><small><a href='link'>Decision Record</a></small>"]]
    P5 --> I1[["<b>Software Initiative</b><br/>[Iniciativa relacionada]<br/><small><a href='link'>Software Initiative Path</a></small>"]]

    C2 -.-> P5
    R2 -.-> P5
```

## Recorrido recomendado

<!--
¿Qué ruta conviene seguir primero?

Describir el recorrido principal recomendado para entender el path sin duplicar el contenido de los artifacts conectados.
-->

| Orden | Nodo, artifact o concepto         | Por qué revisarlo                                                         |
| ----- | --------------------------------- | ------------------------------------------------------------------------- |
| 1     | Motivación de negocio             | Permite identificar qué estamos siguiendo y por qué podría importar       |
| 2     | Situación de negocio              | Permite entender dónde aparece la motivación                              |
| 3     | Dolor, necesidad u oportunidad    | Permite entender qué empuja a intervenir                                  |
| 4     | Consecuencia de negocio           | Permite entender qué se pierde, empeora o queda expuesto si no se atiende |
| 5     | Restricción de negocio            | Permite entender qué limita o condiciona la respuesta posible             |
| 6     | Decisión o iniciativa relacionada | Permite entender qué respuesta se justifica desde esta motivación         |

## Consecuencias y restricciones

<!--
¿Cómo deben interpretarse consecuencias y restricciones dentro de este path?

Usar esta sección para distinguir qué se identifica, qué requiere evaluación y qué debe conectarse con otros artifacts.
No crear documentos nuevos solo por existir una consecuencia o restricción.
-->

| Concepto             | Cómo se interpreta                                                 | Cuándo conectarlo con otro artifact                                              |
| -------------------- | ------------------------------------------------------------------ | -------------------------------------------------------------------------------- |
| Business Consequence | Algo que ocurre o se pierde si la motivación no se atiende         | Cuando afecta prioridad, riesgo, alcance, viabilidad o decisión                  |
| Business Constraint  | Algo que limita la forma de responder a la motivación              | Cuando condiciona alcance, viabilidad, decisión, implementación o adopción       |
| Relevant Consequence | Consecuencia que pesa lo suficiente para condicionar una respuesta | Cuando justifica una decisión, iniciativa, validación o evaluación de viabilidad |
| Viability Constraint | Restricción que condiciona si la respuesta puede sostenerse        | Cuando requiere Viability Document o Decision Record                             |

## Conceptos complementarios

<!--
¿Qué elementos relacionados ayudan a entender esta motivación sin pertenecer necesariamente a la ruta principal?

Usar esta sección solo cuando existan elementos relevantes para preservar continuidad.
No convertirla en lista exhaustiva.
-->

| Concepto complementario | Relación con la motivación | Path o artifact sugerido |
| ----------------------- | -------------------------- | ------------------------ |
| <concepto>              | <relación>                 | <path o artifact>        |
