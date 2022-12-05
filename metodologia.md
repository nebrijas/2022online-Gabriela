# Metodología

**Periodismo de Datos II: herramientas Digitales para la Visualización y Presentación de Datos**

En el transcurso de las clases de **Datos II** nos adentramos en un mundo totalmente nuevo en donde descubrimos novedosas plataformas y herramientas para el desarrollo web y la visualización de datos. Aunque nuestra sección curso varias materias de programación y llegamos a usar uno que otro lenguaje de informático como *HTML*, no habíamos tenido un contacto tan de cerca con el lenguaje **Python** o **Markdown**, tampoco habíamos usado plataformas como **GitHub**, **Anaconda** o **Jupyter**.

Estas herramientas antes mencionadas fueron de vital importancia el desarrollo de las diferentes prácticas. 

Pero una de ellas resalta frente a las demás, **GitHub**, la cual fue de vital importancia para construcción de esta página web, que aunque un poco minimalista, si se puede decir así posee las actividades trabajadas durante la materia.

De acuerdo a lo planteado por la página [developer.mozilla](https://developer.mozilla.org/), **GitHub** es una plataforma online de *social coding* que permite subir repositorios de código almacenarlo en el sistema de control de versiones Git.

Para crear esta página tuve que agotar un pequeño y fácil proceso:
- Entre a la página y me registre con mi mail 
- Seleccione el botón nuevo de la parte superior derecha representado por un símbolo de más
- seleccione nuevo repositorio, al cliquear esta opción nos lleva a una nueva página en donde debemos llenar un formulario con las cualidades de nuestro futuro repositorio.
- Elegimos el Owner, que en este caso al ser un proyecto de la universidad usamos nebrija, nombramos el documento y seleccionamos la opción pública. 
- Para finalizar con el proceso de creación le damos clic a crear repositorio  

Lo siguiente es poner manos a la obra y en el archivo README, el cual se crea instantáneamente con la página, escribir el texto principal de nuestra página y el menú de las diferentes entradas que tendrá nuestra página. Estas entradas estarán enlazadas con las actividades que fuimos subiendo durante las clases. 

***

- [Actividad 1](ad1.md): introducción al lenguaje Markdown y GitHub
- [Actividad 2](ad2.md): prácticas de Markdown
- [Actividad 3](ad3.md): ejercicio de Scraping Web en lenguaje Python e introducción a Jupyter
- [Actividad 4](ad4.md): visualización de Datos y gráficas desde Jupyter

***

## Actividad 1

Para la primera actividad de la materia, el profesor nos dejó como asignación escribir un comentario crítico sobre periodismo de datos, visualización de datos o infografía de entre 300 y 500 palabras. 

Este texto debía ser elaborado desde la plataforma [Riseup Pad](https://pad.riseup.net/p/nebrija-2223-keep), la cual es una aplicación que nos brinda la posibilidad de escribir textos de forma colaborativa grupal en tiempo real que no almacena la **IP** de los participantes. 

Este ejercicio tenía como fin que al momento de subir el material a la plataforma cooperativa, debíamos añadir los atributos correspondientes al lenguaje **Markdown**.

### Markdown

De acuerdo con la página https://markdown.es/, **Markdown** es un **Lenguaje basado en texto plano** que tiene la finalidad de optimizar la legibilidad y de facilitar la publicación del documento elaborado con la misma. Esta se distribuye como plug-in (o al menos está disponible) en diferentes sistemas de gestión de contenidos (Content Management System).

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

`> No busques los errores, busca un remedio. - Henry Ford`

> No busques los errores, busca un remedio. - Henry Ford

**Texto con énfasis**

Para enfatizar un texto con letras cursiva o negrita se debe poner de lado a lado un asterisco `*` para la primera opción y dos `**` para la segunda.

*Texto* (cursiva)

**Texto** (negrita)

**Código** 

Para identificar los códigos de lenguaje de programación utilizamos el acento grave ```


``` [language]
Código en 
varias líneas
```


**Listas**

Para generar una lista no numérica usamos un guion `-`.


- Texto
- Texto
- Texto

**Enlaces**

Para enlazar una **url** a una palabra debemos escribir entre corchetes `[]` la palabra o frase a la que se le añadirá el **hipervínculo** y entre paréntesis `()`el url.

[Texto del enlace aquí](URL "Título del enlace")

**Imágenes**

para añadir una imagen a nuestro documento añadiremos un signo de admiración `!` una pequeña descripción de la foto entre corchetes `[]` y entre paréntesis `()` la dirección de la imagen

`![Texto alternativo](URL "Título de la imagen")`

Luego de escribir nuestra opinión debemos debíamos subir esta asignación en la plataforma **GitHub**

### GitHub

Es una plataforma online para el desarrollo colaborativo, en donde se pueden alojar proyectos y producir códigos fuentes.

Aquí **creamos la página** que enlaza todos los proyectos hechos durante las clases

El proceso de creación comenzó generando una cuenta en la plataforma **GitHub**, la cual nos sirvió para alojar y gestar [nuestro proyecto](https://nebrijas.github.io/2022online-Gabriela/). 

#### Creación de repositorio 

Luego de esto generamos nuestro **repositorio**, llamado [2022online-Gabriela](https://nebrijas.github.io/2022online-Gabriela/)

Estos son un espacio donde se almacenan, organizan, difunden y mantiene la información digital. 

Al momento de producir esta entrada creamos un archivo `.md` llamado automáticamente **README**, la cual será nuestra **página home** del proyecto.  

Luego editamos el contenido de la entrada y escribimos en lenguaje **Markdown** la información que queremos que salga en nuestra página principal

En este caso escribimos un titular, un texto y los títulos de las entradas con sus hipervínculos que los enlazaban directamente a la página de la actividad correspondiente 

```
# Trabajos de Clases de Periodismo de Datos II Herramientas digitales 
Actividades dirigidas y trabajo final
- [AD1](ad1.md)
- [AD2](ad2.md)
- [AD3](ad3.md)
- [AD4](ad4.md)
- [Metodología](metodologia.md)

```

Y para finalizar, dentro de la [AD1](ad1.md) pegamos el texto trabajado en formato Markdown en la plataforma **Riseup Pad**

## Actividad 2

La [segunda actividad](ad2.md) fue muy parecida la primera, pues esta tenía la finalidad de que practicáramos la lengua de **Markdown**. Pero a diferencia de la anterior, en esta ya trabajamos el texto directamente en **GitHub** y con una mayor cantidad de palabras. 

En el ejercicio debíamos realizar un comentario de 500-700 palabras de un artículo o reportaje de periodismo y visualización de datos.

En esta asignación analicé un reportaje de datos Titulado [¿Qué tan democrática es República Dominicana frente a otros países de Latinoamérica?](https://eldinero.com.do/208353/que-tan-democratica-es-republica-dominicana-frente-a-otros-paises-de-latinoamerica/) del periódico financiero online "**elDinero**" en donde se desglosaba la situación actual de los países latinoamericanos en torno a la democracia. 

Esta nota periodística posee un mapa, gráficos de barra y una tabla, de los cuales puede incrustar en el trabajo los dos últimos. 

Un mi caso y tras alguna corrección, eleve el resultado final de la visualización de mi actividad 2 usando un código `iframe` con el cual pude tomar la gráfica de barra y la tabla de datos del reportaje original y ponerlos en mi entrada AD2

```
<div class="flourish-embed" data-src="visualisation/11205434"><iframe scrolling="no" frameborder="0" title="Interactive or visual content" sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation" src="https://flo.uri.sh/visualisation/11205434/embed?auto=1" style="width: 100%; height: 1029.48px;"></iframe><div class="flourish-credit" style="width:100%!important;margin:0 0 4px!important;text-align:right!important;font-family:Helvetica,sans-serif!important;color:#888!important;font-size:11px!important;font-weight:bold!important;font-style:normal!important;-webkit-font-smoothing:antialiased!important;box-shadow:none!important;"><a href="https://public.flourish.studio/visualisation/11205434/?utm_source=showcase&amp;utm_campaign=visualisation/11205434" target="_top" style="display:inline-block!important;text-decoration:none!important;font:inherit!important;color:inherit!important;border:none!important;margin:0 5px!important;box-shadow:none!important;"><img alt="Flourish logo" src="https://public.flourish.studio/resources/bosh.svg" style="font:inherit!important;width:auto!important;height:12px!important;border:none!important;margin:0 2px 0!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;"><span style="font:inherit!important;color:#888!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;">A Flourish data visualization</span></a></div></div>
```

<div class="flourish-embed" data-src="visualisation/11205434"><iframe scrolling="no" frameborder="0" title="Interactive or visual content" sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation" src="https://flo.uri.sh/visualisation/11205434/embed?auto=1" style="width: 100%; height: 1029.48px;"></iframe><div class="flourish-credit" style="width:100%!important;margin:0 0 4px!important;text-align:right!important;font-family:Helvetica,sans-serif!important;color:#888!important;font-size:11px!important;font-weight:bold!important;font-style:normal!important;-webkit-font-smoothing:antialiased!important;box-shadow:none!important;"><a href="https://public.flourish.studio/visualisation/11205434/?utm_source=showcase&amp;utm_campaign=visualisation/11205434" target="_top" style="display:inline-block!important;text-decoration:none!important;font:inherit!important;color:inherit!important;border:none!important;margin:0 5px!important;box-shadow:none!important;"><img alt="Flourish logo" src="https://public.flourish.studio/resources/bosh.svg" style="font:inherit!important;width:auto!important;height:12px!important;border:none!important;margin:0 2px 0!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;"><span style="font:inherit!important;color:#888!important;vertical-align:middle!important;display:inline-block!important;box-shadow:none!important;">A Flourish data visualization</span></a></div></div>

## Actividad 3

En [la actividad 3](ad3.md) nos dispusimos a redactar una documento con lenguaje **Python** a través de la plataforma de **Jupyter**, que abrimos desde **Anaconda**, sobre un `Scraping Web` que sintetiza la búsqueda y obtención de los titulares del periódico digital **El País**.

Para lograr eso, el profesor nos facilitó el **código fuente** a desglosar, en el que teníamos que ir explicando paso por paso y funciones que se aplicaron dentro del código. 

**Scraping Web**

Scraping Web o rasgado se refiero a una técnica usada a través de programas de software para extraer información de una página web.

### Python

De acuerdo a la página web de [platzi](https://platzi.com/blog/python/?utm_source=google&utm_medium=cpc&utm_campaign=18798607679&utm_adgroup=&utm_content=&gclid=CjwKCAiAp7GcBhA0EiwA9U0mtmOIyK6UsbLQnyi2V9uNRmJmeqt5-XL6MKtMEMXFGG7YEP04alnF4xoCddMQAvD_BwE&gclsrc=aw.ds) Python es un lenguaje de alto nivel de programación interpretado. Este puede ser usado en múltiples plataformas, además su código es abierto y libre de uso. Según él [el índice PYPL](https://pypl.github.io/PYPL.html), sé a convertido en la lengua de programación más popular. 

Según [python.org](https://www.python.org/about/apps/) Esta herramienta puede ser utilizada para:
- Desarrollo Web e Internet
- Científico y Numérico
- Educación
- GUI de escritorio
- Desarrollo de software
- Aplicaciones de negocios


### Anaconda

Anaconda es una distribución libre de los lenguajes Python. La cual es usada en ciencia de datos, y aprendizaje automático.

Este es un lenguaje de alto nivel de programación interpretado, con una licencia de código abierto, cuyo fin es la legibilidad de los códigos. Python se emplea para el desarrollo de todo tipo de aplicaciones y juegos.  


#### Jupyter

Es un proyecto sin fines de lucro creado para el desarrollo de software con docenas lenguajes de programación 

Al Abril él programa desde la plataforma de **Anaconda**, creamos una carpeta en donde tendremos nuestro archivo de **Jupyter** juntos y un archivo bajo el lenguaje **Python**. En este punto podemos a trabajar en el código de fuente.   

Para lograr eso, el profesor nos facilitó el código fuente a desglosar, en el que teníamos que ir explicando todos los pasos y funciones que se aplicaron dentro del código. 

En el desarrollo de esta práctica profundizamos en el uso de diferentes funciones, variables y librerías, con las que era posible ejecutar el código fuente para conseguir los resultados. 

#### Pandas

En Computación y Ciencia de datos, pandas es una biblioteca de software escrita como extensión de Numpy para manipulación y análisis de datos para el lenguaje de programación Python

Para iniciar a trabajar debemos tener el [código fuente](docs/codigo_fuente)

Tenemos que instalar las siguientes Librerías para realizar el web scraping

##### Librerías

**Librerías internas**

- [csv](https://docs.python.org/3/library/csv.html): de *comma separated values* o Valores Separados por Comas es el formato muy habitual importación y exportación de hojas de cálculo y bases de datos.
- [re](https://docs.python.org/3/library/re.html): este módulo proporciona operaciones de coincidencia de expresiones regulares similares a las encontradas en Perl.
- [time](https://docs.python.org/es/3/library/time.html): este módulo proporciona varias funciones relacionadas con el tiempo. Para la funcionalidad relacionada, consulte también los módulos datetime y calendar.
- [os](https://docs.python.org/3/library/os.html): este módulo provee una manera versátil de usar funcionalidades dependientes del sistema operativo.

**Librerías externas**

- [termcolor](https://pypi.org/project/termcolor/): es una biblioteca que sirve para imprimir mensajes de colores en el terminal.
- [bs4](https://es.acervolima.com/python-beautifulsoup-encontrar-todas-las-clases/): Beautiful Soup (bs4) es una biblioteca de la cual podemos obtener datos en formato HTML y XML
- [requests](https://cosasdedevs.com/posts/web-scraping-con-requests-y-beautifulsoup-en-python/): se emplea para hacer solicitudes y peticiones a la página de la que extraeremos datos.
- [Pandas](https://pypi.org/project/pandas/): es una herramienta de análisis de datos de código, de lectura rápida en el lenguaje de programación de Python.

Las cuales son instaladas a través de la función `pip install requests bs4 pandas termcolor` 


```python
pip install requests bs4 pandas termcolor
```

    Requirement already satisfied: requests in c:\users\gabri\anaconda3\lib\site-packages (2.28.1)
    Requirement already satisfied: bs4 in c:\users\gabri\anaconda3\lib\site-packages (0.0.1)
    Requirement already satisfied: pandas in c:\users\gabri\anaconda3\lib\site-packages (1.4.4)
    Requirement already satisfied: termcolor in c:\users\gabri\anaconda3\lib\site-packages (2.1.1)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (2022.9.14)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (2.0.4)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (1.26.11)
    Requirement already satisfied: beautifulsoup4 in c:\users\gabri\anaconda3\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: pytz>=2020.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: six>=1.5 in c:\users\gabri\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\gabri\anaconda3\lib\site-packages (from beautifulsoup4->bs4) (2.3.1)
    Note: you may need to restart the kernel to use updated packages.
    

Luego Importamos las librerías para que los siguientes comandos puedan trabajar


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
```

##### Variables 

Creamos una variable llamada **resultado**


```python
resultados = []
```

Para saber qué tipo de variables usamos la función type


```python
type(resultados)
```




    list



El paso siguiente solicitar el acceso de los datos del portal Web para imprimir los titulares **El PAÍS**

#### Solicitud de acceso 


```python
req = requests.get("https://resultados.elpais.com")
```

**get** significa dame la página de **El País** 

Lo que nos dará como resultado **requests.models.Response** que representa la respuesta de **req**

Para solo usar valores iguala a 200 se debe usar el elemnto **if** para que nos muestre solo los estados satisfactorios.

#### Beautiful Soup

Se agrega la variable Beautiful para guardar los *Tags* para que se añadan en lista los títulos

Añadimos la variable para encontrar las **h2** através de un **for** y se impriman las etiquetas y sus textos.


```python
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
```

Luego se crea una variable **soup** donde se encuentra **BeautifulSoup(req.text, 'html.parser')**, lo cual toma el texto, lo analiza

El próximo paso es crear una variable llamada **tags** con la que buscamos todos los **h2** (titulares de las noticias) partir del texto analizado por **BeautifulSoup


```python
soup = BeautifulSoup(req.text, 'html.parser')
tags = soup.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    El Mundial, en vivo
    Universo Mundial
    El calendario a seguir desde América
    ¿Quién va a ganar? Simulador y pronóstico de cada selección 
    La ‘newsletter’
    La paradoja de los Carabineros en Chile: crece la sensación de inseguridad, mejora su apoyo social
    Lula da a su esposa Rosangela Silva protagonismo en la transición en Brasil
    La FIL de Guadalajara recupera fuerza tras el golpe de la pandemia
    El régimen de excepción de Nayib Bukele asfixia a las pandillas: “Policías y soldados tienen poder absoluto” 
    Una esperanza bajo tierra: tras el último rastro de los migrantes desaparecidos rumbo a Estados Unidos
    Tres muertos y 20 desaparecidos por un derrumbe en una vía de Risaralda
    El inagotable debate sobre la cancelación
    Una nueva generación de escritores latinoamericanos restablece los puentes entre América y España
    Un libro en las manos para no sentirse solo
    Las nuevas voces que se abren paso en la FIL de Guadalajara
    Inglaterra supera con comodidad a Senegal y se clasifica a cuartos (3-0)
    Un colosal Mbappé impulsa a Francia a la siguiente fase
    Messi lleva a hombros a Argentina ante Australia (2-1)
    En peligro de objetividad
    Tuteladas, discriminadas: así vive la mujer de Qatar
    La reinvención de la extrema derecha en América Latina
    Las mareas subterráneas de la ola rosa latinoamericana
    El Metro de Bogotá pone la primera piedra tras mil proyectos, cero estaciones y una discusión eterna
    Muere Rafael Cauduro, el muralista mexicano que pintaba “mentiras comprensibles”
    La misoginia dispara los ataques contra las periodistas en México
    Un discurso de Allende para las nuevas generaciones
    Covid cero: la grieta del descontento se agranda en China
    Cuáles son las opciones para una negociación entre Rusia y Ucrania
    Muere el escritor Dominique Lapierre, autor de los superventas ‘La ciudad de la alegría’, ‘¿Arde París?’ y ‘Oh, Jerusalén’
    Las mentiras que dinamitaron la carrera de The Doors
    Ideas de regalos para el jardinero
    Guía de regalos para el ‘foodie’
    “Jugamos al rugby para transformar vidas”: el deporte que desarticuló 11 bandas delictivas de Venezuela
    La supervivencia de la sabana brasileña se decide en los despachos de Bruselas
    El ‘palacio’ de la familia Orbán se erige como símbolo de la corrupción en Hungría
    Irán apunta a una abolición de la policía de la moral tras más de dos meses de protestas
    Los barrios de Bogotá que quieren robarle espacio a los carros 
    Marcela Ángel: “Tenemos que cerrar la brecha entre academia y territorio”
    El exitoso colegio chileno que forma “agentes frente al cambio climático”
    José Antonio Marina: “Que se haya puesto de moda la felicidad es catastrófico”
    El Padre, El Hijo y El Espíritu Santo de ella
    El trágico final de Gérard Philipe, el ‘príncipe de actores’ al que la Nouvelle Vague ninguneó
    Las vidas largas
    Historia de un robo: así se recuperó un manuscrito firmado por Hernán Cortés hace casi 500 años
    ¿Selfie sí o selfie no en Art Basel?
    De las galerías a las calles: así se hizo importante Miami para el arte del mundo
    Cómo el pacto de dos amigas logró que Fleetwood Mac sobreviviera al caos, el sexismo y la cocaína
    La vida bajo los focos de Sadie Sink: una infancia en Broadway y una adolescencia en ‘Stranger Things’
    Todos quieren a Dwayne Johnson
    Shakira niega una relación sentimental con su instructor de surf: “No tengo ninguna pareja”
    El ‘conseguidor’ español que sedujo a las constructoras en América
    Las islas del Caribe colombiano que desaparecen por el cambio climático
    La tragedia en la frontera de Melilla: el papel de Marruecos y España en las muertes del 24-J
    Un tatuaje y un bebé en el nombre de Mircea Cărtărescu
    Qatar 2022, el único Mundial donde es posible ver dos partidos en un mismo día
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Enredados en el Mundial | Los jugadores iraníes vuelven a cantar el himno y ha nacido una estrella en EE UU
    El negocio de la nostalgia del fútbol en Colombia
    ‘Tu opinión es una mierda’: la campaña que alerta sobre los peligros de la polarización
    Venezuela tiene escasez de sacerdotes
    Why Russia-Ukraine peace talks won’t be happening anytime soon  
    The toll of El Salvador’s gang crackdown: ‘Police and soldiers have absolute power’
    Following the FTX bankruptcy, an expert liquidator has been searching for all the missing money 
    How Nazi propaganda dehumanized Jews to facilitate the Holocaust
    Joseph Henrich, evolutionary anthropologist: ‘The best antidote to white supremacy is more science’   
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Toda la actualidad científica en el boletín de Materia
    Letras Americanas: la actualidad literaria de un continente vista por el escritor Emiliano Monge
    Ideas: reportajes y entrevistas para entender el mundo
    China relaja las medidas anticovid en Guangzhou para frenar nuevas protestas
    Hungría evita la confrontación con Bruselas y confía en desbloquear los fondos europeos en 2023 
    Muere el expresidente de China Jiang Zemin
    López Obrador da su aprobación para que ‘el rey del cobre’ Germán Larrea compre Banamex
    Los desafíos al proceso de transición ecológica
    Estos picos han enamorado al chef José Andrés y están hasta en las mesas de Corea del Sur
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Mirian Galán, una de las mejores profesoras del mundo: “El niño no falla. Si suspende, ha suspendido el docente” 
    ¿Adiós a los anuncios con coches para niños y cocinas para niñas? Los jugueteros pactan desterrar los estereotipos sexistas en la publicidad
    La respuesta a la guerra en Ucrania también es literaria
    Lo más escuchado en Spotify en 2022: solo Rosalía se coloca en España en una lista dominada por hombres latinos
    Muere Christine McVie, cantante y teclista de la legendaria banda Fleetwood Mac, a los 79 años
    Bill Hansson, experto en olfato: “No compres feromonas para intentar conseguir sexo, no funciona. Mejor trabaja en tu personalidad”
    Javier de Felipe, neurocientífico: “Me encantaría ser un perro durante un par de minutos” 
    Un proyecto enseña a los robots a crear nuevas herramientas, como los primeros humanos
    Gidey choca contra el muro del maratón en su debut en Valencia
    Sebastián Mora, el corredor que triunfa en el ciclismo del futuro y sufre las penurias del antiguo
    Haliburton alumbra Indiana
    Los dragones que viven entre los granos de arena
    El pueblo de Barcelona donde los vecinos ahorran 50 euros en la factura de la luz gracias a placas solares en edificios municipales
    El medio ambiente tensiona a los socios del Gobierno valenciano 
    Ciencia a toda velocidad: los años increíbles en los que hubo más coches eléctricos que de gasolina
    Oriol Vinyals: “Nuestra generación verá una inteligencia artificial que iguale o supere a la del ser humano”
    “Ser malos”, Sam Va Lentín y el hilo de Bartual: los tuits que merecen pasar a la historia de internet
    La historia de cómo terminó sin acusados el ‘caso Cursach’, la mayor causa judicial de Baleares 
    El equilibrio difícil de Grande- Marlaska: ni incomodar a Marruecos ni a la Guardia Civil 
    La Guardia Civil investiga un triple crimen en un pueblo de Granada
    ‘Fácil’: buscar la libertad sin tener independencia
    ‘Masterchef’ contra el teletrabajo’, por Sergio del Molino
    ‘MasterChef’ cocina con la polémica como ingrediente estrella
    Shakira y Piqué sellan su acuerdo de separación en Barcelona ante el juez
    Los actores de ‘Love Actually’ se reencuentran: ¿qué ha sido de ellos 19 años después?
    Acuerdo de divorcio entre Kim Kardashian y Kanye West: custodia compartida y 200.000 dólares de pensión
    Eviatar Matania: “Los gigantes tecnológicos se están convirtiendo en actores políticos y los veremos en la sala de mando”
    ‘Hombres de mi edad’, por Ignacio Peyró
    La polarización es como las drogas: engancha
    Descansar está mal visto: el arte perdido del reposo
    Madrid, la nueva Miami: así se han hecho con la capital los ricos latinoamericanos
    Si no tiene ahorros, esta es una de las pocas alternativas para comprar casa
    Roe Ethridge, el fructífero intercambio entre el arte y el comercio
    ‘La última vez’, de Guillermo Martínez: un laberinto con final milagrosamente imprevisible
     “En Somalia, cuando aún estamos tratando de reponernos de un golpe, enseguida nos viene el siguiente”
    Una agricultura climáticamente inteligente para resistir a las turbulencias económicas y sociales  
    Oyambre, Son Bou y otras nueve playas españolas para un baño de historia
    Cómo actuar ante el caos de los aeropuertos: qué hacer frente a retrasos y cancelaciones de un vuelo
    El lamentable caso de Anne Hathaway o por qué se odia a algunas famosas sin justificación ninguna
    Samantha Hudson: “Me va bien económicamante, pero no soy Paula Echevarría”
    “Tobogán de piojos”, “genocida de oxígeno”... Por qué cada Mundial recuerda el poderío del español como idioma para insultar
    Alejandro Jato, el actor que será Camilo Sesto: “Da pena la imagen que los jóvenes tienen de él, con lo grande que fue”
    Menú semanal de El Comidista (5 a 11 de diciembre)
    Té para todos: 13 tiendas especializadas donde comprarlo en España
    Inversión verde: pros y contras de una estrategia en revisión
    Iturralde González explica el segundo gol de Japón: “Las imágenes que salen son muy tramposas”
    Gómez de Celis frena hasta tres veces a Carlos Herrera tras hacer esta afirmación sobre el paro
    Cristiano pide a la Juve 20 millones de euros
    El SMS cumple 30 años. El medio era el mensaje
    Las mejores películas de la Historia del Cine según la mítica revista del BFI
    

Este proceso se repetirá en cada sección del periódico digital, creando un bucle.

Luego crearemos variables con las distintas url de cada sección del periódico 

Por ejemplo internacionales:


```python
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Radiografía del descontento chino
    La caravana de la muerte de Kurilivka: una superviviente relata la matanza de 26 civiles que huían de la guerra en Ucrania
    Los libaneses ‘roban’ su propio dinero en los bancos a punta de pistola y con bidones de gasolina
    ¿‘Nuestros’ principios o los de todos?
    China hierve contra la covid cero
    Una globalización centrada en los seres humanos
    Autocracia en crisis
    “¿De qué color es el hambre, mamá?”
    Lula da a su esposa Rosangela Silva protagonismo en la transición en Brasil
    El fiscal general de Irán apunta a la abolición de la policía de la moral tras más de dos meses de protestas 
    El ‘palacio’ de la familia Orbán se erige como símbolo de la corrupción en Hungría
    El régimen de excepción de Nayib Bukele asfixia a las pandillas: “Policías y soldados tienen poder absoluto” 
    Por qué la negociación para la paz en Ucrania queda lejos
    La UE acuerda imponer un tope de 60 dólares al petróleo ruso para golpear las finanzas del Kremlin
    Más de 400 rusos buscan protección en España: “No quiero formar parte de este crimen contra Ucrania”
    El tope al petróleo ruso: un golpe más para Moscú, pero lejos de ser letal
    Zelenski pide prohibir en Ucrania la Iglesia ortodoxa apadrinada por Rusia
    Rusia apunta en su primera lista negra a las organizaciones LGTBI e incluirá a los críticos con el alistamiento militar 
    El boyante negocio de vender equipación militar en Ucrania: “Lo que más compran es ropa térmica; ya hace frío”
    Nueva York, el gran supermercado legal de la marihuana
    Cuba, el precipicio y el cambio pendiente
    Lula negocia con el Congreso de Brasil cómo pagar su gran promesa electoral
    Reaparece el fantasma del control de precios en Venezuela con el repunte de la inflación
    El feminicidio de García Belsunce sigue impune: la justicia argentina absuelve al imputado
    

Para limpiar la pantalla usamos **os.system("clear")**


```python
os.system("clear")
```




    1



Con **print(colored)** añadimos el atributo de color

y con **attrs** se mostrará los títulos con el estilo deseado, en este caso **bold**

#### Color

A continuación se muestran los titulares de las páginas principales del diario El País, que contienen las siguientes palabras:
Feminismo


```python
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))
```

    A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:
    Feminismo
    

Se crea una variable llamada **str_match** y sé utilizando la función **for** para comprobar que tengan las palabras claves, este se repite una y otra vez 


```python
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
```

    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    


```python
print(colored("Igualdad", 'green', attrs=['bold']))

str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))

print(colored("Mujeres", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))

print(colored("Mujer", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))

print(colored("Brecha salarial", 'green', attrs=['bold']))

str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))

print(colored("Machismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))

print(colored("Violencia", 'green', attrs=['bold']))

str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))

print(colored("Maltrato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))

print(colored("Homicidio", 'green', attrs=['bold']))

str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))

print(colored("Género", 'green', attrs=['bold']))

str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))

print(colored("Asesinato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))

print(colored("Sexo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))
```

    Igualdad
    
    Mujeres
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Mujer
    Tuteladas, discriminadas: así vive la mujer de Qatar
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Brecha salarial
    
    Machismo
    
    Violencia
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Maltrato
    
    Homicidio
    
    Género
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Asesinato
    
    Sexo
    Bill Hansson, experto en olfato: “No compres feromonas para intentar conseguir sexo, no funciona. Mejor trabaja en tu personalidad”
    

## Actividad 4

Ya para la última actividad trabajamos con los datos de [la API de datos del COVID-19](https://covid19api.com/) con los cuales pudimos trabajar tablas y gráficos. 

Además, pudimos trabajar con los datos de **Colombia, España, Ecuador y República dominicana**. De los cuales creamos gráficos donde se podían visualizar **el crecimiento de los casos COVID para las fechas 2021-2022**.


Para ello primero importamos las librerías Pandas con la función `!pip install pandas`


```python
pip install pandas
```

    Requirement already satisfied: pandas in c:\users\gabri\anaconda3\lib\site-packages (1.4.4)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: pytz>=2020.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: six>=1.5 in c:\users\gabri\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Note: you may need to restart the kernel to use updated packages.
    

Luego configuramos las distintas variables como:

Configuración de **Pandas**
Para Importar utilizaremos `pd` de **pandas**


```python
import pandas as pd
```


```python
miurl = "https://api.covid19api.com/countries"
```

**Ejecutamos Panda**

Para ello generamos el **dataframe**
La abreviatura de dataframe es `df.` Con `función read_json()` que lee el formato json. Dentro del paréntesis ponemos lo que queremos leer. Ejemplo, un url.


```python
df = pd.read_json(miurl)
```

Para visualizar los datos llamamos el objeto y panda identifica una de las entradas del dataframe.Observamos una tabla de Panda que identifica las entradas del dataframe.


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>Slug</th>
      <th>ISO2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Ecuador</td>
      <td>ecuador</td>
      <td>EC</td>
    </tr>
    <tr>
      <th>1</th>
      <td>French Polynesia</td>
      <td>french-polynesia</td>
      <td>PF</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Greenland</td>
      <td>greenland</td>
      <td>GL</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Honduras</td>
      <td>honduras</td>
      <td>HN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Martinique</td>
      <td>martinique</td>
      <td>MQ</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>243</th>
      <td>Côte d'Ivoire</td>
      <td>cote-divoire</td>
      <td>CI</td>
    </tr>
    <tr>
      <th>244</th>
      <td>Eritrea</td>
      <td>eritrea</td>
      <td>ER</td>
    </tr>
    <tr>
      <th>245</th>
      <td>Faroe Islands</td>
      <td>faroe-islands</td>
      <td>FO</td>
    </tr>
    <tr>
      <th>246</th>
      <td>Niger</td>
      <td>niger</td>
      <td>NE</td>
    </tr>
    <tr>
      <th>247</th>
      <td>Singapore</td>
      <td>singapore</td>
      <td>SG</td>
    </tr>
  </tbody>
</table>
<p>248 rows × 3 columns</p>
</div>



**Exploración de la tabla**

Para ver las primeras entradas de la tabla utilizaremos la siguiente función:


```python
df.head(6)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>Slug</th>
      <th>ISO2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Jamaica</td>
      <td>jamaica</td>
      <td>JM</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Kyrgyzstan</td>
      <td>kyrgyzstan</td>
      <td>KG</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Macedonia, Republic of</td>
      <td>macedonia</td>
      <td>MK</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Marshall Islands</td>
      <td>marshall-islands</td>
      <td>MH</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Papua New Guinea</td>
      <td>papua-new-guinea</td>
      <td>PG</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Sweden</td>
      <td>sweden</td>
      <td>SE</td>
    </tr>
  </tbody>
</table>
</div>



Con **df.tail()** Vemos las últimas


```python
df.tail(6)
```

Para ver las informaciones sobre las variables que contiene el df usamos la siguiente función:


```python
df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 248 entries, 0 to 247
    Data columns (total 3 columns):
     #   Column   Non-Null Count  Dtype 
    ---  ------   --------------  ----- 
     0   Country  248 non-null    object
     1   Slug     248 non-null    object
     2   ISO2     248 non-null    object
    dtypes: object(3)
    memory usage: 5.9+ KB
    

Para visualizar una sola variable


```python
df['Country']
```




    0                        Jamaica
    1                     Kyrgyzstan
    2         Macedonia, Republic of
    3               Marshall Islands
    4               Papua New Guinea
                     ...            
    243    Saint Pierre and Miquelon
    244             Saint-Barthélemy
    245                     Viet Nam
    246                      Bahamas
    247                New Caledonia
    Name: Country, Length: 248, dtype: object



Para ver un valor concreto de una de las variables:


```python
df['Country'][66]
```




    'South Georgia and the South Sandwich Islands'




```python
df['ISO2'].head()
```




    0    JM
    1    KG
    2    MK
    3    MH
    4    PG
    Name: ISO2, dtype: object



## Conclusión

La materia de Periodismo de Datos II: herramientas Digitales para la Visualización y Presentación de Datos me ha abierto un mundo de conocimientos y una puerta de interés. 
Durante este corto plazo pude adquirir los conocimientos necesarios para organizar y generar visualizaciones de datos uniendo el Markdown y Python.
