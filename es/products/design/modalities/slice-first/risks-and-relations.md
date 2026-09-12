# Riesgos y *tradeoffs*

_Slice-First_ es útil, pero puede fallar cuando se confunde velocidad con claridad. Riesgos comunes incluyen:

* implementación ciega
* entendimiento de dominio débil
* arquitectura accidental
* compromisos técnicos prematuros
* código desechable que se vuelve permanente
* validación superficial
* sobreajuste a un solo camino
* impacto de negocio adyacente faltante
* sesgo de prototipo
* malentendido de partes interesadas
* ignorar *feedback* porque la *slice* parece funcionar
* tratar la implementación como prueba de corrección de producto

Para evitar estos riesgos, el equipo debería mantener la *slice* pequeña, explícita y reversible cuando sea posible. Debería preguntar:

* ¿Qué estamos intentando aprender?
* ¿Qué supuestos estamos aceptando?
* ¿Qué riesgos estamos postergando?
* ¿Qué invalidaría esta *slice*?
* ¿Qué haría insegura esta *slice*?
* ¿Qué haría que esta *slice* se vuelva accidentalmente permanente?
* ¿La *slice* sigue siendo lo suficientemente pequeña?
* ¿El *feedback* es lo suficientemente real?
* ¿Deberíamos seguir construyendo o cambiar de modalidad?

_Slice-First_ debería crear aprendizaje rápido. No debería convertirse en una excusa para saltarse el pensamiento o hacer mal trabajo.

# Relación con otras modalidades

_Slice-First_ no siempre es la mejor modalidad. Es mejor cuando el *feedback* rápido de implementación es más valioso que análisis adicional por adelantado.

Un equipo puede empezar con Context-First para entender un dominio amplio, moverse a Problem-First cuando un problema concreto se vuelve claro, y luego usar _Slice-First_ para validar rápidamente una implementación pequeña.

Un equipo también puede empezar con _Slice-First_ cuando el dominio ya está suficientemente entendido y la principal incertidumbre es práctica:

* ¿Esto puede implementarse?
* ¿Los usuarios interactuarán con esto como esperamos?
* ¿Esta integración funciona?
* ¿Este *workflow* es viable?
* ¿Esta pequeña *feature* produce el *feedback* esperado?

Después de Building, el equipo puede volver a Problem-First o Context-First si la *slice* revela incertidumbre más profunda.

Las modalidades pueden combinarse a través de iteraciones. No son identidades, son estrategias.
