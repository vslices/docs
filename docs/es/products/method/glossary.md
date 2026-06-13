# Glosario de VSlices Method

Este glosario define términos usados por *VSlices Method*.

*VSlices Method* se enfoca en cómo *VSlices Design*, *VSlices Docs Standard* y *VSlices Framework* pueden usarse durante trabajo real para preservar continuidad a través de descubrimiento, documentación, diseño, arquitectura, implementación, validación y evolución.

Estos términos ayudan a describir cómo los equipos avanzan a través de incertidumbre sin forzar un proceso rígido.

## Conceptos de Method

* **Camino de continuidad** (*Continuity path*): el camino conectado que sigue una pieza de trabajo a través de descubrimiento, razonamiento de diseño, documentación, arquitectura, implementación, validación y evolución.

* **Punto de entrada de trabajo** (*Work entry point*): el lugar donde un equipo comienza una pieza de trabajo, como un escenario, problema, *workflow*, caso de uso, documento, decisión, *slice* de implementación o resultado de validación.

* **Incertidumbre actual** (*Current uncertainty*): la falta de entendimiento más importante que hace riesgosa la siguiente decisión, documento, diseño o implementación.

* **Estructura útil más pequeña** (*Smallest useful structure*): la cantidad mínima de estructura de proceso, documentación, diseño o implementación necesaria para preservar el conocimiento del que depende el trabajo futuro.

* **Guía de Method** (*Method guidance*): orientación práctica para decidir cómo usar los productos de *VSlices* en un contexto de trabajo específico sin imponer un proceso universal.

## Conceptos de orientación de trabajo

* **Trabajo orientado al contexto** (*Context-oriented work*): trabajo que comienza entendiendo el escenario circundante, ambiente de negocio, organización, operación, sistema o restricciones antes de acotarse hacia un problema o implementación específica.

* **Trabajo orientado al problema** (*Problem-oriented work*): trabajo que comienza desde una tensión, necesidad, riesgo, pregunta, falla u oportunidad visible que necesita entenderse antes de decidir qué construir.

* **Trabajo orientado a slice** (*Slice-oriented work*): trabajo que comienza desde una *slice* pequeña y útil de implementación, documentación, validación o entrega para aprender de forma segura desde *feedback* real.

* **Trabajo orientado a validación** (*Validation-oriented work*): trabajo que comienza desde la necesidad de confirmar, rechazar o refinar un supuesto, decisión, documento, comportamiento, implementación o idea de producto.

* **Trabajo orientado a evolución** (*Evolution-oriented work*): trabajo que comienza desde cambiar, extender, corregir, reemplazar o mejorar conocimiento, documentación, arquitectura o implementación existente.

## Conceptos de continuidad

* **Preservación de conocimiento** (*Knowledge preservation*): el acto de mantener entendimiento importante disponible para trabajo futuro, especialmente cuando decisiones, comportamientos, límites, riesgos o validaciones podrían olvidarse.

* **Retorno de conocimiento** (*Knowledge return*): el acto de traer aprendizaje desde implementación, validación, uso, revisión o *feedback* de vuelta hacia documentación, razonamiento de diseño, decisiones y trabajo futuro.

* **Ruptura de continuidad** (*Continuity break*): un punto donde descubrimiento, documentación, razonamiento de diseño, arquitectura, implementación, validación o evolución se desconectan entre sí.

* **Ciclo de continuidad** (*Continuity loop*): el movimiento recurrente desde entendimiento hacia documentación, diseño, implementación, validación, aprendizaje y entendimiento mejorado.

* **Trabajo trazable** (*Traceable work*): trabajo cuyo contexto, decisiones, comportamiento, documentación, implementación, validación y cambios futuros todavía pueden seguirse después de que el trabajo se completa.

## Conceptos de adopción

* **Adopción progresiva** (*Progressive adoption*): adoptar productos, documentos, patrones o prácticas de *VSlices* gradualmente según necesidad real, en vez de intentar usar toda la suite de una vez.

* **Utilidad local** (*Local usefulness*): el valor que un concepto, documento, método o patrón de implementación de *VSlices* entrega en el contexto actual antes de tratarse como generalmente útil.

* **Estructura suficiente** (*Enough structure*): la cantidad de estructura necesaria para reducir confusión, preservar intención, apoyar decisiones o habilitar evolución segura sin agregar ceremonia innecesaria.

* **Sobreestructuración** (*Over-structuring*): agregar más estructura de proceso, documentación, abstracción, arquitectura o *framework* de la que justifica la incertidumbre actual o necesidad del dominio.

* **Subestructuración** (*Under-structuring*): usar muy poca estructura para preservar conocimiento importante, causando que el trabajo futuro dependa de memoria, explicaciones repetidas o supuestos frágiles.

## Relación entre los términos

*VSlices Method* ayuda a los equipos a decidir cómo avanzar a través del trabajo mientras preservan continuidad.

```text id="bnor3e"
Work entry point
-> Current uncertainty
-> Smallest useful structure
-> Knowledge preservation
-> Implementation or validation
-> Knowledge return
-> Continuity path
```

Esta no es una secuencia obligatoria. Un equipo puede comenzar desde contexto, un problema, una *slice*, un documento, una implementación existente, una decisión o *feedback* de validación.

Lo importante es que el trabajo permanezca conectado al conocimiento que explica por qué existe, cómo debería evolucionar y de qué depende el trabajo futuro.
