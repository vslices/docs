# Problem-First

_Problem-First_ es una modalidad de VSlices Design que parte desde un problema específico de negocio o sistema, y construye suficiente contexto alrededor para mejorarlo de forma efectiva.

Es útil cuando el equipo ya sabe qué duele, pero todavía necesita entender suficiente contexto para evitar resolver la versión incorrecta del problema.

_Problem-First_ asume que no toda iteración de diseño necesita descubrimiento amplio del dominio.

A veces el punto de partida más responsable no es todo el contexto, sino un problema claro.

## Definición

_Problem-First_ es una modalidad de diseño donde el equipo empieza con un problema conocido y entiende progresivamente el contexto alrededor de él.

En la metáfora de la pirámide, _Problem-First_ busca equilibrio entre base y altura.

```text
base / height -> balanced
```

Esto significa que el equipo no construye inmediatamente desde la declaración del problema, pero tampoco pasa demasiado tiempo explorando todo el dominio antes de avanzar.

El objetivo es entender lo suficiente del contexto circundante para definir una mejora útil, factible y segura.

## Cuándo usarlo

Usa _Problem-First_ cuando existe un problema claro que merece atención enfocada.

Es especialmente útil cuando:

* ya se conoce un punto de dolor específico
* el problema tiene impacto de negocio
* el dominio circundante está parcialmente entendido
* el equipo necesita mejorar un área concreta
* el equipo puede identificar quiénes son afectados por el problema
* el problema es lo suficientemente importante como para analizarlo antes de construir
* el alcance debería permanecer enfocado
* el equipo necesita evitar descubrimiento amplio, pero todavía necesita contexto
* el riesgo no es que todo el dominio sea desconocido, sino que el problema sea malentendido
* resolver el problema puede afectar flujos, reglas o responsabilidades cercanas

_Problem-First_ es útil cuando el equipo puede decir:

> Sabemos dónde está el dolor, pero todavía necesitamos entenderlo lo suficiente para mejorarlo con seguridad.

## Cuándo no usarlo

_Problem-First_ puede ser insuficiente cuando:

* el dominio es demasiado poco claro como para identificar el problema real
* la declaración del problema es solo un síntoma
* muchas áreas discrepan sobre cuál es realmente el problema
* el contexto de negocio circundante es mayormente desconocido
* la mejora puede afectar una cadena operacional amplia
* el costo de optimización local es alto
* el equipo necesita descubrir límites antes de definir el problema

En esos casos, Context-First puede ser más apropiado.

_Problem-First_ también puede ser excesivo cuando:

* el dominio ya está bien entendido
* el cambio es pequeño y de bajo riesgo
* el equipo necesita *feedback* rápido de implementación
* el mejor aprendizaje vendrá de una pequeña *slice* funcionando

En esos casos, Slice-First puede ser más apropiado.

## Características

_Problem-First_ normalmente tiene estas características:

* parte desde un punto de dolor conocido
* se enfoca en un área específica de mejora
* evita exploración amplia por adelantado
* construye suficiente contexto alrededor del problema
* enfatiza causa, impacto, riesgo y alcance
* da fuerte atención a Planning
* usa la implementación para validar la mejora elegida
* equilibra análisis con entrega
* intenta evitar tanto construcción prematura como descubrimiento infinito

_Problem-First_ no intenta entender todo el negocio antes de actuar.

Intenta entender el problema lo suficiente para mejorarlo responsablemente.

## Ventajas

_Problem-First_ ayuda al equipo a:

* mantenerse enfocado en un problema concreto
* evitar descubrimiento amplio innecesario
* conectar el trabajo de diseño con dolor de negocio visible
* reducir parálisis por análisis
* avanzar mientras todavía se preserva suficiente contexto
* distinguir síntomas de causas
* identificar flujos y responsabilidades afectadas
* definir el alcance con más claridad
* evaluar *tradeoffs* antes de construir
* entregar valor más rápido que una iteración amplia de Context-First

Es especialmente valioso cuando el mayor riesgo no es falta general de conciencia del dominio, sino malentender el problema que se está resolviendo.

## Desventajas

_Problem-First_ también tiene costos. Puede:

* explorar insuficientemente el dominio más amplio
* resolver un síntoma en vez de una causa
* optimizar un proceso local mientras daña uno adyacente
* perder dependencias ocultas
* asumir demasiado pronto el límite del problema
* producir una solución que funciona técnicamente, pero falla operacionalmente
* moverse a Planning antes de haber descubierto suficiente contexto
* moverse a Building antes de que los riesgos hayan sido explicitados

El principal peligro de _Problem-First_ es la optimización local. El equipo puede resolver el problema visible mientras ignora el sistema más amplio que lo produjo.
