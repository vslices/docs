# Slice-First

_Slice-First_ es una modalidad de VSlices Design que parte desde una pequeña *vertical slice* para aprender desde el *feedback* de implementación lo antes posible.

Es útil cuando el equipo puede aprender más de forma segura construyendo una pieza delgada y funcional del sistema que extendiendo el análisis por adelantado.

_Slice-First_ asume que no toda iteración de diseño necesita una base contextual amplia antes de la implementación. A veces, el punto de partida más responsable es una *slice* pequeña, concreta y de extremo a extremo.

## Definición

_Slice-First_ es una modalidad de diseño donde el equipo mantiene intencionalmente pequeña la base contextual inicial y avanza rápido hacia una *vertical slice* funcional.

En la metáfora de la pirámide, _Slice-First_ da más peso a la altura que a la base.

```text
base / height -> small
```

Esto significa que el equipo invierte solo el esfuerzo suficiente en Understanding y Contextualizing para evitar implementación ciega, y luego avanza rápidamente hacia Planning y Building.

El objetivo no es saltarse el entendimiento. Es aprender mediante implementación mientras se mantiene la *slice* lo suficientemente pequeña para limitar el riesgo.

## Cuándo usarlo

Usa _Slice-First_ cuando el *feedback* de implementación es más valioso que un análisis extendido por adelantado. Es especialmente útil cuando:

* el dominio ya está razonablemente entendido
* el equipo necesita validación rápida
* el cambio propuesto puede probarse mediante una pequeña *vertical slice*
* el costo de equivocarse es bajo o contenido
* el equipo necesita validar dirección técnica
* el equipo necesita validar dirección de producto
* el equipo necesita reducir incertidumbre mediante *software* funcionando
* la *slice* puede entregarse sin desestabilizar flujos adyacentes
* el equipo puede observar *feedback* poco después de la entrega
* el trabajo puede acotarse lo suficiente para evitar expansión accidental

_Slice-First_ es útil cuando el equipo puede decir:

> Sabemos lo suficiente para construir una pequeña *slice*, y construirla nos enseñará lo que necesitamos después.

## Cuándo no usarlo

_Slice-First_ puede ser riesgoso cuando:

* el dominio es mayormente desconocido
* el proceso de negocio está fragmentado o poco claro
* el costo de construir algo incorrecto es alto
* la *slice* afecta *workflows* críticos
* la *slice* puede crear compromisos arquitectónicos irreversibles
* el equipo no puede validar el resultado después de la entrega
* el contexto circundante es demasiado débil para definir una *slice* segura
* las partes interesadas pueden tratar la *slice* como solución final
* la *slice* depende de reglas de negocio no resueltas
* la *slice* tocaría muchos flujos o responsabilidades adyacentes

En esos casos, Context-First o Problem-First pueden ser más apropiados.

_Slice-First_ también puede ser innecesario cuando el problema ya está bien entendido y el equipo puede implementar la mejora directamente sin necesitar una *slice* de aprendizaje.

## Características

_Slice-First_ normalmente tiene estas características:

* base contextual inicial pequeña
* movimiento rápido hacia la implementación
* aprendizaje mediante *software* funcionando
* alcance estrecho
* orientación fuerte al *feedback*
* conciencia explícita del riesgo
* baja ceremonia
* alta sensibilidad a restricciones de implementación
* preferencia por integración vertical por sobre modelado amplio
* disposición a refinar el entendimiento después de la entrega

_Slice-First_ no significa construir al azar. Significa construir una *slice* pequeña e intencional con suficiente entendimiento para hacer que el aprendizaje sea seguro.

## Ventajas

_Slice-First_ ayuda al equipo a:

* aprender rápidamente desde implementación real
* evitar sobreanalizar antes del *feedback*
* validar dirección técnica temprano
* validar dirección de producto temprano
* exponer restricciones de integración
* revelar desconocidos que solo aparecen durante el desarrollo
* reducir incertidumbre mediante *software* funcionando
* crear progreso visible
* mantener alcance pequeño
* evitar diseñar una solución grande desde supuestos no probados

Es especialmente valioso cuando el mayor riesgo es pasar demasiado tiempo analizando algo que podría aprenderse desde una implementación pequeña.

## Desventajas

_Slice-First_ también tiene costos. Puede:

* explorar insuficientemente el dominio circundante
* construir desde supuestos débiles
* producir implementación desechable
* crear forma arquitectónica prematura
* ocultar complejidad de dominio detrás de una demo funcional
* confundir *feedback* de prototipo con entendimiento del dominio
* crear soluciones locales que no escalan conceptualmente
* perder impacto de negocio adyacente
* hacer que las partes interesadas crean que la *slice* está más completa de lo que realmente está
* requerir retrabajo después de que aparece nuevo entendimiento

El principal peligro de _Slice-First_ es tratar el aprendizaje rápido como prueba de entendimiento completo.

Una *slice* puede validar algo, rara vez valida todo.
