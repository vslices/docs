# Nota de Soporte - Validación - <tema>

## Organización

```mermaid
flowchart LR
    R["Nota de Soporte<br/><small>¿Qué se necesita?</small>"]
    K["validation<br/><small>¿Qué significa lo obtenido frente a un criterio?</small>"]

    B1["Resultado evaluado<br/><small>¿Qué resultado estamos interpretando?</small>"]
    B2["Criterio usado<br/><small>¿Contra qué se interpreta?</small>"]
    B3["Interpretación<br/><small>¿Qué significa el resultado?</small>"]
    B4["Uso esperado<br/><small>¿Cómo debería usarse esta validación?</small>"]

    R --> K
    K --> B1 & B2 & B3 & B4
```

## Resultado evaluado

<!--
¿Qué resultado estamos interpretando?

Referenciar o describir brevemente el resultado observado que será evaluado.
-->

## Criterio usado

<!--
¿Contra qué se interpreta?

Indicar expectativa, criterio, regla, comportamiento esperado o condición usada para interpretar el resultado.
-->

## Interpretación

<!--
¿Qué significa el resultado?

Explicar si el resultado cumple, no cumple, cumple parcialmente o deja dudas frente al criterio usado.
-->

## Uso esperado

<!--
¿Cómo debería usarse esta validación?

Indicar si esta validación debería alimentar una decisión, feedback, actualización documental o nueva iteración.
-->