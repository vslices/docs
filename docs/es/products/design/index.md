# VSlices Design

VSlices Design ayuda a los equipos a decidir cuánto entendimiento de dominio se necesita antes de convertir conocimiento de negocio en *software*.

Proporciona modalidades de diseño, herramientas de razonamiento y heurísticas de modelado para moverse desde material de negocio poco claro hacia decisiones de *software* más claras sin perder continuidad.

VSlices Design es intencionalmente independiente de VSlices Framework. No necesitas usar VSlices Framework para aplicar VSlices Design.

El Framework puede ayudar más adelante a implementar algunas de las ideas descubiertas mediante Design, pero Design en sí mismo es un producto de razonamiento agnóstico al *stack*.

El propósito de VSlices Design es ayudar a los equipos a entender:

* con qué contexto de negocio están trabajando
* cuánta incertidumbre existe
* qué tipo de enfoque de diseño es apropiado
* cómo el conocimiento de dominio se convierte en artefactos de *software*
* cuándo explorar ampliamente
* cuándo enfocarse en un problema específico
* cuándo aprender desde una pequeña *vertical slice*

VSlices Design no asume que todos los proyectos necesitan la misma metodología.

Distintas situaciones requieren distintas formas de moverse desde descubrimiento hacia implementación.

## Propósito

Muchos proyectos de *software* empiezan desde artefactos que aparecen demasiado tarde en el proceso de razonamiento:

* historias de usuario
* pantallas
* APIs
* tablas de base de datos
* componentes técnicos
* tareas de implementación

Estos artefactos son útiles, pero no siempre son el punto de partida correcto.

Cuando el dominio es poco claro, fragmentado, manual, impulsado por legado u organizacionalmente complejo, partir directamente desde la implementación puede crear complejidad accidental.

VSlices Design existe para reducir ese riesgo.

Su propósito es ayudar a los equipos a elegir la cantidad correcta de entendimiento, contexto, planificación y *feedback* de implementación antes de avanzar.

## ¿Qué problema resuelve?

Muchos equipos comienzan el diseño de *software* desde el primer artefacto visible:

* una pantalla
* una historia de usuario
* un *endpoint*
* una tabla de base de datos
* una tarea técnica
* una *feature* solicitada

Esos artefactos son útiles, pero normalmente aparecen después de que preguntas importantes del dominio ya fueron omitidas.

VSlices Design ayuda a los equipos a pausar antes de comprometerse demasiado pronto con una estructura.

Su pregunta principal es:

```text
¿Entendemos suficiente del material de negocio para dar forma al software de manera segura?
```

> A veces la respuesta requiere descubrimiento contextual amplio.
> A veces requiere análisis enfocado de un problema.
> A veces requiere construir una pequeña *vertical slice* para aprender desde *feedback* de implementación.

VSlices Design ayuda a los equipos a elegir el punto de partida correcto para la incertidumbre que realmente enfrentan.

## ¿Cuándo debería usar VSlices Design?

Usa VSlices Design cuando el equipo necesita razonar sobre un sistema de *software* antes de decidir cómo debería construirse.

Es especialmente útil cuando el equipo enfrenta incertidumbre alrededor del dominio, el problema, los límites o la forma de la solución. VSlices Design puede ayudar cuando:

* el contexto de negocio todavía no está claro;
* el equipo no está seguro de dónde están los límites del sistema;
* las partes interesadas describen soluciones antes de que el problema subyacente sea entendido;
* distintas personas usan palabras distintas para el mismo concepto;
* el equipo necesita decidir cuánto descubrimiento es necesario antes de construir;
* el equipo quiere evitar diseñar arquitectura desde pantallas, tablas, *endpoints* o tareas demasiado pronto;
* la implementación ya empezó, pero el modelo de dominio todavía se siente inestable.

VSlices Design no solo es útil antes de la implementación. También puede usarse durante la implementación cuando aparece nuevo conocimiento de dominio, cuando una *slice* revela supuestos incorrectos o cuando el equipo se da cuenta de que la estructura actual ya no representa claramente el negocio.

La pregunta principal es:

> ¿Entendemos suficiente del material de negocio para dar forma a la estructura de *software* de manera segura?

Si la respuesta es no, VSlices Design ayuda al equipo a decidir qué tipo de entendimiento falta y qué modalidad puede ayudar después.

## Qué no es VSlices Design

VSlices Design no es una metodología universal. No afirma que todos los sistemas deberían diseñarse de la misma manera. Y no asume que:

* Context-First siempre sea correcto
* Problem-First siempre sea correcto
* Slice-First siempre sea correcto
* el descubrimiento amplio siempre sea necesario
* la implementación rápida siempre sea mejor
* la documentación sea valiosa por defecto

VSlices Design valora la documentación solo cuando preserva intención, reduce ambigüedad o mejora continuidad entre decisiones. El enfoque correcto depende de la incertidumbre, el riesgo, la madurez del dominio y la urgencia de negocio de la situación.

## Relación con la VSlices Suite

VSlices Design es un producto dentro de la VSlices Suite.

Se conecta con los otros productos, pero permanece independiente.

* VSlices Design proporciona las modalidades de diseño y herramientas de razonamiento.
* VSlices Docs Standard puede proporcionar estructuras formales de documentación para preservar la intención descubierta.
* VSlices Method puede definir cómo se aplica el proceso de diseño dentro de un flujo de ingeniería.
* VSlices Framework puede reflejar más adelante los conceptos resultantes como contextos, capacidades, *features*, flujos, errores e integraciones.

El objetivo es la continuidad.

El entendimiento de dominio no debería desaparecer cuando el equipo empieza a documentar.

La documentación no debería quedar desconectada de la arquitectura.

La arquitectura no debería quedar desconectada de la implementación.

La implementación debería permanecer trazable hacia la intención de negocio que la justificó.

## Principio central

VSlices Design sigue un principio simple: *Entender el material de negocio antes de construir la estructura de software*.

> A veces eso requiere descubrimiento contextual amplio.
> A veces requiere análisis enfocado de un problema.
> A veces requiere una pequeña *vertical slice*.

Lo importante no es elegir la modalidad más sofisticada, sino elegir la modalidad que coincide con la incertidumbre que el equipo realmente enfrenta.
