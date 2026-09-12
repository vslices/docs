# Usar Domus Orbis como proyecto de validación

## Estado

Aceptada.

## Contexto

VSlices evoluciona como una suite de ingeniería de software compuesta por:

* VSlices Framework
* VSlices Design
* VSlices Docs Standard
* VSlices Method

La suite busca preservar la continuidad entre:

* descubrimiento del dominio
* documentación
* razonamiento de diseño
* arquitectura
* implementación
* validación
* evolución

Como VSlices sigue en una etapa fundacional temprana, existe un alto riesgo de diseñar abstracciones que sean teóricamente elegantes pero no validadas frente al trabajo real de software.

Este riesgo es especialmente importante porque VSlices no está destinado a convertirse en una colección de abstracciones interesantes.

VSlices debe crecer a partir de problemas recurrentes observados en sistemas reales. Domus Orbis es actualmente el principal proyecto real disponible para validar las ideas de VSlices.

Contiene suficiente complejidad de producto, dominio, documentación, arquitectura e implementación para revelar si los conceptos de VSlices son útiles en la práctica.

## Decisión

Domus Orbis se usará como el proyecto principal de validación de VSlices durante la etapa v0.1.

Los nuevos conceptos, abstracciones, estructuras de documentación, técnicas de diseño y guía del método de VSlices deben probarse contra Domus Orbis antes de tratarse como partes estables de la suite.

Esto aplica especialmente a:

* patrones de modelado de dominio
* organización de features
* modelado de capacidades
* estructuras de documentación
* modalidades de diseño
* workflows del método
* límites arquitectónicos
* primitivas de implementación
* trazabilidad entre productos

Una idea de VSlices no debe convertirse en oficial solo porque sea elegante. Debe convertirse en oficial cuando sobreviva al contacto con necesidades reales del proyecto.

## Fundamento

Domus Orbis proporciona un entorno concreto donde VSlices puede probarse a lo largo del ciclo de vida. Puede validar si VSlices ayuda a preservar la continuidad entre:

* comprensión del dominio
* documentación del sistema
* razonamiento sobre el diseño
* definición de la arquitectura
* implementación del comportamiento
* evolución del sistema a lo largo del tiempo

Esto importa porque VSlices no es solo un framework.

Si la validación ocurre solo mediante ejemplos de código, entonces VSlices Framework puede evolucionar, pero VSlices Design, VSlices Docs Standard y VSlices Method pueden quedar sin probar.

Domus Orbis permite validar la suite como un ciclo de vida conectado, no solo como una biblioteca de implementación.

## Rol de validación

Domus Orbis debe usarse para responder preguntas como:

* ¿Esta abstracción reduce la complejidad accidental?
* ¿Este documento preserva conocimiento útil?
* ¿Esta técnica de diseño ayuda a aclarar el dominio?
* ¿Este paso del método ayuda a pasar del descubrimiento a la implementación?
* ¿Este patrón sigue siendo entendible después de un tiempo?
* ¿Esta estructura ayuda a la evolución futura?
* ¿Esta idea sigue funcionando cuando el dominio se vuelve confuso?
* ¿Esto crea más ceremonia que valor?

Si Domus Orbis expone fricción, esa fricción debe tratarse como retroalimentación de diseño.

El objetivo no es forzar a Domus Orbis a ajustarse a VSlices. Es permitir que Domus Orbis revele dónde VSlices es útil, incompleto, poco claro o excesivamente diseñado.

## Consecuencias

Esta decisión le da a VSlices un camino de validación concreto. Reduce el riesgo de abstracción prematura.

También crea una restricción saludable: no toda idea interesante debe promoverse de inmediato a la suite.

Algunas ideas pueden permanecer como:

* experimentos
* notas de campo
* entradas de Alive Lab
* patrones locales
* posibilidades futuras

Esto es aceptable. VSlices debe preferir la utilidad validada por encima de la completitud teórica.

## Límite de alcance

Domus Orbis es el proyecto principal de validación, no el único proyecto futuro posible de validación.

Un patrón validado en Domus Orbis debe seguir tratándose con cuidado antes de generalizarse.

Algunas necesidades de Domus Orbis pueden ser específicas de ese proyecto.

Algunas ideas de VSlices pueden requerir validación en otros dominios antes de convertirse en recomendaciones estables.

Domus Orbis valida que una idea puede funcionar en un proyecto real.

No demuestra automáticamente que la idea sea universal.

## Regla de documentación

Cuando una idea de VSlices se valida mediante Domus Orbis, la documentación debe preservar:

* qué problema apareció
* qué solución se intentó
* qué tradeoff se aceptó
* qué cambió en el diseño
* qué cambió en la implementación
* y qué sigue siendo incierto

Esto mantiene visible la validación y evita que la suite finja que las decisiones aparecieron completamente formadas.

## Tradeoff aceptado

Usar Domus Orbis como proyecto principal de validación puede sesgar las decisiones tempranas de VSlices hacia las necesidades de un solo sistema.

Este tradeoff se acepta porque validar contra un proyecto real es mejor que no validar contra ninguno.

Más adelante, el riesgo se reducirá probando VSlices en proyectos, dominios y contextos de colaboración adicionales.

## Principio

VSlices no debe diseñarse solo a partir de la teoría.

VSlices debe moldearse con la presión de proyectos reales.

Domus Orbis existe como el primer lugar donde las ideas de VSlices deben demostrar que ayudan.
