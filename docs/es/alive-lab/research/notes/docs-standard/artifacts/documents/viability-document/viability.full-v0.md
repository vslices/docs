---
artifact:
  kind: document
  type: viability
  scope: <concept|feature|capability|initiative|product|service|project|change|decision|handoff|experiment|artifact>
  target: <target-name>
  language: <es|en>

metadata:
  status: <draft|candidate|active|deprecated|superseded>
  relates: 
    - relation: <references/referenced-by|complements|depends-on|owned-by|derived-from|updates|supersedes/superseded-by>
      target: <artifact-id>

document:
  question: ¿Es viable?
  kind: <economic|technical|operational|temporal|organizational|adoption>

tooling:
  schema:
    version: 0.1.0
  template:
    name: viability.document
    version: 0.1.0
---

# Documento de Viabilidad - <tema>

## Organización

```mermaid
flowchart LR
    R["Documento de Viabilidad<br/><small>¿Es viable?</small>"]

    B1["Objeto evaluado<br/><small>¿Qué estamos evaluando?</small>"]
    B2["Criterio de viabilidad<br/><small>¿Qué significa que sea viable para este kind?</small>"]
    B3["Condiciones necesarias<br/><small>¿Qué debe cumplirse para que sea viable?</small>"]
    B4["Restricciones conocidas<br/><small>¿Qué limita su viabilidad?</small>"]
    B5["Evaluación inicial<br/><small>¿Qué tan viable parece ahora?</small>"]
    B6["Riesgo de inviabilidad<br/><small>¿Qué podría volverlo inviable?</small>"]

    B7["Factores evaluados<br/><small>¿Qué factores influyen en esta viabilidad?</small>"]
    B8["Capacidades requeridas<br/><small>¿Qué capacidades deben existir para sostenerla?</small>"]
    B9["Costos o esfuerzo relevante<br/><small>¿Qué costo o esfuerzo condiciona esta viabilidad?</small>"]
    B10["Alternativas de viabilidad<br/><small>¿Qué alternativas podrían hacerla más viable?</small>"]
    B11["Supuestos de viabilidad<br/><small>¿Qué estamos asumiendo para considerarlo viable?</small>"]
    B12["Señales de alerta<br/><small>¿Qué indicios mostrarían pérdida de viabilidad?</small>"]
    B13["Condiciones de revisión<br/><small>¿Qué haría necesario reevaluar la viabilidad?</small>"]

    R --> B1 & B2 & B3 & B4 & B5 & B6
    R -.-> B7 & B8 & B9 & B10 & B11 & B12 & B13
```

## Objeto evaluado

<!--
¿Qué estamos evaluando?

Indicar el concepto, iniciativa, cambio, feature, capability, servicio, producto, experimento, decisión o artifact cuya viabilidad será evaluada.

La escala debe interpretarse según el scope definido en metadata.
-->

## Criterio de viabilidad

<!--
¿Qué significa que sea viable para este kind?

Explicar qué condiciones mínimas permitirían considerar viable este elemento según la dimensión de viabilidad indicada en metadata.

Ejemplos de kind:
- economic
- technical
- operational
- temporal
- organizational
- adoption
-->

## Condiciones necesarias

<!--
¿Qué debe cumplirse para que sea viable?

Listar condiciones necesarias para sostener esta viabilidad según el kind evaluado.
-->

- <condición necesaria>

## Restricciones conocidas

<!--
¿Qué limita su viabilidad?

Registrar restricciones conocidas sin convertir esta sección en planificación completa.
-->

| Restricción | Cómo limita la viabilidad |
| --- | --- |
| <restricción> | <impacto sobre la viabilidad> |

## Evaluación inicial

<!--
¿Qué tan viable parece ahora?

Indicar una evaluación inicial y breve de viabilidad según la información disponible.
-->

## Riesgo de inviabilidad

<!--
¿Qué podría volverlo inviable?

Registrar riesgos o condiciones que podrían hacer que este elemento deje de ser viable.
-->

- <riesgo de inviabilidad>

## Factores evaluados

<!--
¿Qué factores influyen en esta viabilidad?

Registrar factores relevantes para el kind evaluado.
No incluir todas las dimensiones de viabilidad, solo las que correspondan al kind de este artifact.
-->

| Factor | Evaluación |
| --- | --- |
| <factor> | <evaluación> |

## Capacidades requeridas

<!--
¿Qué capacidades deben existir para sostener esta viabilidad?

Indicar capacidades técnicas, económicas, operativas, temporales, organizacionales o de adopción según el kind evaluado.
-->

| Capacidad requerida | Por qué importa |
| --- | --- |
| <capacidad> | <por qué es necesaria> |

## Costos o esfuerzo relevante

<!--
¿Qué costo o esfuerzo condiciona esta viabilidad?

Registrar costos, esfuerzos, carga, complejidad o inversión requerida según el kind evaluado.
-->

| Costo o esfuerzo | Impacto sobre la viabilidad |
| --- | --- |
| <costo o esfuerzo> | <impacto> |

## Alternativas de viabilidad

<!--
¿Qué alternativas podrían hacerla más viable?

Registrar alternativas que podrían reducir costo, riesgo, esfuerzo, complejidad o fricción.
-->

| Alternativa | Cómo mejora la viabilidad |
| --- | --- |
| <alternativa> | <mejora esperada> |

## Supuestos de viabilidad

<!--
¿Qué estamos asumiendo para considerarlo viable?

Registrar premisas que sostienen la evaluación de viabilidad y que podrían cambiar.
-->

| Supuesto | Riesgo si cambia |
| --- | --- |
| <supuesto> | <qué se vería afectado si deja de ser cierto> |

## Señales de alerta

<!--
¿Qué indicios mostrarían pérdida de viabilidad?

Registrar señales tempranas de que la viabilidad podría estar deteriorándose.
-->

- <señal de alerta>

## Condiciones de revisión

<!--
¿Qué haría necesario reevaluar la viabilidad?

Indicar cambios, evidencia, decisiones o condiciones futuras que justificarían revisar esta evaluación.
-->

- <condición de revisión>