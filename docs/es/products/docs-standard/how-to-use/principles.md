# Principios

*VSlices Docs Standard* define estructuras de documentación reutilizables para preservar conocimiento a lo largo del ciclo de vida de un sistema de *software*.

No existe para hacer que los equipos produzcan más documentos.

Existe para ayudar a los equipos a preservar el conocimiento del que dependen las decisiones de *software*.

*VSlices Docs Standard* trata la documentación como parte de la continuidad de ingeniería, no como una actividad administrativa separada.

## Idea central

Los sistemas de *software* pierden claridad cuando el entendimiento, la documentación, la arquitectura y la implementación evolucionan por separado.

Un equipo puede:

* entender el dominio durante el descubrimiento, pero perder ese entendimiento al escribir requerimientos
* documentar decisiones, pero perder su conexión con el código
* implementar comportamiento, pero olvidar la intención de negocio que lo justificó
* entregar una *feature*, pero no preservar lo aprendido al construirla

*VSlices Docs Standard* existe para reducir esa fragmentación.

La documentación debería ayudar a futuros lectores a entender no solo *qué* fue decidido o construido, sino también *por qué* existe y *qué conocimiento lo sostiene*.

## Principios

Los principios de VSlices Docs Standard ayudan a decidir cuándo documentar, cuánto estructurar y qué conocimiento vale la pena preservar.

### Documentar para preservar conocimiento útil

La documentación debería existir porque ayuda a tomar mejores decisiones presentes o futuras, no porque una lista de documentos diga que debe existir.

### Mantener continuidad

La documentación debería mantener conectados el entendimiento del dominio, las decisiones, la implementación, la validación y la evolución.

### Usar estructura suficiente

La estructura documental debería ser tan pequeña como sea posible y tan explícita como sea necesario para preservar el conocimiento importante.

### Dar responsabilidad clara a cada documento

Cada documento debería explicar una responsabilidad clara y dejar lo demás a otros documentos.

!!! principle "Principio de Documentación"

    Documenta para preservar conocimiento útil, no para completar una lista de documentos.

## Qué conocimiento debería preservar

Usa los principios para decidir si un documento ayuda a preservar conocimiento que el trabajo futuro podría necesitar.

*VSlices Docs Standard* suele ayudar cuando el equipo necesita preservar:

* lenguaje de dominio
* contexto de negocio
* procesos actuales
* comportamiento esperado
* capacidades
* decisiones
* supuestos
* riesgos
* validación
* feedback
* evolución del sistema

No todos estos elementos necesitan un documento propio.

Lo importante es reconocer qué conocimiento podría perderse si el equipo avanza sin hacerlo explícito.

!!! risk "Riesgo a evitar"

    Más documentación no significa más continuidad. Si un documento no preserva conocimiento útil, puede convertirse en ruido.

