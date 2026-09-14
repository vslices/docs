---
type: research-question
state: candidate
code: RQ-008

related_questions:
* RQ-001
* RQ-002
* RQ-004
* RQ-005
* RQ-007

related_notes: []

related_synthesis:
* SYN-0001

related_studies:
* STU-007

affects:
* VSlices Research
* VSlices Framework
* VSlices Docs Standard
* VSlices Method
* VSlices Tooling
---

# RQ-008 — Realización semántica en VSlices Framework

## Pregunta

¿En qué condiciones una realización de software puede preservar la intención, los límites semánticos y la autoridad definidos en el dominio, permitiendo que la separación física emerja sólo cuando las fuerzas reales la justifiquen?

## Estado

candidate

## Origen

Esta pregunta surge de la definición inicial de VSlices Framework como una capa semántica e interpretativa entre la intención preservada documentalmente y sus realizaciones técnicas.

Framework propone reducir el espacio de interpretaciones válidas mediante conceptos, relaciones, restricciones y criterios explícitos. Entre sus principios provisionales se encuentran:

* la división semántica precede a la división física;
* arquitectura de proyecto, solución y despliegue son niveles distintos;
* Productos y Servicios organiza responsabilidades de solución;
* coherencia, cohesión y acoplamiento permiten evaluar fronteras;
* reducir acoplamiento no debe duplicar autoridad, reglas ni fuentes de verdad;
* una realización concreta debe ser reemplazable sin perder el significado que debía preservar.

## Problema observado

Una intención puede estar documentada, pero aun así traducirse a software de maneras incompatibles o difíciles de explicar.

En particular, es frecuente confundir una frontera lógica con una obligación técnica de crear proyectos, repositorios, bases de datos, procesos o despliegues independientes. También puede ocurrir lo inverso: una solución físicamente separada conserva dependencias implícitas, ownership ambiguo o fuentes de verdad duplicadas.

La pregunta busca observar cómo preservar significado durante la realización sin convertir Framework en una arquitectura única, una biblioteca obligatoria ni una traducción automática de documentos a código.

## Hipótesis inicial

Hacer explícitas las responsabilidades, límites, autoridad, relaciones y criterios de evaluación podría permitir realizaciones progresivas más explicables y reemplazables.

La utilidad dependería de que esos conceptos orienten decisiones reales sin imponer separación prematura, métricas mecánicas o certezas que la evidencia todavía no sostiene.

## Qué busca observar esta pregunta

Esta pregunta busca observar si Framework ayuda a:

* explicar por qué existe una pieza y qué responsabilidad posee;
* distinguir límites semánticos de sus realizaciones físicas;
* asignar y conservar ownership de reglas, datos e invariantes;
* detectar cuándo una dependencia es necesaria, accidental u oculta;
* evaluar fronteras mediante coherencia, cohesión y acoplamiento;
* evitar que el desacoplamiento duplique autoridad o fuentes de verdad;
* decidir progresivamente cuándo una frontera lógica requiere una representación física;
* preservar continuidad entre intención, arquitectura, implementación y evolución.

También busca observar cuándo esos conceptos son insuficientes, ambiguos o introducen ceremonial sin valor.

## Mecanismos candidatos

Los mecanismos candidatos de Framework incluyen:

* arquitecturas de solución, inicialmente Productos y Servicios;
* distinción entre arquitecturas de proyecto, solución y despliegue;
* responsabilidades explícitas de Productos, Servicios, Dependencies y Nexus;
* criterios de coherencia, cohesión y acoplamiento;
* límites de consistencia, invariantes y autoridad exclusiva cuando correspondan;
* declaraciones explícitas de garantías, supuestos y decisiones abiertas;
* documentación y tooling como apoyo a la interpretación, no como sustitutos del juicio humano.

## Evidencia inicial disponible

La evidencia inicial es conceptual y proviene de:

* la definición provisional de VSlices Framework;
* los criterios de organización arquitectónica;
* la arquitectura de solución Productos y Servicios;
* los patrones provisionales Feature, Rule y Consistency Boundary;
* [STU-007 — Continuidad entre sistemas heredados y adopción parcial de VSlices Framework](../studies/stu-007-continuidad-sistemas-heredados-adopcion-parcial-vslices-framework.md);
* las RQs de continuidad documental relacionadas.

STU-007 ofrece un caso institucional anonimizado donde la migración busca dar continuidad a productos existentes, no introducir una separación física por defecto.

## Evidencia faltante

Todavía falta observar:

* si la intención preservada permite distinguir interpretaciones incompatibles en decisiones reales;
* qué información documental mínima necesita Framework para orientar una realización;
* cuándo un Producto, Servicio, Dependency o Nexus representa una frontera útil;
* cuándo una frontera lógica debe mantenerse dentro de la misma realización física;
* qué fuerzas justifican extraer una frontera hacia módulo, repositorio, proceso, persistencia o despliegue;
* cómo se preserva autoridad sin duplicar reglas o datos;
* si los criterios de coherencia, cohesión y acoplamiento son comprensibles y aplicables;
* qué garantías pueden verificarse de forma independiente de una plataforma;
* qué parte de la interpretación puede volverse determinista o asistida por tooling e IA.

## Posibles casos de estudio

El caso inicial es STU-007. Allí se observará una migración progresiva de productos existentes hacia una arquitectura de Productos y Servicios, manteniendo la evidencia institucional anonimizada.

Otros estudios podrán aportar evidencia cuando involucren una realización con un problema práctico propio, no como requisito previo para fragmentar el caso actual.

## Riesgos metodológicos

### Riesgo de confirmar la arquitectura por diseño

El estudio no debe interpretar toda mejora como evidencia a favor de Framework ni todo problema como una aplicación deficiente.

### Riesgo de confundir organización física con calidad

Separar repositorios, procesos o bases de datos no prueba por sí mismo que exista una frontera semántica coherente.

### Riesgo de mecanizar criterios

Coherencia, cohesión y acoplamiento no deben transformarse en una puntuación que sustituya el juicio contextual y la evidencia.

### Riesgo de atribución única

Las diferencias observadas pueden depender de experiencia, tecnología, presión de entrega, contexto institucional o disponibilidad de conocimiento, además de VSlices.

### Riesgo de privacidad

La evidencia disponible puede ser resumida o sintética, lo que limita la verificabilidad externa y exige distinguir observación, inferencia e interpretación.

## Relación con Framework

Esta pregunta puede afectar:

* la definición de Framework como capa semántica e interpretativa;
* la relación entre Docs Standard y Framework;
* la formalización de Productos y Servicios;
* la distinción entre niveles arquitectónicos;
* los criterios de organización arquitectónica;
* las garantías y límites de patrones;
* las condiciones para separación física progresiva;
* tooling determinista y realización asistida por IA.

## Límite actual

Esta pregunta no asume que VSlices Framework preserva continuidad por definición ni que una sola migración pueda validarlo universalmente.

Mientras no exista evidencia analizada, su estado debe mantenerse como `candidate`. Sus resultados deberán formular condiciones, tensiones y límites locales antes de convertirse en reglas o garantías del producto.
