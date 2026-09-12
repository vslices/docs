# Tratar PResolver como una abstracción derivada de VSlices

## Estado

Aceptada

## Contexto

VSlices se está desarrollando como una suite de ingeniería de software centrada en preservar la continuidad entre:

* descubrimiento del dominio
* documentación
* razonamiento de diseño
* arquitectura
* implementación
* validación
* evolución

Durante el desarrollo de VSlices, apareció un patrón más amplio. Varias ideas de VSlices parecen útiles más allá de la ingeniería de software:

* modalidades de razonamiento
* documentación progresiva
* decisiones explícitas
* tradeoffs explícitos
* intervenciones acotadas
* salvaguardas
* loops de validación
* continuidad entre comprensión, acción y evolución

Esto creó la posibilidad de definir una metodología más amplia llamada tentativamente PResolver.

Sin embargo, PResolver no debe introducirse como una metodología completamente independiente antes de que VSlices se valide.

Domus Orbis y otros proyectos de software validan VSlices como una especialización de ingeniería de software. No validan directamente PResolver como una metodología general de resolución de problemas.

## Decisión

Trataremos PResolver como una abstracción extraída de VSlices.

VSlices sigue siendo la suite concreta de ingeniería de software. PResolver representa la estructura más amplia de resolución de problemas que puede abstraerse de VSlices si su razonamiento, documentación y patrones de método demuestran ser útiles.

La dirección práctica es:

```text
Construir VSlices
-> validar VSlices en software
-> observar patrones recurrentes
-> eliminar supuestos específicos de software
-> definir PResolver v0.1
-> probar PResolver en otros dominios
```

> No trataremos PResolver como el producto principal en esta etapa.
>
> No crearemos un PResolver Framework.
>
> No moveremos conceptos de VSlices Framework a PResolver a menos que sobrevivan a la abstracción fuera del software.

## Fundamento

Esto preserva el enfoque.

VSlices es concreto, técnico y actualmente accionable. PResolver es más amplio, más abstracto y menos validado.

Al extraer PResolver desde VSlices en lugar de inventarlo por adelantado, evitamos crear una metodología genérica desconectada de la práctica.

Esto también le da a PResolver un camino de validación más saludable. La pregunta no es:

> ¿Puede Domus Orbis validar PResolver?

La pregunta es:

> Si VSlices funciona en software, ¿qué partes de su razonamiento, documentación y estructura de método siguen siendo útiles fuera del software?

Esto mantiene a PResolver como algo experimental sin negar su potencial.

## Consecuencias

La documentación de VSlices debe seguir enfocándose en ingeniería de software.

PResolver puede aparecer dentro de Alive Lab como una teoría exploratoria.

PResolver v0.1 puede documentar más adelante la abstracción reutilizable detrás de:

* PResolver Method
* PResolver Design
* PResolver Docs Standard

Estos deben tratarse como posibles productos futuros, no como compromisos actuales.

La relación debe expresarse como:

```text
VSlices valida una especialización de software.
PResolver abstrae la estructura reutilizable.
Otros dominios prueban la abstracción.
```

## Tradeoffs

Esta decisión retrasa el posicionamiento público de PResolver.

Eso es aceptable porque una productización prematura podría debilitar VSlices.

Esta decisión también significa que PResolver no recibirá documentación completa de inmediato.

Eso es aceptable porque la primera prioridad sigue siendo VSlices.

El beneficio es que PResolver puede crecer a partir de patrones observados en lugar de especulación.

## Riesgos

PResolver puede volverse demasiado genérico si abstraemos de manera demasiado agresiva.

VSlices puede volverse más difícil de explicar si PResolver se introduce demasiado pronto.

La abstracción puede fallar fuera del software.

Algunos patrones de VSlices pueden no generalizar bien.

También existe el riesgo de crear un segundo universo de documentación antes de que el primero sea estable.

## Salvaguardas

PResolver debe seguir siendo exploratorio hasta que existan suficientes ejemplos fuera del software.

VSlices sigue siendo el foco principal del producto.

PResolver no debe reintroducir conceptos en VSlices a menos que aclaren el trabajo de ingeniería de software existente.

No debe crearse un PResolver Framework en la etapa actual.

PResolver debe documentarse primero como una teoría de Alive Lab, no como una sección de producto.

## Validación

Esta decisión se considera válida mientras:

* VSlices siga siendo más fácil de explicar como una suite de ingeniería de software
* PResolver ayude a explicar patrones más amplios sin quitar foco
* los conceptos de PResolver puedan extraerse del trabajo real de VSlices
* no se introduzca prematuramente una estructura de framework o producto
* experimentos futuros puedan probar PResolver fuera del software

Esta decisión debería revisarse si:

* PResolver obtiene validación repetida fuera del software
* la documentación de VSlices se ve limitada por lenguaje específico de software
* las ofertas de servicio requieren un marco más amplio de resolución de problemas
* PResolver empieza a requerir su propia estructura estable de documentación
