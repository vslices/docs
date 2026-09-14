# VSlices Docs Standard

VSlices Docs Standard define estructuras de documentación reutilizables para preservar conocimiento a lo largo del ciclo de vida de un sistema de software.

No existe para hacer que los equipos produzcan más documentos.

Existe para ayudar a los equipos a preservar el conocimiento del que dependen las decisiones de software.

!!! principle "Principio de Documentación"

    Documenta para preservar conocimiento útil, no para completar una lista de documentos.

## Propósito

VSlices Docs Standard ayuda a los equipos a mantener conectados el entendimiento del dominio, el razonamiento de diseño, la documentación, las decisiones, la implementación, la validación y la evolución.

Su propósito es reducir la pérdida de conocimiento entre lo que el equipo entiende, decide, documenta, construye, valida y cambia.

## Idea central

La documentación debería existir cuando preserva conocimiento necesario para tomar decisiones presentes o futuras.

Un documento no debería crearse porque pertenece al estándar.

Debería crearse porque ayuda a mantener visible una parte importante del contexto, intención, comportamiento, decisión, validación o evolución del sistema.

## Qué proporciona

VSlices Docs Standard proporciona:

* **principios**: ideas que guían cómo debe usarse la documentación
* **modelado de documentos**: reglas para entender notas, documentos, referencias, estados y relaciones
* **taxonomía**: agrupación de documentos según el tipo de conocimiento que preservan
* **caminos de continuidad**: formas de entender cómo se mueve el conocimiento entre documentos, decisiones, implementación y aprendizaje
* **reglas contra la burocracia**: criterios para evitar convertir la documentación en ceremonia
* **estructuras de documento**: formatos reutilizables para tipos comunes de conocimiento de ingeniería

El estándar es intencionalmente progresivo. Un equipo debe usar la estructura más pequeña útil que preserve el conocimiento del que depende el trabajo futuro.

## Cómo usarlo

Empieza por el conocimiento que necesitas preservar.

| Si necesitas preservar...                                                                   | Usa...                                                                                  |
| ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| Conocimiento temprano, incierto, local o temporal                                           | **[Nota de soporte](./taxonomy/support-note.md)**                      |
| Lenguaje que puede afectar el entendimiento, el comportamiento, el nombrado o los límites   | **[Vocabulario de dominio](./taxonomy/domain-vocabulary.md)**     |
| Dónde ocurre el trabajo                                                                     | **[Documento de contexto](./taxonomy/context-document.md)**        |
| Responsabilidades, coordinación, *workflows* o reglas operativas                            | **[Documento de proceso](./taxonomy/process-document.md)**          |   
| Significado explícito de un comportamiento, consecuencias, validaciones o errores esperados | **[Documento de caso de uso](./taxonomy/use-case-document.md)**   |
| Una capacidad estable de la que dependen varios comportamientos o procesos                  | **[Documento de capacidad](./taxonomy/capability-document.md)**  |
| Una elección con *tradeoffs*, consecuencias o impacto futuro significativo                  | **[Registro de decisión](./taxonomy/decision-record.md)**            |
| Evidencia que cambia o confirma conocimiento del que dependerá el trabajo futuro            | **[Nota de validación](./taxonomy/validation-note.md)**              |

!!! risk "Riesgo a evitar"

    No crees un documento porque el estándar lo contiene. Créalo porque preserva conocimiento útil para decisiones presentes o futuras.


## Qué no es

VSlices Docs Standard no es una metodología completa.

* No define el flujo de trabajo completo para ejecutar una iteración
* No requiere que se cree cada documento
* No define reuniones, roles, controles de etapa ni rituales de entrega

Esas preocupaciones pertenecen a VSlices Method.

Docs Standard define los instrumentos. Method define cómo se usan esos instrumentos durante el trabajo real.

## Relación con la VSlices Suite

VSlices Docs Standard es uno de los productos dentro de VSlices Suite.

| Producto                                       | Relación con VSlices Docs Standard                                              |
| ---------------------------------------------- | ------------------------------------------------------------------------------- |
| **[VSlices Design](../design/index.md)**       | Define cómo los equipos razonan sobre el diseño.                                |
| **[VSlices Method](../method/index.md)**       | Define cómo los equipos aplican diseño y documentación durante el trabajo real. |
| **[VSlices Framework](../framework/index.md)** | Puede reflejar ese conocimiento en la implementación.                           |

Docs Standard es independiente de VSlices Framework. Un equipo puede usar estos documentos con cualquier tecnología, arquitectura, lenguaje o proceso de entrega.
