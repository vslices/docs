# Usar el proyecto de la compañía de seguros como caso de adopción

## Estado

Aceptada.

## Contexto

VSlices se está desarrollando como una suite compuesta por:

* VSlices Method
* VSlices Design
* VSlices Docs Standard
* VSlices Framework

Domus Orbis es actualmente el proyecto principal de validación para validar las ideas de VSlices en un proyecto donde podemos moldear el proceso, la documentación, la arquitectura y la implementación con alto control.

Sin embargo, eso no cubre otro escenario importante:

> Unirse a un proyecto existente que no fue creado usando VSlices Method, pero donde existe apertura para aplicar algunas prácticas de VSlices de forma progresiva.

El contexto de trabajo actual dentro de una compañía de seguros proporciona este escenario. El proyecto ya existe.

Su documentación, arquitectura, prácticas de desarrollo, comprensión del dominio y hábitos del equipo actuales no se crearon usando VSlices.

Esto lo convierte en un caso de adopción valioso para VSlices Method, VSlices Design y VSlices Docs Standard.

## Decisión

El contexto del proyecto de la compañía de seguros se usará como un caso de adopción para validar cómo VSlices puede introducirse en un proyecto existente. Este caso se enfocará en:

* comprender un dominio existente
* documentar conocimiento progresivamente
* identificar contexto faltante
* preservar la intención descubierta
* mejorar la continuidad entre conversaciones y documentación
* aplicar razonamiento de diseño sin forzar la adopción del framework
* validar si VSlices Method puede ayudar en un proyecto que no comenzó con VSlices

Este caso no tiene la intención de validar primero VSlices Framework. El objetivo principal de validación es:

```text
VSlices Method
VSlices Design
VSlices Docs Standard
```

VSlices Framework puede mencionarse solo cuando los patrones de implementación se vuelvan relevantes.

## Fundamento

La mayoría de los equipos reales no empiezan desde un lienzo en blanco. Muchos métodos de ingeniería útiles deben funcionar en proyectos que ya tienen:

* código
* arquitectura
* huecos de documentación
* presión de entrega
* hábitos del equipo
* lenguaje de negocio
* complejidad accidental

Si VSlices solo funciona cuando se aplica desde el principio, su valor práctico sería limitado. Este caso de adopción ayuda a validar si VSlices puede aportar valor de forma incremental. La pregunta clave es:

> ¿Puede VSlices ayudar a recuperar la continuidad en un proyecto donde la continuidad no se preservó intencionalmente desde el inicio?

## Alcance

Este caso de adopción debe validar un uso ligero de las prácticas de VSlices. El enfoque debe estar en actividades como:

* crear documentos de contexto a partir del conocimiento existente
* extraer vocabulario de conversaciones y sistemas
* documentar capacidades descubiertas
* identificar límites poco claros
* registrar decisiones
* mapear procesos actuales
* separar conceptos de dominio de detalles de implementación
* usar modalidades de VSlices Design para razonar sobre el sistema existente

El trabajo debe evitar introducir ceremonia innecesaria.

El objetivo no es convertir el proyecto en un proyecto VSlices. Es observar dónde ayuda VSlices.

## No objetivos

Esta decisión no significa:

* forzar VSlices Framework en el proyecto de la compañía de seguros
* exigir que el equipo adopte todos los productos de VSlices
* reescribir la documentación existente
* reemplazar la arquitectura existente
* imponer terminología de VSlices demasiado pronto
* o tratar el proyecto como un laboratorio controlado

Este es un caso de adopción, no un proyecto de migración.

## Preguntas de validación

Este caso debería ayudar a responder:

* ¿Puede VSlices Method ser útil cuando se introduce tarde?
* ¿Qué documentos aportan valor primero en un proyecto existente?
* ¿Qué técnicas de VSlices Design ayudan a entender contexto heredado o existente?
* ¿Cuánta documentación es útil antes de que se convierta en ceremonia?
* ¿Puede VSlices Docs Standard ayudar a recuperar intención faltante?
* ¿Puede la terminología de VSlices coexistir con el lenguaje actual del equipo?
* ¿Qué debería introducirse primero cuando un equipo tiene contexto limitado?
* ¿Qué prácticas son demasiado pesadas para la adopción temprana?

## Resultados esperados

Los resultados útiles pueden incluir:

* documentos de contexto
* notas de vocabulario
* documentos de capacidad
* notas de proceso
* registros de decisión
* observaciones de límites
* notas de campo
* lecciones de adopción

Estos resultados deben ser pequeños y prácticos. Deben preservar conocimiento que de otro modo permanecería disperso en reuniones, conversaciones, tickets, código o memoria personal.

## Tradeoff aceptado

Este caso puede no permitir una validación completa de VSlices porque el contexto del proyecto es externo y ya está restringido. Algunas limitaciones pueden incluir:

* influencia limitada sobre la arquitectura
* acceso limitado a decisiones históricas
* restricciones organizacionales existentes
* visibilidad incompleta del dominio
* presión de entrega

Este tradeoff se acepta porque precisamente esas restricciones son lo que hacen útil el caso. La adopción real rara vez ocurre en condiciones ideales.

## Relación con Domus Orbis

Domus Orbis sigue siendo el proyecto principal de validación para construir y refinar VSlices con alto control.

El proyecto de la compañía de seguros se convierte en un caso de validación complementario para adopción progresiva.

```text
Domus Orbis
  valida VSlices como un ciclo de vida diseñado.

Proyecto de la compañía de seguros
  valida VSlices como ayuda para la adopción en un ciclo de vida existente.
```

Ambos casos son útiles, pero responden preguntas distintas.

## Principio

VSlices no debe ayudar solo cuando un proyecto comienza correctamente.

VSlices también debe ayudar a recuperar claridad cuando un proyecto ya existe.

La adopción progresiva forma parte de la arquitectura progresiva.
