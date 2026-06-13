# VSlices Docs Standard

VSlices Docs Standard define estructuras de documentación reutilizables para preservar conocimiento a lo largo del ciclo de vida de un sistema de software.

Su propósito es ayudar a los equipos a mantener conectados el entendimiento del dominio, la documentación, el razonamiento de diseño, las decisiones, el comportamiento de implementación, la validación y la evolución.

VSlices Docs Standard no existe para hacer que los equipos produzcan más documentos. Existe para ayudar a los equipos a preservar el conocimiento del que dependen las decisiones de software.

## Qué proporciona

VSlices Docs Standard proporciona:

- __principles__: las ideas que guían cómo debe usarse la documentación.
- __document modeling__: cómo funcionan las notas, los documentos, las referencias, los estados y las relaciones.
- __taxonomy__: cómo se agrupan los documentos según el tipo de conocimiento que preservan.
- __continuity paths__: cómo se mueve el conocimiento entre documentos, decisiones, implementación y aprendizaje.
- __anti-bureaucracy rules__: cómo evitar convertir la documentación en ceremonia.
- __document structures__: formatos reutilizables para tipos comunes de conocimiento de ingeniería.

El estándar es intencionalmente progresivo. Un equipo debe usar la estructura más pequeña útil que preserve el conocimiento del que depende el trabajo futuro.

## Qué no es

VSlices Docs Standard no es una metodología completa.

- No define el flujo de trabajo completo para ejecutar una iteración.
- No requiere que se cree cada documento.
- No define reuniones, roles, controles de etapa ni rituales de entrega.

Esas preocupaciones pertenecen a VSlices Method. Docs Standard define los instrumentos y Method define cómo se usan esos instrumentos durante el trabajo real.

## Cómo usarlo

Empieza por el conocimiento que necesitas preservar.

* **Usa una Nota de soporte (_Support Note_ en inglés)** cuando el conocimiento sea temprano, incierto, local o temporal.
* **Usa un Vocabulario de dominio (_Domain Vocabulary_ en inglés)** cuando el lenguaje pueda afectar el entendimiento, el comportamiento, el nombrado o los límites.
* **Usa un Documento de contexto (_Context Document_ en inglés)** cuando el equipo necesite preservar dónde ocurre el trabajo.
* **Usa un Documento de proceso (_Process Document_ en inglés)** cuando las responsabilidades, la coordinación, los _workflows_ o las reglas operativas importen.
* **Usa un Documento de caso de uso (_Use Case Document_ en inglés)** cuando el comportamiento necesite significado explícito, consecuencias, validaciones o errores esperados.
* **Usa un Documento de capacidad (_Capability Document_ en inglés)** cuando varios comportamientos o procesos dependen de una capacidad estable.
* **Usa un Registro de decisión (_Decision Record_ en inglés)** cuando una elección tenga tradeoffs, consecuencias o impacto futuro significativos.
* **Usa una Nota de validación (_Validation Note_ en inglés)** cuando la evidencia cambie o confirme conocimiento del que dependerá el trabajo futuro.

No crees un documento porque el estándar lo contiene. Créalo porque preserva conocimiento útil.

## Relación con la suite VSlices

VSlices Docs Standard es uno de los productos dentro de VSlices Suite.

* **VSlices Design** define cómo los equipos razonan sobre el diseño.
* **VSlices Docs Standard** define cómo los equipos preservan distintos tipos de conocimiento.
* **VSlices Method** define cómo los equipos aplican diseño y documentación durante el trabajo real.
* **VSlices Framework** refleja ese conocimiento en la implementación.

Docs Standard es independiente de VSlices Framework. Un equipo puede usar estos documentos con cualquier tecnología, arquitectura, lenguaje o proceso de entrega.
