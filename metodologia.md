# Metodologia

**Periodismo de Datos II: Herramientas Digitales para la Visualización y Presentacion de Datos**

En el transcurso de las clases de **Datos II** nos adentramos en un mundo totalmente nuevo en donde descubrimos novedosas plataformas y herramientas para el desarrollo web y la visualización de datos. Aunque nuestra sección curso varias materias de programación y llegamos a usar uno que otro lenguaje de programación como *HTML*, no habíamos tenido un contacto tan de cerca con el lenguaje **Python** o **Markdown**, tampoco habíamos usado plataformas como **GitHub**, **Anaconda** o **Jupyter**.

Estas herramientas antes mencionadas fueron de vital importancia la construcción de esta página web, que aunque un poco minimalista, si se puede decir así posee las actividades trabajadas durante la materia.

- [Actividad 1](ad1.md): Introducción al lenguaje Markdown y GitHub
- [Actividad 2](ad2.md): Prácticas de Markdown
- [Actividad 3](ad3.md): Ejercicio de Scraping Web en lenguaje Python e introducción a Jupyter
- [Actividad 4](ad4.md): Visualización de Datos y gráficas desde Jupyter

***

## Actividad 1

Para la primera actividad de la materia, el profesor nos dejó como asignación escribir un comentario crítico sobre periodismo de datos, visualización de datos o infografía de entre 300 y 500 palabras. 

Este texto debía ser elaborado desde la plataforma [pad](https://pad.riseup.net/p/nebrija-2223-keep), la cual es una aplicación que nos brinda la posibilidad de escribir textos de forma colaborativa grupal en tiempo real que no almacena la **IP** de los participantes. 

Este ejercicio tenía como fin que al momento de subir el material a la plataforma cooperativa, debíamos añadir los atributos correspondientes al lenguaje **Markdown**.

### Markdown

Este **Lenguaje de programación basado en texto plano** tienen la finalidad de optimizar la legibilidad y de facilitar la publicación del documento elaborado con la misma. Esta se distribuye como plug-in (o al menos está disponible) en diferentes sistemas de gestión de contenidos (CMS).

**Encabezados**

Para crear un encabezado debemos añadir una almohadilla o hashtag `#` frente a un texto, la cantidad de símbolo dependerá de la jerarquía del título. 


```python
# Encabezado h1 
## Encabezado h2
### Encabezado h3
#### Encabezado h4
##### Encabezado h5
###### Encabezado h6
```

**Citas**

si queremos insertar una cita usaremos el símbolo `>`frente al texto 


```python
> No busques los errores, busca un remedio. - Henry Ford
```

> No busques los errores, busca un remedio. - Henry Ford

**Texto con énfasis**

Para enfatizar un texto con letras cursiva o negrita se debe poner de lado a lado un asterisco `*` para la primera opción y dos `**` para la segunda.


```python
*Texto* (cursiva)

**Texto** (negrita)
```

**Código** 

Para identificar los códigos de lenguaje de programación utilizamos el acento grave ```


```python
``` [language]
Código en 
varias líneas
```
```

**Listas**

Para crear una lista no numérica usamos un guion `-`.



```python
- Texto
- Texto
- Texto
```

- Texto
- Texto
- Texto

**Enlaces**

para enlazar una **url** a una palabra debemos escribir entre corchetes `[]` la palabra o frase a la que se le añadirá el **hipervínculo** y entre paréntesis `()`el url.


```python
[Texto del enlace aquí](URL "Título del enlace")
```

**Imágenes**

para añadir una imagen a nuestro documento añadiremos un signo de admiración `!` una pequeña descripción de la foto entre corchetes `[]` y entre paréntesis `()` la dirección de la imagen


```python
![Texto alternativo](URL "Título de la imagen")
```

Luego de escribir nuestra opinión debemos debíamos subir esta asignación en la plataforma **GitHub**

### GitHub

Es una plataforma online para el desarrollo colaborativo, en donde se pueden alojar proyectos y crear códigos fuentes.

Aquí **creamos la página** que enlaza todos los proyectos hechos durante las clases

El proceso de creación comenzó generando una cuenta en la plataforma **GitHub** la cual nos sirvió para alojar y gestar [nuestro proyecto](https://nebrijas.github.io/2022online-Gabriela/). 

#### Creación de repositorio 

Luego de esto generamos nuestro **repositorio**, llamado [2022online-Gabriela](https://nebrijas.github.io/2022online-Gabriela/)

Estos son un espacio donde se almacenan, organizan, difunden y mantiene la información digital. 

Al momento de crear esta entrada creamos un archivo `.md` llamado automáticamente **README**, la cual será nuestra **página home** del proyecto.  

Luego editamos el contenido de la entrada y escribimos en lenguaje **Markdown** la información que queremos que salga en nuestra página principal

En este caso escribimos un titular, un texto y los títulos de las entradas con sus hipervínculos que los enlazaban directamente a la página de la actividad correspondiente 

```
# Trabajos de Clases de Periodismo de Datos II Herramientas dirigitales 
Actividades dirigidas y trabajo final
- [AD1](ad1.md)
- [AD2](ad2.md)
- [AD3](ad3.md)
- [AD4](ad4.md)
- [Metodología](metodologia.md)

```

Y para finalizar, dentro de la [AD1](ad1.md) pegamos el texto trabajado en formato Markdown en la plataforma **pad**

## Actividad 2

La [segunda actividad](ad2.md) fue muy parecida la primera, pues esta tenía la finalidad de que practicáramos la lengua de **Markdown**. Pero a diferencia de la anterior, en esta ya trabajamos el texto directamente en **GitHub** y con una mayor cantidad de palabras. 

En esta asignación analicé un reportaje de datos Titulado [¿Qué tan democrática es República Dominicana frente a otros países de Latinoamérica?](https://eldinero.com.do/208353/que-tan-democratica-es-republica-dominicana-frente-a-otros-paises-de-latinoamerica/) del periódico financiero online "**elDinero**" en donde se desglosaba la situación actual de los países latinoamericanos en torno a la democracia. 

Un mi caso y tras alguna corrección, eleve el resultado final de la visualización de mi actividad 2 usando un código `iframe` con el cual pude tomar la gráfica de barra y la tabla de datos del reportaje original y ponerlos en mi entrada AD2

```
<div class="flourish-embed" data-src="visualisation/11205434"><iframe scrolling="no" frameborder="0" title="Interactive or visual content" sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation" src="https://flo.uri.sh/visualisation/11205434/embed?auto=1" style="width: 100%; height: 1029.48px;"></iframe><div class="flourish-credit" style="width:100%!important;margin:0 0 4px!important;text-align:right!important;font-family:Helvetica,sans-serif!important;color:#888!important;font-size:11px!important;font-weight:bold!important;font-style:normal!important;-webkit-font-smoothing:antialiased!important;box-shadow:none!important;"><a href="https://public.flourish.studio/visualisation/11205434/?utm_source=showcase&amp;utm_campaign=visualisation/11205434" target="_top" style="display:inline-block!important;text-decoration:none!important;font:inherit!important;color:inherit!important;border:none!important;margin:0 5px!important;box-shadow:none!important;"><img alt="Flourish logo" src="https://public.flourish.studio/resources/bosh.svg" style="font:inherit!important;width:auto!important;height:12px!important;border:none!important;margin:0 2px 0!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;"><span style="font:inherit!important;color:#888!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;">A Flourish data visualization</span></a></div></div>
```

<div class="flourish-embed" data-src="visualisation/11205434"><iframe scrolling="no" frameborder="0" title="Interactive or visual content" sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation" src="https://flo.uri.sh/visualisation/11205434/embed?auto=1" style="width: 100%; height: 1029.48px;"></iframe><div class="flourish-credit" style="width:100%!important;margin:0 0 4px!important;text-align:right!important;font-family:Helvetica,sans-serif!important;color:#888!important;font-size:11px!important;font-weight:bold!important;font-style:normal!important;-webkit-font-smoothing:antialiased!important;box-shadow:none!important;"><a href="https://public.flourish.studio/visualisation/11205434/?utm_source=showcase&amp;utm_campaign=visualisation/11205434" target="_top" style="display:inline-block!important;text-decoration:none!important;font:inherit!important;color:inherit!important;border:none!important;margin:0 5px!important;box-shadow:none!important;"><img alt="Flourish logo" src="https://public.flourish.studio/resources/bosh.svg" style="font:inherit!important;width:auto!important;height:12px!important;border:none!important;margin:0 2px 0!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;"><span style="font:inherit!important;color:#888!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;">A Flourish data visualization</span></a></div></div>

## Actividad 3

En la actividad 3 nos dispusimos a redactar una documento con lenguaje **Python** a través de la plataforma de **Jupyter** sobre un `Scraping Web` que sintetiza la búsqueda y obtención de los titulares del periódico digital El País. 

Para lograr eso, el profesor nos facilitó el **código fuente* a desglosar, en el que teníamos que ir explicando paso por paso y funciones que se aplicaron dentro del código. 

**Scraping Web**

Scraping Web o rasgado se refiero a una técnica usada a través de programas de software para extraer información de una página web.


```python

```


```python

```

### Python

### Anaconda

#### Jupyter

## Actividad 4
