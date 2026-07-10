# Comparación de modalidades de diseño

VSlices Design proporciona distintas modalidades para abordar el diseño de *software* dependiendo del tipo de incertidumbre que enfrenta el equipo.

Estas modalidades no son metodologías que compiten entre sí. Son estrategias de diseño.

Un equipo no necesita identificarse permanentemente con una de ellas. El mismo proyecto puede usar distintas modalidades en distintos momentos, dependiendo de qué es lo que actualmente no está claro.

El propósito de esta comparación es ayudar a los equipos a decidir por dónde empezar.

## Resumen

| Modalidad     | Usar cuando                                                                                                     | Incertidumbre principal                                                                              | Riesgo si se omite                                                                            |
| ------------- | --------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| Context-First | El área de negocio es<br/>amplia, poco clara,<br/>fragmentada o mal<br/>entendida.                                          | El equipo todavía no entiende<br/>suficiente del contexto de<br/>dominio.                                    | Construir estructuras<br/>de *software* basadas en<br/>supuestos, lenguaje<br/>incompleto o límites<br/>mal entendidos. |
| Problem-First | Existe un dolor,<br/>ineficiencia, riesgo<br/>u oportunidad visible,<br/>pero sus causas no<br/>están completamente<br/>entendidas. | El equipo todavía no sabe qué<br/>problema debería resolverse<br/>realmente.                                 | Resolver síntomas<br/>en vez de causas.                                                                     |
| Slice-First   | El equipo puede<br/>aprender de forma<br/>segura construyendo<br/>una parte pequeña,<br/>estrecha y reversible<br/>del sistema.     | El equipo todavía no sabe si<br/>una solución, modelo o<br/>integración propuesta<br/>funcionará en la práctica. | Pasar demasiado<br/>tiempo diseñando<br/>antes de validar<br/>la realidad.                                          |

## Context-First

Context-First es útil cuando el equipo todavía no entiende el material de negocio lo suficiente como para definir límites de *software* confiables.

Esta modalidad empieza explorando:

* quién participa en el dominio,
* qué responsabilidades existen,
* qué procesos importan,
* qué conceptos usa el negocio,
* qué restricciones dan forma a las decisiones,
* y dónde podrían existir límites.

Context-First ayuda a evitar arquitectura prematura.

Es especialmente útil cuando un equipo está entrando a un dominio nuevo, reemplazando un proceso legado o intentando entender cómo interactúan varias áreas de negocio.

### Preferir Context-First cuando

* el lenguaje de dominio no está claro;
* las partes interesadas describen el mismo concepto de formas diferentes;
* los procesos de negocio no están bien documentados;
* el equipo no sabe dónde deberían estar los límites del sistema;
* el riesgo de malentender el dominio es mayor que el riesgo de retrasar la implementación.

### Tener cuidado cuando

Context-First puede volverse demasiado amplio si el equipo sigue explorando sin decidir qué necesita construirse.

El objetivo no es entender todo. Es entender lo suficiente para tomar decisiones de diseño más seguras.

---

## Problem-First

Problem-First es útil cuando el equipo ya ve un dolor concreto, pero todavía no lo entiende con suficiente profundidad.

Esta modalidad parte desde un problema en vez de un contexto amplio.

El equipo investiga:

* qué está ocurriendo,
* quién está afectado,
* cuándo aparece el problema,
* qué lo causa,
* qué consecuencias crea,
* y qué contaría como mejora.

Problem-First ayuda a evitar resolver algo incorrecto.

Es especialmente útil cuando las partes interesadas piden una *feature*, pero el equipo sospecha que la *feature* solicitada puede ser solo una solución posible.

### Preferir Problem-First cuando

* un dolor de negocio es visible;
* los usuarios están pidiendo una solución específica, pero la necesidad subyacente no está clara;
* el equipo necesita separar síntomas de causas;
* existen varias soluciones posibles;
* el costo de construir algo incorrecto es significativo.

### Tener cuidado cuando

Problem-First puede volverse demasiado estrecho si el equipo ignora el contexto circundante.

Algunos problemas son síntomas de problemas estructurales más grandes.

Cuando eso ocurre, el equipo puede necesitar moverse temporalmente hacia Context-First.

---

## Slice-First

Slice-First es útil cuando el equipo puede aprender de forma segura construyendo una pequeña parte vertical del sistema.

Esta modalidad parte desde un candidato de implementación estrecho.

La *slice* debería ser lo suficientemente pequeña para validar supuestos sin comprometer toda la arquitectura demasiado temprano.

Slice-First ayuda a los equipos a aprender desde comportamiento ejecutable.

Es especialmente útil cuando el equipo ya tiene suficiente entendimiento para intentar algo concreto, pero todavía necesita *feedback* de implementación, usuarios, integraciones o restricciones técnicas.

### Preferir Slice-First cuando

* el dominio está suficientemente entendido para una parte pequeña del sistema;
* el equipo necesita *feedback* técnico o de producto;
* un experimento pequeño puede reducir incertidumbre;
* el costo de construir una *slice* estrecha es aceptable;
* la *slice* puede cambiarse, eliminarse o expandirse después.

### Tener cuidado cuando

Slice-First puede crear arquitectura accidental si el equipo trata la primera *slice* como la estructura final del sistema.

El objetivo no es construir rápido a cualquier costo. Es aprender mediante una pieza controlada de implementación.

---

## Movimiento entre modalidades

Las modalidades no son etapas lineales.

Un equipo puede empezar con Context-First, descubrir un problema específico, moverse a Problem-First y luego validar una solución mediante Slice-First.

Un equipo también puede empezar con Slice-First, descubrir que la *slice* expone conceptos de dominio mal entendidos y volver a Context-First.

La pregunta importante es:

> ¿Qué tipo de incertidumbre estamos enfrentando ahora?

VSlices Design usa modalidades para responder esa pregunta sin forzar a todos los proyectos dentro del mismo proceso de diseño.

---

## Resumen

| Modalidad     | Usar cuando                                                            | Riesgo principal reducido                                |
| ------------- | ---------------------------------------------------------------------- | -------------------------------------------------------- |
| Context-First | el negocio/dominio es poco claro o<br/>fragmentado                         | construir la abstracción incorrecta                      |
| Problem-First | el dominio existe, pero un problema<br/>específico necesita clarificación  | resolver síntomas en vez de causas                       |
| Slice-First   | la incertidumbre se reduce mejor<br/>mediante *feedback* de implementación | planificar demasiado antes de<br/>contrastar con la realidad |

| Si el equipo dice...                                                           | Considerar...              |
| ------------------------------------------------------------------------------ | -------------------------- |
| Todavía no entendemos esta área de negocio.                                  | Context-First              |
| Sabemos que algo duele, pero no estamos seguros de cuál es<br/>el problema real. | Problem-First              |
| Entendemos lo suficiente para probar una pieza pequeña y<br/>aprender de ella.   | Slice-First                |
| Seguimos descubriendo nuevos conceptos de negocio<br/>mientras construimos.      | Volver hacia Context-First |
| Estamos construyendo *features* solicitadas, pero el dolor permanece.        | Volver hacia Problem-First |
| Estamos discutiendo demasiado y validando muy poco.                          | Movernos hacia Slice-First |
