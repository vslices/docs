# Documento de Contexto - <tema>

## Organización

```mermaid
flowchart LR
    R["Documento de Contexto<br/><small>¿Dónde existe?</small>"]

    B1["Escenario<br/><small>¿En qué situación aparece?</small>"]
    B2["Motivación contextual<br/><small>¿Por qué importa entender este contexto?</small>"]
    B3["Situación actual<br/><small>¿Qué ocurre hoy?</small>"]
    B4["Elementos involucrados<br/><small>¿Qué personas, sistemas, procesos o artifacts participan?</small>"]
    B5["Límites contextuales<br/><small>¿Dónde aplica y dónde deja de aplicar?</small>"]

    B6["Origen del contexto<br/><small>¿De dónde viene este contexto?</small>"]
    B7["Riesgos de malentendido<br/><small>¿Qué se puede interpretar mal sin este contexto?</small>"]
    B8["Mantenimiento<br/><small>¿Cuándo debería revisarse este contexto?</small>"]
    B9["Supuestos contextuales<br/><small>¿Qué estamos asumiendo como cierto?</small>"]
    B10["Contexto no resuelto<br/><small>¿Qué todavía no entendemos bien?</small>"]

    B1_1["Situación observada<br/><small>¿Qué situación concreta origina este contexto?</small>"]
    B1_2["Momento o etapa<br/><small>¿En qué momento del trabajo aparece?</small>"]

    B2_1["Intención preservada<br/><small>¿Qué intención se busca no perder?</small>"]
    B2_2["Costo de no entenderlo<br/><small>¿Qué se vuelve más difícil sin este contexto?</small>"]

    B3_1["Estado actual<br/><small>¿Cómo están las cosas ahora?</small>"]
    B3_2["Fricciones actuales<br/><small>¿Qué tensiones existen hoy?</small>"]
    B3_3["Condiciones actuales<br/><small>¿Qué condiciones hacen que este contexto exista hoy?</small>"]

    B4_1["Actores o roles<br/><small>¿Quiénes participan o se ven afectados?</small>"]
    B4_2["Sistemas o artifacts<br/><small>¿Qué sistemas, documentos o artifacts participan?</small>"]
    B4_3["Procesos o superficies<br/><small>¿Qué procesos, vistas o superficies aparecen?</small>"]

    B5_1["Aplica en<br/><small>¿Dónde sí aplica este contexto?</small>"]
    B5_2["No aplica en<br/><small>¿Dónde no debería extrapolarse?</small>"]
    B5_3["Zona gris<br/><small>¿Qué límites todavía no están claros?</small>"]

    B6_1["Observación base<br/><small>¿Qué observación originó este contexto?</small>"]
    B6_2["Fuente de contexto<br/><small>¿Qué conversación, artifact o caso lo soporta?</small>"]

    B7_1["Malinterpretación posible<br/><small>¿Qué podría entenderse mal?</small>"]
    B7_2["Consecuencia del malentendido<br/><small>¿Qué problema causa esa confusión?</small>"]

    B8_1["Gatillo de revisión<br/><small>¿Qué cambio obligaría a revisar este contexto?</small>"]

    B9_1["Supuesto explícito<br/><small>¿Qué estamos dando por válido?</small>"]
    B9_2["Riesgo del supuesto<br/><small>¿Qué pasa si este supuesto cambia?</small>"]

    B10_1["Duda abierta<br/><small>¿Qué falta entender?</small>"]
    B10_2["Impacto de la duda<br/><small>¿Qué decisión se ve afectada por no saberlo?</small>"]

    R --> B1 & B2 & B3 & B4 & B5
    R -.-> B6 & B7 & B8 & B9 & B10

    B1 --> B1_1 & B1_2
    B2 --> B2_1 & B2_2
    B3 --> B3_1 & B3_2 & B3_3
    B4 --> B4_1 & B4_2 & B4_3
    B5 --> B5_1 & B5_2 & B5_3

    B6 -.-> B6_1 & B6_2
    B7 -.-> B7_1 & B7_2
    B8 -.-> B8_1
    B9 -.-> B9_1 & B9_2
    B10 -.-> B10_1 & B10_2
```

## Escenario

<!--
¿En qué situación aparece este concepto, problema, sistema, capacidad, decisión o artifact?
- ¿Qué situación concreta origina este contexto?
- ¿En qué momento del trabajo aparece?
-->

### Situación observada

<!--
¿Qué situación concreta origina este contexto?
-->

### Momento o etapa

<!--
¿En qué momento del trabajo aparece?
-->

## Motivación contextual

<!--
¿Por qué importa entender este contexto?
- ¿Qué intención se busca no perder?
- ¿Qué se vuelve más difícil sin este contexto?
-->

### Intención preservada

<!--
¿Qué intención se busca no perder?
-->

### Costo de no entenderlo

<!--
¿Qué se vuelve más difícil sin este contexto?
-->

## Situación actual

<!--
¿Qué ocurre hoy?
- ¿Cómo están las cosas ahora?
- ¿Qué tensiones existen hoy?
- ¿Qué condiciones hacen que este contexto exista hoy?
-->

### Estado actual

<!--
¿Cómo están las cosas ahora?
-->

### Fricciones actuales

<!--
¿Qué tensiones existen hoy?
-->

### Condiciones actuales

<!--
¿Qué condiciones hacen que este contexto exista hoy?
-->

## Elementos involucrados

<!--
¿Qué personas, sistemas, procesos o artifacts participan en este contexto?
- ¿Quiénes participan o se ven afectados?
- ¿Qué sistemas, documentos o artifacts participan?
- ¿Qué procesos, vistas o superficies aparecen?
-->

| Tipo | Elemento | Participación en el contexto |
| --- | --- | --- |
| <actor, rol, sistema, proceso, superficie o artifact> | <nombre> | <cómo participa o por qué importa> |

## Límites contextuales

<!--
¿Dónde aplica y dónde deja de aplicar este contexto?
- ¿Dónde sí aplica este contexto?
- ¿Dónde no debería extrapolarse?
- ¿Qué límites todavía no están claros?
-->

| Tipo de límite | Descripción |
| --- | --- |
| Aplica en | <dónde sí aplica este contexto> |
| No aplica en | <dónde no debería extrapolarse> |
| Zona gris | <qué límites todavía no están claros> |

## Origen del contexto

<!--
¿De dónde viene este contexto?
- ¿Qué observación originó este contexto?
- ¿Qué conversación, artifact o caso lo soporta?
-->

### Observación base

<!--
¿Qué observación originó este contexto?
-->

### Fuente de contexto

<!--
¿Qué conversación, artifact o caso lo soporta?
-->

## Riesgos de malentendido

<!--
¿Qué se puede interpretar mal si este contexto no se entiende?
- ¿Qué podría entenderse mal?
- ¿Qué problema causa esa confusión?
-->

| Malinterpretación posible | Consecuencia |
| --- | --- |
| <qué podría entenderse mal> | <qué problema causa esa confusión> |

## Mantenimiento

<!--
¿Cuándo debería revisarse este contexto?
- ¿Qué cambio obligaría a revisar este contexto?
-->

### Gatillo de revisión

<!--
¿Qué cambio obligaría a revisar este contexto?
-->

## Supuestos contextuales

<!--
¿Qué estamos asumiendo como cierto?
- ¿Qué estamos dando por válido?
- ¿Qué pasa si este supuesto cambia?
-->

| Supuesto explícito | Riesgo del supuesto |
| --- | --- |
| <qué estamos dando por válido> | <qué pasa si este supuesto cambia> |

## Contexto no resuelto

<!--
¿Qué todavía no entendemos bien?
- ¿Qué falta entender?
- ¿Qué decisión se ve afectada por no saberlo?
-->

| Duda abierta | Impacto de la duda |
| --- | --- |
| <qué falta entender> | <qué decisión se ve afectada por no saberlo> |
