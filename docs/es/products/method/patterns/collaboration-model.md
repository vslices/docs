# Modelo de colaboración

El modelo de colaboración (_Collaboration Model_ en inglés) explica cómo las personas o equipos pueden trabajar usando _VSlices Method_ sin perder continuidad.

_VSlices Method_ no requiere roles fijos. Describe responsabilidades que pueden ser asumidas por una persona, compartidas por un equipo pequeño o distribuidas entre equipos especializados.

El objetivo no es definir un organigrama. Es preservar la intención a medida que el trabajo se mueve entre descubrimiento, documentación, diseño, implementación, validación y evolución.

## Idea central

Las etapas de una iteración de _VSlices Design_ son responsabilidades de colaboración. No son roles obligatorios.

* Un equipo pequeño puede asumir todas las responsabilidades en conjunto.
* Una organización más grande puede distribuirlas entre distintas personas o equipos.

La regla importante es la continuidad:

> Cada responsabilidad debería preservar suficiente intención para que la siguiente responsabilidad pueda actuar sin tener que adivinar por qué el trabajo importa.

## Responsabilidades comunes

Una iteración de _VSlices Method_ puede involucrar varias responsabilidades.

No necesitan estar separadas. Solo necesitan ser lo suficientemente visibles para que la continuidad pueda preservarse.

* **Responsabilidad de descubrimiento** identifica señales del dominio, problemas, lenguaje, workflows, actores e incertidumbre.
* **Responsabilidad de preservación de contexto** organiza el conocimiento descubierto en un contexto compartido.
* **Responsabilidad de razonamiento de diseño** elige cómo razonar sobre la incertidumbre actual.
* **Responsabilidad de decisión** selecciona una dirección mientras hace explícitos los tradeoffs.
* **Responsabilidad de construcción** convierte la dirección seleccionada en comportamiento funcional.
* **Responsabilidad de validación** reúne evidencia desde revisión, uso, entrega u operación.
* **Responsabilidad de continuidad** lleva el nuevo aprendizaje de vuelta al contexto compartido.

En un equipo pequeño, las mismas personas pueden asumir todas las responsabilidades. En una organización más grande, distintos grupos pueden asumir distintas responsabilidades.

## Colaboración a través del flujo de iteración

El flujo compartido de iteración de VSlices Design es:

```text
Understanding
-> Contextualizing
-> Planning
-> Building
-> Understanding
```

> La colaboración debería proteger la continuidad a través de este flujo.
> _Understanding_ no debería producir notas desconectadas.
> _Contextualizing_ no debería producir documentos que nadie usa.
> _Planning_ no debería producir decisiones sin contexto.
> _Building_ no debería implementar comportamiento sin intención.
> _Validation_ no debería convertirse en feedback aislado que nunca cambia el trabajo futuro.

Cada etapa debería dejar suficiente conocimiento para que la siguiente etapa avance de forma responsable.

## Handoffs

Un _handoff_ ocurre cuando la responsabilidad se mueve de una persona o equipo a otro.

Un _handoff_ no necesita ceremonia, necesita intención preservada. Los _handoffs_ útiles normalmente aclaran:

* qué contexto sostiene el trabajo actual
* qué problema u oportunidad se está abordando
* qué decisión se ha tomado
* qué sigue siendo incierto
* qué comportamiento se espera
* qué feedback debería observarse

El propósito de un _handoff_ no es transferir documentos. El propósito es transferir suficiente entendimiento para que el trabajo pueda continuar sin perder significado.

## Equipos pequeños

En un equipo pequeño, la colaboración puede ocurrir mediante conversación directa. La documentación puede seguir siendo ligera.

El principal riesgo es que el conocimiento permanezca implícito porque todos creen que el contexto es compartido. Los equipos pequeños deberían preservar conocimiento cuando:

* una decisión afecta trabajo futuro
* un término puede interpretarse de distintas formas
* un comportamiento tiene consecuencias importantes
* un workflow tiene excepciones
* la validación cambia el entendimiento del problema

Mientras más pequeño es el equipo, más tentador es depender solo de la memoria. _VSlices Method_ debería ayudar a preservar las pocas cosas que el trabajo futuro no debería tener que redescubrir.

## Organizaciones más grandes

En una organización más grande, las responsabilidades pueden estar distribuidas. Un grupo puede:

* descubrir señales del dominio
* otro puede organizar contexto
* otro puede planificar el trabajo
* otro puede construir
* otro puede validar

El principal riesgo es la optimización local. Cada grupo puede hacer correctamente su parte mientras la intención original desaparece entre etapas.

Las organizaciones más grandes deberían preservar continuidad haciendo que el contexto, las decisiones, el comportamiento esperado y la validación sean lo suficientemente visibles para que otros grupos puedan continuar el trabajo de forma responsable.

## Riesgos de colaboración

Varios riesgos aparecen comúnmente cuando la colaboración pierde continuidad.

* **Descubrimiento sin preservación** crea conocimiento que desaparece después de las conversaciones.
* **Documentación sin uso** crea artefactos desconectados del trabajo.
* **Planificación sin contexto** crea tareas que ocultan la razón detrás del trabajo.
* **Construcción sin intención** crea implementación que resuelve el ticket, pero no el problema.
* **Validación sin ciclos de feedback** crea aprendizaje que no cambia decisiones futuras.
* **Especialización sin continuidad** crea equipos que optimizan su etapa mientras debilitan el sistema completo.

El _Collaboration Model_ existe para hacer visibles estos riesgos antes de que se vuelvan normales.

## Principio guía

La estructura debería adaptarse a la organización. La organización no debería verse forzada a adaptarse al método.

Usa la estructura de colaboración más pequeña que preserve la intención de la que depende el trabajo futuro.

* Si la conversación directa preserva suficiente continuidad, usa conversación directa.
* Si el trabajo cruza tiempo, personas, equipos o decisiones, preserva el conocimiento que no debería perderse.
