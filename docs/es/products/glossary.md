# Glosario compartido

Este glosario define términos compartidos usados en los productos de VSlices.

Su propósito es preservar un lenguaje común entre VSlices Design, VSlices Docs Standard, VSlices Method y VSlices Framework.

Estos términos ayudan a conectar el descubrimiento del dominio, la documentación, la arquitectura, la implementación y la evolución sin obligar a cada producto a redefinir los mismos conceptos.

## Conceptos de la suite

- __Continuidad__: la preservación del entendimiento a lo largo del descubrimiento, la documentación, el diseño, la arquitectura, la implementación, la validación y la evolución.

- __Intención arquitectónica__: el razonamiento detrás de la estructura arquitectónica, los límites, las decisiones y los tradeoffs que deben seguir siendo comprensibles a medida que el sistema evoluciona.

- __Arquitectura progresiva__: un enfoque en el que la estructura arquitectónica se introduce gradualmente a medida que el dominio, los riesgos y las necesidades de implementación lo justifican.

## Términos centrales de dominio a software

- __Scenario__: responde _¿dónde estamos trabajando?_. Representa el contexto de negocio, organizacional, operativo o del sistema donde se está observando conocimiento. Un scenario puede incluir empresas, ecosistemas, departamentos, sistemas, restricciones, personas y condiciones circundantes.

- __Work Line__: responde _¿qué ofrecemos u operamos?_. Representa un área, departamento, servicio, línea de negocio, flujo de valor u oferta estable dentro de un scenario. Un work line ayuda a identificar lo que la organización proporciona o mantiene.

- __Work Process__: responde _¿cómo lo hacemos?_. Representa las responsabilidades, roles, reglas de coordinación y estructura operativa usadas para ejecutar un work line. Un work process explica cómo personas, áreas o sistemas organizan el trabajo para producir valor.

- __Workflow__: responde _¿qué se hace?_. Representa la secuencia concreta de pasos, decisiones, transferencias y participantes responsables dentro de un work process. Un workflow hace visible cómo el trabajo pasa de un estado, actor, sistema o responsabilidad a otro.

- __Use Case__: responde _¿qué significa este comportamiento?_. Representa la consecuencia esperada, las validaciones, reglas, resultados y significado de dominio de una interacción u operación. Un use case explica por qué un comportamiento importa y qué debe ser verdadero para que sea válido.

## Conceptos de apoyo

- __Actor__: una persona, rol, sistema, organización o participante externo que forma parte de un scenario, work process, workflow o use case.

- __Responsibility__: un deber, decisión, acción o propiedad esperada asignada a un actor, rol, área o sistema.

- __Handoff__: un punto en el que el trabajo pasa de un actor, rol, área, sistema o responsabilidad a otro.

- __Boundary__: un límite que separa contextos, responsabilidades, conceptos, sistemas, decisiones o áreas de propiedad.

- __Capability__: una capacidad estable requerida por el negocio o el sistema. Una capability describe lo que debe ser posible, independientemente de la implementación específica que la proporcione.

- __Feature__: un comportamiento, acción o vertical slice concreto que entrega valor o apoya una necesidad validada dentro de un contexto de dominio.

- __Flow__: un movimiento dirigido de trabajo, datos, comportamiento o control a través de un sistema o proceso. En documentación, un flow puede describir movimiento de negocio. En implementación, puede convertirse en una estructura ejecutable.

## Conceptos de conocimiento

- __Domain Language__: las palabras y significados usados por las personas que entienden u operan el dominio.

- __Assumption__: algo que el equipo cree actualmente que es verdadero, pero que no ha validado por completo.

- __Risk__: una posible fuente de falla, malentendido, costo, retraso, retrabajo o complejidad accidental.

- __Decision__: una dirección seleccionada tomada bajo un contexto específico, con tradeoffs y consecuencias aceptadas.

- __Validation__: evidencia reunida para confirmar, rechazar o refinar una assumption, decision, behavior, document, implementation o product idea.

- __Feedback__: conocimiento producido después de que un documento, decisión, feature, workflow o implementación se usa, revisa, prueba o entrega.

## Relación entre los términos centrales

Los términos centrales normalmente se mueven desde el contexto amplio hacia el comportamiento concreto:

```text
Scenario
-> Work Line
-> Work Process
-> Workflow
-> Use Case
```

Esto no significa que cada iteración deba documentar todos los niveles. La secuencia solo describe cómo el conocimiento puede volverse más específico.

* Un equipo puede comenzar desde un scenario cuando el dominio no está claro.
* Un equipo puede comenzar desde un workflow cuando el trabajo ya es visible.
* Un equipo puede comenzar desde un use case cuando el comportamiento esperado ya se conoce.

La parte importante es mantener el concepto elegido conectado con el conocimiento que lo respalda.
