# Glosario de VSlices Framework

Este glosario define términos usados por VSlices Framework.

VSlices Framework se enfoca en implementar software orientado al dominio con comportamiento explícito, errores explícitos, composición funcional, arquitectura progresiva y baja ceremonia.

Estos términos ayudan a conectar conocimiento de dominio, comportamiento de aplicación, requisitos de runtime y estructura ejecutable.

## Conceptos de ejecución

- __Flow__: una composición ejecutable que describe cómo el trabajo, los datos, el comportamiento, las dependencias y los errores esperados se mueven a través de una operación.

- __Feature__: un comportamiento, acción o vertical slice concreto que entrega valor o apoya una necesidad validada dentro de un contexto de dominio.

- __Step__: una pequeña unidad de comportamiento ejecutable dentro de un flow, normalmente responsable de una transformación significativa, validación en runtime, decisión o efecto secundario.

- __Pipeline__: una composición ordenada de pasos, comportamientos, efectos, validaciones en runtime o transformaciones que producen un resultado.

## Conceptos de modelado de dominio

- __Domain Type__: un valor fuertemente modelado que representa un concepto de dominio con validación explícita en runtime, significado e invariantes.

- __Invariant__: una regla que debe permanecer verdadera para que un domain type, comportamiento, capability o estado se considere válido.

- __Runtime validation__: el acto de comprobar si un valor, comportamiento, comando, solicitud o estado satisface las reglas esperadas antes de continuar.

- __Expected error__: una condición de fallo conocida que pertenece al dominio o al flujo de la aplicación y debe modelarse explícitamente en lugar de tratarse como una excepción inesperada.

- __Unexpected error__: una falla que no formaba parte del flujo esperado del dominio o de la aplicación, normalmente causada por infraestructura, defectos, dependencias no disponibles o supuestos inválidos.

## Conceptos de composición

- __Capability__: una capacidad estable requerida por el negocio o el sistema. En Framework, una capability puede representarse mediante contratos explícitos, implementaciones, dependencias o comportamientos componibles.

- __Trait__: una unidad componible de comportamiento o capacidad que puede adjuntarse, combinarse o reutilizarse sin depender de modelos fuertemente basados en herencia.

- __Effect__: una representación explícita de trabajo que puede requerir dependencias, producir resultados, fallar o interactuar con el mundo externo.

- __Functional composition__: la práctica de construir comportamiento componiendo funciones más pequeñas, efectos, validaciones en runtime y transformaciones en estructuras ejecutables mayores.

- __Runtime requirement__: una dependencia explícita o requisito de entorno necesario para un flow, feature, effect u operación durante la ejecución.

## Conceptos de integración

- __Integrator__: un mecanismo que invoca una feature desde un estilo de interacción específico, como un endpoint HTTP, comando CLI, tarea en background, acción de UI, tarea programada o manejador de eventos.

- __Adapter__: una implementación específica de tecnología que conecta los conceptos de VSlices con frameworks, bibliotecas, plataformas, infraestructura o proveedores externos.

- __Provider__: una fuente externa o interna de capability usada por un adapter, feature, integración o comportamiento de runtime.

- __Port__: un contrato explícito que describe una necesidad de interacción entre una feature, capability, adapter, provider o boundary de runtime sin obligar al comportamiento de dominio a depender de una tecnología o estilo específico de infraestructura.

## Conceptos de error y resultado

- __Result__: un resultado explícito de una operación, normalmente representando éxito o fallo sin requerir excepciones para el control normal del flujo.

- __Error as value__: la práctica de representar fallos esperados como valores explícitos que pueden componerse, retornarse, evaluarse, registrarse, probarse y documentarse.

- __Failure path__: la ruta que toma una operación cuando un expected error, un fallo de validación en runtime, un problema de dependencia o un problema inesperado impide la finalización normal.

- __Success path__: la ruta que toma una operación cuando todas las validaciones requeridas en runtime, dependencias, decisiones y efectos se completan como se esperaba.

## Relación entre los términos

VSlices Framework intenta mantener el software ejecutable cerca de la intención del dominio.

```text
Domain Type
-> Feature
-> Flow
-> Runtime requirement
-> Expected error
-> Result
```

Esto no significa que cada implementación necesite todos los conceptos. Una feature pequeña puede necesitar solo un domain type, un flow simple y un result explícito. Más estructura solo debería aparecer cuando el dominio, el comportamiento o las necesidades de runtime lo justifiquen.

El objetivo no es añadir ceremonia de framework. El objetivo es hacer que el comportamiento, las dependencias, los errores y el significado del dominio sean lo suficientemente explícitos como para poder componerse, probarse y evolucionar con seguridad.
