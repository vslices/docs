# Definición de soporte de idioma de primera clase

## Estado

Aceptada.

## Contexto

La documentación de VSlices está evolucionando hacia su primer v0.1 público.

Hasta ahora, la documentación se ha escrito principalmente en inglés para apoyar el alcance internacional. Sin embargo, VSlices también nace de un contexto de habla hispana, y algunos lectores podrían quedar bloqueados para comprender el proyecto si el inglés es la única puerta de entrada disponible.

Esto crea una preocupación de producto y documentación:

* VSlices busca enseñar conceptos de ingeniería, no ocultarlos detrás de barreras de idioma.
* El español no debe tratarse como algo secundario.
* La documentación multilingüe no debe añadir una carga de mantenimiento excesiva durante v0.1.
* La estructura de la documentación debe preservar la continuidad entre idiomas.
* Read the Docs ya proporciona soporte nativo para proyectos de traducción.
* MkDocs puede configurarse por idioma mediante archivos de configuración dedicados.
* Las variables de proyecto de Read the Docs pueden usarse para seleccionar la configuración correcta de MkDocs por proyecto.

El objetivo es definir el español como idioma de documentación de primera clase desde el inicio.

## Decisión

VSlices soportará documentación en inglés y español como idiomas de primera clase.

El inglés seguirá siendo por ahora el idioma internacional de documentación por defecto.

El español se mantendrá como idioma oficial de documentación, no como traducción secundaria o informal.

El repositorio de documentación usará organización de idioma basada en carpetas:

```text
docs/
  en/
    index.md
    start-here/
    products/

  es/
    index.md
    start-here/
    products/
```

Cada idioma puede tener su propia configuración de ReadTheDocs y MkDocs:

```text
mkdocs.en.yml
mkdocs.es.yml
```

Read the Docs usará proyectos de traducción nativos:

```text
vslices      -> inglés
vslices-es   -> proyecto de traducción al español
```

Ambos proyectos de Read the Docs pueden apuntar al mismo repositorio.

La configuración activa de MkDocs se seleccionará mediante un `.readthedocs.yaml` específico. El desarrollo local puede usar tres configuraciones:

```text
es/.readthedocs.yaml -> docs en español
.readthedocs.yaml    -> docs en inglés

mkdocs.local.yml -> vista previa local multilingüe
mkdocs.en.yml    -> vista previa solo en inglés
mkdocs.ess.yml   -> vista previa solo en español
```

## Fundamento

Usar organización de idioma basada en carpetas le da a cada idioma su propio espacio de documentación. Esto se prefiere frente a archivos basados en sufijos como:

```text
index.md
index.es.md
```

Porque la documentación de VSlices no es solo material de referencia de API. Contiene:

* filosofía
* definiciones de producto
* razonamiento de diseño
* documentación del método
* términos del glosario
* decisiones
* ejemplos
* explicaciones educativas

La documentación en español puede preservar la misma intención que la documentación en inglés sin ser siempre una traducción literal frase por frase.

La regla deseada es:

```text
Misma estructura conceptual.
Intención equivalente.
No necesariamente traducción literal.
```

Esto apoya un modelo multilingüe más saludable. Los documentos en inglés y español normalmente deben compartir la misma ruta relativa:

```text
docs/en/products/framework/index.md
docs/es/products/framework/index.md
```

Esto preserva la trazabilidad entre idiomas y al mismo tiempo permite que cada idioma exprese las ideas de forma natural.

## Consecuencias

Esta decisión permite que VSlices:

* ofrezca a lectores de habla hispana un punto de entrada real
* preserve la accesibilidad internacional mediante el inglés
* evite duplicar repositorios
* mantenga el soporte nativo de idioma de Read the Docs
* mantenga navegación específica por idioma
* configure explícitamente cada compilación por idioma
* y evolucione las traducciones progresivamente

Esta decisión también introduce responsabilidades de mantenimiento:

* las páginas traducidas pueden desviarse de sus equivalentes en inglés
* la navegación puede necesitar actualizarse por idioma
* los nuevos documentos pueden requerir planificación de traducción
* y cada compilación de idioma debe validarse de forma independiente

Estos tradeoffs se aceptan.

## Principio

El soporte de idioma forma parte de la accesibilidad de la documentación.

VSlices no debe preservar solo la continuidad arquitectónica.

También debe preservar el acceso conceptual para las personas que intentan aprenderlo, evaluarlo y usarlo.
