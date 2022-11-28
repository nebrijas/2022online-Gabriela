# Ad3_Gabriela_Castro
## Ejercicio Python para lograr un sraping de una web

A Continuación trabajaremos en **la actividad 3**, en la cual elaboraremos un ejercicio *Scraping* Web a través del lenguaje de programación Python en una libreta de la plataforma Jupyter en formato [Archivo.ipynb](docs/Ad3.ipynb)


Para iniciar a trabajar debemos tener el código fuente



### Código fuente


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored

resultados = []

req = requests.get("https://resultados.elpais.com")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')

tags = soup.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')

tags = soup3.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')

tags = soup14.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req16 = requests.get("https://elpais.com/television/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup16 = BeautifulSoup(req16.text, 'html.parser')

tags = soup16.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)


os.system("clear")

print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))

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

    El Mundial, en vivo
    Universo Mundial
    El calendario a seguir desde América
    ¿Quién va a ganar? Simulador y pronóstico de cada selección 
    La ‘newsletter’
    Las protestas se extienden en China contra la política de covid cero
    La gestión del frío enfrenta a Zelenski y al alcalde de Kiev
    La vida bajo los bombardeos rusos
    Así se vive en un refugio invernal durante la guerra
    Pobreza en el Olimpo académico de EE UU: la huelga que cimbra a la Universidad de California 
    El caótico primer mes de Elon Musk en Twitter
    ‘Argentina, 1985’, un debate nacional entre la ficción y la memoria
    Alemania rescata un empate contra España sobre el final del partido
    Un empate socialdemócrata
    Datos y gráficos | Alemania explota un error de España para empatar un partido equilibrado
    Croacia da vuelta el partido y elimina a Canadá (4-1)
    Marruecos da un batacazo a Bélgica sobre el final (0-2)
    Costa Rica se redime ante un Japón sin puntería (0-1)
    Madrid, la nueva Miami: así se han hecho con la capital española los ricos latinoamericanos
    López Obrador saca músculo en las calles con una manifestación masiva en México
    El Bosque, el pueblo mexicano que se tragó el mar
    Argentina contra la impunidad de los feminicidios
    Neofascistas, nacionalpopulistas, tecnosoberanistas. ¿Cómo llamamos a las nuevas derechas radicales? 
    Las abuelas que han viralizado el arte de elaborar la pasta italiana
    Pepa Bueno: “Las páginas de EL PAÍS tienen que ser el lugar donde los diferentes se encuentren”
    Videoanálisis | La FIL mastodóntica y popular está de vuelta
    La FIL de Guadalajara pone una vela al libro y otra al balón
    Concepción Company: “De todos los mexicanismos me quedo con apapachar”
    El acoso invernal de Putin 
    Por el bien de todos
    Otra forma de violencia política
    Yo te vi, papá, emocionarte con Messi
    Ideas de regalos para el jardinero
    Guía de regalos para el ‘foodie’
    Bolsonaro reaparece en una ceremonia militar tras batallar su derrota desde la trastienda
    El sueño hecho realidad del refugiado sirio del selfi con Merkel
    Crónica del asesinato de una niña en la Francia rural
    La violencia verbal de Vox desborda el Congreso español
    
    El negocio de las chicas imagen en las discotecas: “La misión es sonreír y que los hombres beban más”
    Las guatemaltecas que estudian ingeniería para llevar luz a sus comunidades
    Impresiones 3D y Telegram: el premiado proyecto de estudiantes colombianos para potabilizar agua
    La ‘ciudad esponja’: diez soluciones para resolver el problema del agua en México
    Cómic y energía nuclear: el superventas francés que sacude el debate sobre el cambio climático
    En la biblioteca de Almudena Grandes
    Otras mujeres
    Adiós a Ellen Pompeo, la funcionaria de la tele
    ¿Selfie sí o selfie no en Art Basel?
    De las galerías a las calles: así se hizo importante Miami para el arte del mundo
    La bestial tensión sexual entre Bruce Willis y Cybill Shepherd en ‘Luz de luna’, la serie en la que la actriz tuvo mucho que decir
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    Alessandro Michele, crónica de una salida anunciada
    Leonor Lavado: “Somos como hablamos: la voz es nuestro ADN psicológico”
    De la carnicería de su padre en España a la estrella Michelin en Chicago
    Macondo Inundado: el pueblo donde nunca deja de llover 
    Dormir en una caja a 200 euros la noche para asistir al Mundial de Qatar
    Retrato de Pablo Milanés a través de sus 10 canciones más decisivas
    De Honduras a Ucrania: cuando un niño crece bajo las bombas
    Qatar 2022, el único mundial donde es posible ver dos partidos en un mismo día
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Enredados en el Mundial | Los jugadores iraníes vuelven a cantar el himno y ha nacido una estrella en EE UU
    Al menos 500 alpacas mueren por una ola de frío en Perú
    Los partidarios de Bolsonaro utilizan sus móviles para pedir un golpe “extraterrestre” 
    Cuatro carceleros dan un brutal paliza a un hombre negro en Georgia
    Protests spread across China as anger builds over Xi Jinping’s zero-Covid policy 
    War in Ukraine: The battle to survive sub-zero temperatures 
    The story of a crypto scammer that ended in suicide
    To boost oil supplies, US looks to lift sanctions on Venezuela
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Toda la actualidad científica en el boletín de Materia
    Letras Americanas: la actualidad literaria de un continente vista por el escritor Emiliano Monge
    Ideas: reportajes y entrevistas para entender el mundo
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    El primer ministro de Rumania: “Necesitamos un esfuerzo común en la OTAN para defender cada centímetro de territorio frente a Rusia”  
    La justicia investiga si el Gobierno de Macron favoreció a consultoras privadas en las dos últimas campañas presidenciales en Francia
    Aquí puede buscar si ha sido engañado por la estafa internacional de las criptomonedas
    El secreto de la pirámide
    El futuro de las compras: más redes sociales, pago a plazos y vuelta de la tienda física
     El Papa detecta fallos en Caritas Internationalis y cesa a sus responsables 
    La Iglesia italiana da por primera vez cifras de los abusos cometidos por el clero
    El Senado de EE UU da un paso clave para blindar el matrimonio homosexual frente al Supremo
    Muere Hans Magnus Enzensberger, gran intelectual alemán del siglo XX
    ‘Close’, una mirada conmovedora a la fragilidad de la preadolescencia
    La gran retrospectiva de Vermeer en Ámsterdam aviva la polémica sobre la autoría de ‘Muchacha con flauta’
    Vivir con un trastorno alimentario: “Me di cuenta cuando me miré al espejo y vi la muerte”
    Josefa Ros Velasco, filósofa: “Si alguien se aburre suele darse a la botella, cuando le pasa a un país suele darse una revuelta”
    La insólita historia de la mujer que descubrió el primer antibiótico español
    Canadá conquista su primera Davis a lomos de Aliassime
    La selección femenina de baloncesto se clasifica para el próximo Eurobasket
    La trituradora del Barcelona no tiene piedad con el Atlético (1-6)
    Operación ‘OS35’: cómo rescatar un gigante de 40.288 toneladas varado a la sombra de Gibraltar
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    La izquierda retira por sorpresa y a última hora la propuesta para abolir los toros en Francia 
    Mastodon: qué es y cómo funciona la red social en la que los usuarios deciden qué está permitido
    Así serán las nuevas marcas de verificación en Twitter: azul, oro y gris
    Gafas con funciones de un móvil, ‘Photoshop’ instantáneo y otros inminentes avances gracias a los nuevos chips
    Sánchez pide a la patronal que negocie con los sindicatos un acuerdo salarial
    El pasado franquista pervive en Santa Cruz de Tenerife
    La federación de la España Vaciada busca implantarse en todo el país 
    El ‘bon vivant’ acorralado de la FIFA que grabó a sus amigos
    ¿Qué ocurre tras la edad de oro de la televisión? El mismo oro, aunque enterrado bajo una oferta masiva
    ‘This England’, por Carlos Boyero
    Windsor desvela su decoración navideña en las primeras festividades sin Isabel II y con Carlos III como rey
    Camila y los 1.000 osos Paddington: la reina entrega a una ONG infantil los peluches en homenaje a Isabel II
    Stallone vs. Schwarzenegger, la “competición” eterna: “Éramos antagonistas. Soñaba con pegarle y él con pegarme a mí”
    El misterio de Manuel Carrasco: cómo salir de una barriada de pescadores y acabar siendo un cantante que llena estadios
    Los guardianes de la ensaladilla rusa, la tapa popular que subió a los altares ‘gourmet’ 
    Erri De Luca, escritor: “Construir una vida es más difícil que contarla”
    Descansar está mal visto: el arte perdido del reposo
    Perdidos en el laberinto del paro
    Su vecino lo timaba con la calefacción central
    En la cuneta del sueño americano
    Descuidos de seleccionador: los lectores agregan libros de fútbol que no entraron en la lista
    Mi combate contra la ablación y el VIH en Senegal
    Masacre en Melilla: la peligrosa decisión de socialistas y populares
    Oyambre, Son Bou y otras nueve playas españolas para un baño de historia
    Cómo actuar ante el caos de los aeropuertos: qué hacer frente a retrasos y cancelaciones de un vuelo
    Samantha Hudson: “Me va bien económicamante, pero no soy Paula Echevarría. Nunca seré normativa”
    Alaska: “No entiendo la cultura de la cancelación”
    ¿Es buena idea masturbarse antes de salir? Las verdades y mentiras de la relajación posorgasmo
    El dilema Kit Connor: ¿debe conocerse la sexualidad de un actor para interpretar un papel gay?
    Vender carne... y un estilo de vida: así son las nuevas hamburgueserías
    ¿Cuál es la mejor receta de puré de patatas?
    Las nuevas jubilaciones: más retiros parciales, casi a los 65 años y cobrando 1.258 euros
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Macarena Olona sorprende a todos al publicar este mensaje sobre Begoña Gómez
    Le van a llover los palos: la cantada de Courtois que mete en un lío gordo a Bélgica
    Ocho mil millones de cursis
    Las 10 mejores películas y sagas posapocalípticas
    Las protestas se extienden en China contra la política de covid cero
    La gestión del frío enfrenta a Zelenski y al alcalde de Kiev
    El sueño hecho realidad del refugiado sirio del selfi con Merkel
    La vida bajo los bombardeos rusos
    Democracias a la defensiva
    La UE vista desde el G-20 de Bali 
    El arte ruso de la provocación
    Los moderados han ganado las elecciones de medio mandato en Estados Unidos
    Los trabajadores migrantes de provincias en China estallan contra los confinamientos por covid
    Sobrevivir bajo cero en Ucrania
    La UE teme que los ataques rusos contra la red eléctrica de Ucrania fuercen otra oleada de refugiados
    Encuentran el cadáver de una niña desaparecida en el corrimiento de tierra en la isla italiana de Ischia
    La vida bajo los bombardeos rusos
    Crónica del asesinato de una niña española en la Francia rural
    Bolsonaro reaparece en una ceremonia militar tras batallar su derrota desde la trastienda
    La muerte de 10 personas en un incendio en Xinjiang extiende las protestas contra la política de covid cero en China 
    Estados Unidos autoriza a Chevron a operar en Venezuela ante el diálogo de Maduro con la oposición
    El Gobierno venezolano y la oposición acuerdan descongelar entre 3.000 y 5.000 millones de fondos estatales en el extranjero
    Alemania da un golpe de timón a sus políticas sociales con la ambiciosa reforma de Scholz
    La nota del autor de la matanza del Walmart de Virginia: “Se reían de mí y decían que era un asesino en serie”
    La pobreza se ceba con los menores de 18 años en América Latina
    Tres horas libres en el trabajo para ver el partido… ¡Bienvenidos a Brasil!
    Petro y López Obrador estrenan un eje latinoamericano con el éxito de la negociación de Venezuela como trasfondo
    Nayib Bukele desplegará policías y militares para cercar las ciudades de El Salvador contra los pandilleros
    Violencia sexual 
    El acoso invernal de Putin 
    Mari Carmen vuela en globo 
    Los desposeídos
    ‘Arraigo’
    Aunque nos tiemble la barbilla
    Otra forma de violencia política
    El espejo escocés todavía sirve 
    Orfandad representativa
    Las cámaras
    Venezuela negocia 
    Más cerca de la Luna 
    Arte del pasado
    Iglesias y lo impermeable
    El carnaval de Infantino
    El Roto
    Flavita Banana
    Riki Blanco
    Peridis
    Sciammarella
    Envía tu carta
    Lucha feminista no solo en días mundiales
    Gamberros ilustrados
    Contra la violencia machista 
    Noticias positivas en tiempos caóticos
    Bomba nuclear en Barcelona
    Una maldita lista en tiempos airados
    El defensor del lector contesta
    Las provocaciones de los ultras desbordan el vaso en el Congreso
    Tres años de exabruptos de Vox en el Congreso de los Diputados
    Memoria pétrea del franquismo 
    Aunque nos tiemble la barbilla
    Orfandad representativa
    Otra forma de violencia política
    Mudar de piel
    El nuevo retroorden de Vox
    Sánchez pide a la patronal que negocie con los sindicatos un acuerdo salarial
    Abascal defiende la violencia verbal de Vox y llama “enloquecida” a la ministra Irene Montero 
    Los sindicatos y los agentes sociales de Castilla y León se alzan contra Vox
    La federación de la España Vaciada busca implantarse en todo el país 
    El ‘clan de Santiago’ se topa con los ‘halcones’ del PP
    Bendodo, el nuevo ‘poli malo’ de Feijóo
    El pasado franquista pervive en Santa Cruz de Tenerife
    El abogado de la mayor estafa inmobiliaria de España que pasó a vender la cocaína robada al Tío José
    La Guardia Civil asegura que tardó cuatro horas en saber que hubo muertos en la tragedia de Melilla
    Albares: “España no quiere verse sin embajador en Venezuela. La decisión de retirarlo es reversible”
    Feijóo reclama unir en el PP el voto de castigo a Sánchez en las urnas y rechaza agitar las calles como Vox
    Hay casi 4.000 cervezas artesanas españolas. ¿Cómo probarlas todas?
    El cambio hacia un consumo sostenible empieza por los pies
    Los tentáculos mundiales de la estafa en ‘criptos’: ‘call centers’ por Europa, falsos ‘brokers’ y miles de víctimas 
    Las asociaciones de consumidores enfrían el alcance de las ayudas a hipotecados vulnerables
    Borja Prado enseña el colmillo en Mediaset
    Simulador de hipoteca: calcule la cuota de su préstamo
    El coste de la vida
    La intermediación del ahorro y su evolución
    Ecos de una goleada histórica (en la patronal)
    La Europa ganadora que necesitamos
    Una recesión largamente anunciada
    Ferrovial inaugura la ampliación de la autopista I-66  en Virginia, con una inversión de 3.550 millones de euros
    Tu programa me suena: cómo protegerse ante el plagio en televisión
    Javier Biosca, la historia del mayor estafador de España en criptomonedas que acabó en suicidio
    Madrid, la nueva Miami: así se han hecho con la capital los ricos latinoamericanos
    La gran paradoja de los españoles ante la economía: pesimistas en lo colectivo, optimistas en lo individual
    Mejora la fiscalidad para el cine y las series: podrán deducirse hasta 10 millones por capítulo
    Caballos al galope: un negocio con un impacto económico de 7.400 millones de euros
    Si no tiene ahorros, esta es una de las pocas alternativas para comprar casa
    Rotundas sorpresas presupuestarias
    Una sentencia de la Audiencia de Madrid aboca al sobreseimiento del ‘caso Plus Ultra’
    Bruselas cree que el empleo aguantará mejor en esta crisis ante el alto número de puestos de trabajo sin cubrir
    Madrid, la nueva Miami: así se han hecho con la capital los ricos latinoamericanos
    Si no tiene ahorros, esta es una de las pocas alternativas para comprar casa
    Los efectos de una economía de andar por casa
    Caballos al galope: un negocio con un impacto económico de 7.400 millones de euros
    Los impuestos que se necesitan para construir la sociedad del futuro
    De 800 millones para Repsol a 500 para Iberdrola: así es la factura del impuesto energético a las empresas
    Sareb recibe una oleada de demandas de sus directivos por la rebaja salarial
    Telepizza lanza un SOS a sus bonistas y encarga a Houlihan Lokey reestructurar su deuda
    Guerra abierta entre cuerpos de funcionarios por el nuevo proceso de promoción interna
    Por primera vez un juez declara nulo un contrato de alquiler por aplicación de la perspectiva de género
    Visitas a centros de acogida y muchas horas de estudio: así se forman los jueces en materia de género
    La justicia obliga a Iberia a controlar el peso de las maletas para que los azafatos no se lesionen
    La difícil tarea de recuperar el talento investigador que un día hizo las maletas
    Descubre las formaciones de marketing ‘online’ más buscadas (y económicas) de 2023
    La quinta edición de EnlightED aborda los retos del aprendizaje y la educación en la era digital  
    Logística de ida y vuelta, cuando la solución está en reciclar menos y reutilizar más
    Logística y digitalización, el manual de supervivencia para pymes
    Empleados satisfechos, empresas de éxito
    Diez claves del bienestar corporativo para empresas de éxito
    Las aventuras de un par de calcetines que dan empleo a todo un pueblo
    Cultura financiera como punto de partida para volver a empezar
    Las soluciones digitales que necesita mi negocio 
    Las fórmulas de financiación más adecuadas para mi negocio
    Alexia Putellas, un Balón de Oro a base de “esfuerzo, constancia, disciplina y saber reinventarse”
    El método Muñoz para triunfar en cada reto que se propone
    ¿Por qué se está enfriando la economía china?
    ¿Cómo Estados Unidos espera ganar la guerra de los chips?
    Si tú lo imaginas, yo te lo imprimo
    Por qué tu casa puede ser tu radiografía además de tu biografía
    Cómo garantizar la seguridad en un mundo de amenazas híbridas
    ¿Cuáles son los dilemas éticos del uso de la inteligencia artificial?
    Cómo conseguir ayudas a la digitalización para autónomos y pymes con Kit Digital
    Un brindis con vino español por la sostenibilidad, la economía y el empleo
    La ley de familias da a los trabajadores hasta nueve días remunerados al año para atender urgencias y cuidados de familiares enfermos
    ¿Protege más a las mujeres elevar las penas?
    El Vaticano lamenta “con sorpresa y pesar” que China nombre a un obispo 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Los secretos atronadores del secretario general
    Balance de la COP27: un fondo para los más vulnerables mientras la meta de los 1,5 grados se aleja
    El silencio del cardenal Omella
    La cuarta dosis de la vacuna contra la covid se estanca: menos de la mitad de los mayores de 60 la ha recibido
    Gobierno y Junta chocan por Doñana mientras se agrava el deterioro ecológico 
    El feminismo se fractura en Madrid en las protestas contra la violencia machista que recorren España
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Listas de espera: más personas que nunca aguardan operación, pero bajan los días de demora
    Operación ‘OS35’: cómo rescatar un gigante de 40.288 toneladas varado a la sombra de Gibraltar
    328 mensajes de tu ex o cómo la violencia machista entra por el móvil
    Las manifestaciones del 25-N regresan bajo lemas que condensan los debates del movimiento feminista
    Los secretos atronadores del secretario general
    El primer Mundial en horario lectivo y con ‘smartphones’ se juega también en los institutos
    Linces y águilas imperiales se refugian en fincas privadas que se alían con conservacionistas  
    Unas gafas que cambian la forma de ver el mundo
    Cambia tu relación con los papeles de la cocina
    Enfermería, los profesionales de las ‘curas invisibles’ en las personas con VIH
    Las ciudades marcan el objetivo: acabar con el VIH en 2030
    La huella de carbono, el rastro que marca el futuro del planeta
    El club de la eficiencia energética 
    Psoriasis, en las profundidades de la piel
    Contar para sanar
    La nueva revolución agrícola 
    Nuevos talentos de la economía circular
    Lo lejos que se puede llegar con otra metodología educativa 
    Cuando el empleo se convierte en la mejor terapia 
    A solas con la obesidad
    Freno y marcha atrás en la obesidad infantil
    ¿Hasta dónde puede llegar el ser humano? El viaje a la oscuridad más absoluta
    El viaje a uno de los paraísos más bellos de España. Por qué este paisaje cuelga de las paredes de medio mundo
    Acuicultura: la importancia de comer ‘azul’ para vivir en verde
    El cultivo de pescado español, a la vanguardia del planeta
    El futuro de la aviación verde
    En busca de la eficiencia energética en los aeropuertos
    Un día en el servicio de ayuda a domicilio
    Trabajadores esenciales. Los que nunca paran
    Consejos para alimentar correctamente a los animales de compañía
    Cuidados y necesidades de perros y gatos en su etapa sénior
    Combatir el desperdicio alimentario desde la cesta de la compra
    Kilómetro cero para llenar la despensa
    Acompañamiento, el modelo alternativo de acogida de refugiados
    El metro como refugio. De los andenes de Madrid en 1936 a los de Kiev en 2022
    Yogures con menos azúcar, paso firme hacia la alimentación infantil del futuro
    Invisible, pero vital: el ciclo de las aguas subterráneas
    La bomba de calor, el sistema de climatización más sostenible y eficiente
    El primer Mundial en horario lectivo y con ‘smartphones’ se juega también en los institutos
    El cabecilla de los cánticos machistas del Elías Ahuja vuelve al colegio mayor pese a anunciarse su expulsión definitiva
    La nueva ley de enseñanzas artísticas endurecerá los requisitos para ser profesor y hará más homogéneas las pruebas de acceso del alumnado
    Una madre denuncia insultos homófobos a su hija en un colegio de Madrid: “Su tutor nos dijo que tenemos que respetar la opinión de los demás”
    Cataluña aprueba un complemento para ampliar la jornada a los profesores de informática de FP
    Más de 6.000 estudiantes de FP empezaron tarde el curso por el largo proceso de inscripción en Cataluña
    Cuando la escuela se convierte en un gueto: América Latina tiene las primarias más segregadas del mundo
    Ay, Lomloe
    Guarderías rurales contra la despoblación: “Si la escuela cierra, el pueblo muere”
    Aprendizaje, identidad comunitaria y desarrollo sostenible
    El Tribunal Superior de Navarra cuestiona que los colegios que segregan a niños y niñas sean excluidos de los conciertos educativos
    Evaluar competencias
    La Selectividad a los 50: ¿cirugía mayor o estiramiento facial?
    La libertad de elección de centro educativo y los cheques escolares en Madrid
    Selectividad: Desatar el nudo gordiano
    El nuevo sistema para evaluar los conocimientos digitales de los profesores valdrá en toda España
    Ofrecer comedor gratis en todos los colegios públicos es “alcanzable y urgente”: costaría 1.664 millones al año, según la ONG Educo  
    Una fórmula para que la escuela pública compita mejor con la concertada
    La pérdida de alumnos por el descenso de la natalidad está afectando con más fuerza a la escuela pública que a la concertada
    La disparidad de resultados entre autonomías en la EVAU se origina en la escuela, no en el examen 
    Las autonomías del PP critican la nueva Selectividad porque no prevé un examen único para todo el Estado
    La escalada vertiginosa de notas en Bachillerato: los sobresalientes de los que llegan a Selectividad se doblan en seis años
    El caso de Georgia, en EE UU: becar sin importar la renta agranda la desigualdad
    El techo de cristal del grado medio de FP: candidatos demasiado preparados se quedan con los puestos
    César Rendueles: “Hay universidades privadas que son como academias de conducir con pretensiones”
    La fuga de miles de médicos agrava el déficit de especialistas en España
    Jóvenes tutelados en la Universidad: “Tu pasado no tiene por qué condicionar tu futuro”
    Si tu familia está desahogada estudiarás Medicina y dobles grados, si no, Óptica o Educación 
    Volver a empezar
    Borges, 'Funes el memorioso' y la neurona Jennifer Aniston
    ¿Contra qué se rebela la lectura?
    Gobierno y Junta chocan por Doñana mientras se agrava el deterioro ecológico 
    Linces y águilas imperiales se refugian en fincas privadas que se alían con conservacionistas  
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    El precio del Ave Madrid-Barcelona cae un 43% pero sube un 14% en las líneas sin competencia 
    El plan del Gobierno para las reservas de agua mantiene intacta la alta presión del regadío
    Operación ‘OS35’: cómo rescatar un gigante de 40.288 toneladas varado a la sombra de Gibraltar
    Balance de la COP27: un fondo para los más vulnerables mientras la meta de los 1,5 grados se aleja
    Clemente Álvarez, premio a la conservación de la biodiversidad de la Fundación BBVA: “Debemos difundir la voz de alarma de los científicos”
    Investigan la brutalidad en una montería en la Sierra de Segura de Jaén 
    La pandemia y los carriles bici impulsan que cada vez más españoles pedaleen por las ciudades 
    España sigue anclada en la sequía a pesar de las lluvias: así es el mapa desigual del agua y las restricciones
    El cambio climático perjudica su salud
    Por qué comer animales puede ayudar a luchar contra el cambio climático
    Por qué hay que dejar de comer animales para luchar contra el cambio climático
    Bombas de carbono 
    Crisis de los insectos: esto no es un armagedón sino una debacle provocada por los humanos
    El quebrantahuesos reconquista los cielos 
    Un año de crisis climática sin fin
    Ríos imposibles: las 171.000 barreras que rompen el curso de agua en España
    Volver a empezar
    Borges, 'Funes el memorioso' y la neurona Jennifer Aniston
    ¿Contra qué se rebela la lectura?
    Josefa Ros Velasco, filósofa: “Si alguien se aburre suele darse a la botella, cuando le pasa a un país suele darse una revuelta”
    La insólita historia de la mujer que descubrió el primer antibiótico español
    Hilda Hudson, la primera conferenciante en el gran congreso internacional de matemáticas
    De León al espacio, pasando por una pequeña universidad pública: “Invirtiendo en ciencia se puede llegar a lo más alto”
    “Soñamos con ir a la Luna, pero no llegaremos a Marte” 
    Pablo Álvarez y Sara García, primeros astronautas españoles de la ESA en 30 años
    Una vacuna universal contra la gripe que usa la tecnología de ARN, probada con éxito en ratones
    Palabras y árboles
    Europa resucita su misión para taladrar Marte en busca de vida en 2028  
    El aroma de la inspiración y la piedra de la locura
    ¿Por qué son rocosos los satélites de los planetas gaseosos?
    ¿Cómo nos afecta en la Tierra la formación de un agujero negro?: tres grandes físicos lo desvelan
    Los límites de la terapia hormonal de la menopausia: no se recomienda para prevenir enfermedades, pero sí para tratar sofocos severos
    Sarro en dientes de miles de años muestra que los humanos del Paleolítico tenían mejor salud bucal
    El embarazo transforma el cerebro de las mujeres para favorecer el vínculo con sus hijos
    Rosa Ballester, catedrática de historia de la ciencia: “Sabemos que para mejorar la salud también importa la vivienda digna o la alimentación” 
    ¿Cómo nos afecta en la Tierra la formación de un agujero negro?: tres grandes físicos lo desvelan
    Hilda Hudson, la primera conferenciante en el gran congreso internacional de matemáticas
    Por qué el entrelazamiento cuántico revoluciona nuestro entendimiento de la naturaleza
    La órbita del telescopio ‘James Webb’ y el problema de los tres cuerpos
    Cien años de las ecuaciones que expandieron el universo
    Sangaku
    El tamiz de Apolonio
    La respuesta a la gran pregunta
    El aroma de la inspiración y la piedra de la locura
    ‘Los hijos de Hansen’ y la marginación social provocada por la lepra
    Los fractales y su estructura narrativa como parte del relato
    El amanecer de todo y el dinosaurio como animal modernista
    Los universos paralelos de un visionario científico llamado Philip K. Dick
    ¿Por qué son rocosos los satélites de los planetas gaseosos?
    ¿Es nueva la producción de alimentos en macrogranjas? 
    ¿Cómo se ve el cielo nocturno desde el ecuador?
    ¿Por qué las olas van siempre hacia la playa?
    Ciencia para derrumbar el mito de que la soja es mala para prevenir el cáncer de mama
    Cuidado con las conservas caseras: es importante hacerlas bien
    Una propuesta alternativa, barata y saludable a la nueva cesta de la compra
    Aditivos, propiedades saludables y fechas de caducidad: guía para entender las etiquetas alimentarias
    Desiertos de comida, o cuando comprar productos frescos es una odisea
    Carmen Machi: “Que te metieran mano en el metro nos parecía normal”
    Cómic y energía nuclear: el superventas francés que sacude el debate sobre el cambio climático
    ‘Argentina, 1985’, un debate nacional entre la ficción y la memoria
    Meter la mano en la vaca 
    El hombre alegría
    Una novia compartida con Arturo Pérez-Reverte y El Hombre Enmascarado
    Hans Magnus Enzensberger, un escéptico de la originalidad
    Videoanálisis | La FIL mastodóntica y popular está de vuelta
    Pepa Bueno: “Las páginas de EL PAÍS tienen que ser el lugar donde los diferentes se encuentren”
    Muere Irene Cara, actriz y cantante de ‘Fama’ y ‘Flashdance’, a los 63 años
    La Mano de Irulegi, más incógnitas que respuestas sobre el origen del euskera
    El periplo bajo las bombas de medio centenar de cuadros de artistas ucranios hasta llegar al Museo Thyssen de Madrid
    Otras mujeres
    Hermosa Márcia: el valor inquebrantable de una madre brasileña
    Muere Hans Magnus Enzensberger, gran intelectual alemán del siglo XX
    Bono, cantante de U2: “La filantropía nunca lo va a cambiar todo en el mundo”
    El Gran Hermano de George Orwell nació en la Guerra Civil 
    El fenómeno Colleen Hoover: cómo vender 20 millones de libros sin moverte de tu pueblo
    El bisnieto del apache Gerónimo hace memoria: “Murió sin dignidad, exhibido en ferias y desfiles” 
    El primer protagonista homosexual de Disney y un ejército de mujeres capitaneada por Viola Davis, entre los estrenos de la semana
    Santo Estevo, el monasterio al que todos le tienen fe
    La Calahorra de siempre, más viva que nunca
    La novela negra del siglo XXI no existe (sin Michael Connelly)
    Celebra el Black Friday con los mejores descuentos en ocio
    Disfruta de '¡Ay, Carmela!' en el Teatro Pavón
    Francesc Tosquelles en el Museo Reina Sofía
    Asiste en familia al preestreno de 'Rabbit Academy'
    La temida voltereta de la abolición de los toros en el sur de Francia quedó en un susto
    Las obras de mejora de la plaza de toros de Las Ventas comienzan en diciembre
    Actos a favor y en contra de los toros en Francia antes de que se debata su prohibición
    Luis Miguel Leiro, picador premiado y desencantado: “Amo y respeto a los animales, pero el toro ha nacido para la lidia”
    Las nuevas coordenadas culturales de Latinoamérica
    Las más bellas cartas de amor en castellano, las memorias de Marguerite Duras y otros libros de la semana
    Amor mío queridísimo: la delicadeza sentimental de Felisberto Hernández
    Ellas fueron modernas: cuatro artistas alemanas en la vorágine del cambio de siglo
    Anacrónicas y audaces: las cantautoras latinas que renuevan la música de raíz
    Los mejores libros infantiles y juveniles de noviembre
    Palabra de Kafka
    Una ‘Yerma’ con poco nervio y zozobra
    Lo nuevo de Pablo Remón es una virguería teatral y la actriz Fernanda Orazi es un fenómeno
    ‘Los chicos del coro’, una versión escénica sugestiva y con pinceladas feministas
    Trampantojo: HCQ
    Lo que jode es la respuesta: la diferencia entre crítica, cancelación y censura
    Edmonia, Frida y Amrita: tres mestizas
    La basura se lee con anteojos
    Mi otoño alemán
    ‘Percusión’: una novela del pasado para recordar el futuro
    Pere Gimferrer dentro del laberinto
    ‘La brecha’: cómo cambiar un mundo mal hecho
    ‘Tu sueño imperios han sido’: la historia boca arriba
    Nona Fernández: “En Chile intentan que conciliemos el sueño otra vez”
    Cristina Lucas: “Todo lo que se publicita está sobrevalorado”
    Enrique Gracián: “Hay infinitos más grandes que otros”
    Àlex Brendemühl: “La serie sobre el rey emérito no te deja indiferente”
    Marta Etura: “De no ser actriz, habría sido matrona”
    El calendario
    Universo Mundial
    La galería del día
    Las predicciones
    La ‘newsletter’
    España sabe competir
    Dani Olmo: “Nos faltó más control”
    Los 15 jugadores de España que han sellado el empate ante Alemania, uno por uno 
    España gana 1-1
    El Mundial de los valientes
    Algunos apuntes del arbitraje
    Yo te vi, papá, emocionarte con Messi
    Busquets descubre las carencias de Alemania
    Datos y gráficos | Alemania explota un error de España para empatar un partido equilibrado
    Un empate socialdemócrata
    Japón gripa, Costa Rica se redime
    Marruecos descose a Bélgica
    La victoria de Marruecos en Qatar acaba con disturbios en varias ciudades de Bélgica y Países Bajos
    El ocaso no alcanza a Croacia
    Mundial de Qatar 2022: últimas noticias en directo | Tite: “Creo que Neymar volverá a jugar en el Mundial”
    Canadá conquista su primera Davis a lomos de Aliassime
    La trituradora del Barcelona no tiene piedad con el Atlético (1-6)
    La selección femenina de baloncesto se clasifica para el próximo Eurobasket
    Txelu Fernández, plata terapéutica
    Messi libera a Argentina
    El homenaje de Luis Enrique a su hija Xana el día que cumpliría 13 años | Universo Mundial
    Última hora del Mundial de Qatar: vídeo en directo
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Es nieta de un mito del Barça y arrasa en TikTok. El secreto de esta artista de 20 años que quiere emular a Rosalía
    Cómo no perderte ni un solo minuto del Mundial
    Las promesas del baloncesto español piden consejo a Sergio Scariolo
    A toda mecha hacia el mundial de la consagración
    Cómo disfrutar de la montaña con todas las garantías
    Así hemos contado el Bélgica - Marruecos del Mundial de Qatar 2022
    Marruecos descose a Bélgica
    Última hora del Mundial de Qatar: vídeo en directo
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Japón gripa, Costa Rica se redime
    Así hemos contado el Japón - Costa Rica del Mundial de Qatar 2022
    Resumen de la jornada 7 del Mundial de Qatar 2022
    El Mundial de los valientes
    Mastodon: qué es y cómo funciona la red social en la que los usuarios deciden qué está permitido
    Así serán las nuevas marcas de verificación en Twitter: azul, oro y gris
    Gafas con funciones de un móvil, ‘Photoshop’ instantáneo y otros inminentes avances gracias a los nuevos chips
    Elon Musk ya edita tuits y Twitter no se ha hundido aún, ¿qué hará en el futuro?
    Elon Musk declara una “amnistía general” en Twitter para las cuentas suspendidas
    Así está fallando Twitter: racismo, derechos de autor y desprotección en dictaduras
    Quo Vadis, Elon Musk: por qué el colapso de Twitter no es un divertimento
    Candid Wüest: “Si alguien ‘apaga’ Ucrania, probablemente haya una respuesta y eso no interesa porque todos los países son vulnerables”
    El reclutamiento de personal se reinventa en las redes: “Se crea una relación de confianza entre los candidatos y las empresas mucho antes de haber contacto directo”
    El biógrafo de Elon Musk: “Para él, el caos es el procedimiento operativo estándar”
    Aplicaciones, relojes y etiquetas QR ayudan a evitar la desaparición de personas con demencia
    Cómo acorazar el ‘router’ ante un ciberataque con estos sencillos pasos
    La confusa nueva política de Elon Musk en Twitter: permitir mensajes de odio, pero que se vean menos
    ¿Y si cierra Twitter? Cómo descargar el historial y borrar los mensajes directos
    “Nos vemos en Mastodon, Space Karen”: los usuarios bromean sobre el fin de Twitter
    Centros de datos para acelerar la digitalización en España
    Los cuatro coches que llegaron a España en el año de los Juegos y la Expo
    Ocho mil millones de cursis
    Guía de viaje a la nube: una aventura con escalas
    Árboles tuiteros contra la ceguera botánica
    De Baudelaire a Midjourney: los nuevos “enemigos mortales del arte”
    Mastodon: qué es y cómo funciona la red social en la que los usuarios deciden qué está permitido
    Así serán las nuevas marcas de verificación en Twitter: azul, oro y gris
    Gafas con funciones de un móvil, ‘Photoshop’ instantáneo y otros inminentes avances gracias a los nuevos chips
    Elon Musk ya edita tuits y Twitter no se ha hundido aún, ¿qué hará en el futuro?
    Elon Musk declara una “amnistía general” en Twitter para las cuentas suspendidas
    Así está fallando Twitter: racismo, derechos de autor y desprotección en dictaduras
    Quo Vadis, Elon Musk: por qué el colapso de Twitter no es un divertimento
    Candid Wüest: “Si alguien ‘apaga’ Ucrania, probablemente haya una respuesta y eso no interesa porque todos los países son vulnerables”
    El reclutamiento de personal se reinventa en las redes: “Se crea una relación de confianza entre los candidatos y las empresas mucho antes de haber contacto directo”
    El biógrafo de Elon Musk: “Para él, el caos es el procedimiento operativo estándar”
    Aplicaciones, relojes y etiquetas QR ayudan a evitar la desaparición de personas con demencia
    Cómo acorazar el ‘router’ ante un ciberataque con estos sencillos pasos
    La confusa nueva política de Elon Musk en Twitter: permitir mensajes de odio, pero que se vean menos
    ¿Y si cierra Twitter? Cómo descargar el historial y borrar los mensajes directos
    “Nos vemos en Mastodon, Space Karen”: los usuarios bromean sobre el fin de Twitter
    Centros de datos para acelerar la digitalización en España
    Los cuatro coches que llegaron a España en el año de los Juegos y la Expo
    Ocho mil millones de cursis
    Guía de viaje a la nube: una aventura con escalas
    Árboles tuiteros contra la ceguera botánica
    De Baudelaire a Midjourney: los nuevos “enemigos mortales del arte”
    Confesiones de la mujer que lleva 40 años decidiendo quién será James Bond
    Atún rojo: el inesperado nexo cultural que une a Japón con el Mediterráneo
    Las excentricidades imposibles de las Kardashian: de escáneres cerebrales a 700 dólares en gominolas de cannabis
    Mis séptimos Premios Icon
    Los 12 patios del palacio de Viana en Córdoba: una muñeca rusa llena de plantas
    Arnau Griso, el adiós de un grupo que empezó como una broma y acabó creando el pop ‘buenrollero’: “Tenemos la necesidad de matar al padre”
    De Kim Kardashian en la cárcel a Selena Gómez con los Beckham: así celebran Acción de Gracias de los famosos
    Windsor desvela su decoración navideña en las primeras festividades sin Isabel II y con Carlos III como rey
    Una gran fiesta en el pequeño mundo ideal de ICON
    Sumer, el ‘kebab’ artesano de barrio en Madrid que acoge tertulias filosóficas
    Sara Carbonero, operada de urgencia tres años después de superar un cáncer de ovario
    Camila y los 1.000 osos Paddington: la reina entrega a una ONG infantil los peluches en homenaje a Isabel II
    Salen a subasta 175 objetos de Marilyn Monroe: de la carta única de su padre a unas pestañas postizas  
    Manuel Outumuro toca cumbre
    Diane de Beauvau-Craon, la última princesa rebelde: “Me drogué mucho, bebí mucho alcohol, me acosté con muchos gais y aquí sigo”
    Marta Ortega reúne en A Coruña a grandes protagonistas de la moda internacional en la inauguración de la muestra sobre Steven Meisel
    Antonio Alvarado: “La moda pudo conmigo, pero me aportó más de lo que me perjudicó”
    El Barça se viste de Herno
    Humaredas mediáticas, monotonía, discursos vacíos y otras amenazas y retos de la gastronomía 
    Sumer, el ‘kebab’ artesano de barrio en Madrid que acoge tertulias filosóficas
    Los guardianes de la ensaladilla rusa, la tapa popular que subió a los altares ‘gourmet’ 
    Ishida, los ‘dioses’ de la cocina japonesa: “Tenemos que dejar de desear tantas cosas, y hay que hacerlo ya”  
    Una selección imprescindible de productos con descuento: comprar en Black Friday nunca fue tan fácil
    El ‘bon vivant’ acorralado de la FIFA que grabó a sus amigos
    Leonor Lavado: “Somos como hablamos: la voz es nuestro ADN psicológico”
    ¿Qué ocurre tras la edad de oro de la televisión? El mismo oro, aunque enterrado bajo una oferta masiva
    Adiós a Ellen Pompeo, la funcionaria de la tele
    ‘This England’
    El gol a Infantino de dos ministras europeas
    ‘Los marginados’ de Carmen Sarmiento, televisión adulta
    ‘La ruta’: por qué nos invade la nostalgia del ‘after’
    La veteranía de María del Monte y Francisco se mide con la juventud de María Terremoto y Juanlu Montoya en los premios Radiolé  
    La violencia machista entre los adolescentes, el drama que ni ellos quieren reconocer
    ‘La Sagrada Familia’ rescata el mito Pujol y disecciona su caída
    Álex Pina, creador de ‘La casa de papel’, encierra a ricos en un búnker de lujo durante el fin del mundo en su nueva serie en Netflix
    Regreso al hospital terrorífico de Lars von Trier
    Ander Puig, el fichaje trans de ‘Élite’: “Voy a recibir mucho amor y mucho odio”
    Eurovisión permitirá votos de espectadores de todo el mundo a partir de 2023
    Berto Romero se pasa al terror, sobrenatural aunque naturalista, en la serie ‘El otro lado’
    Por qué se quebró Ronaldo en París: “Éramos gladiadores”
    ¿Qué ver hoy en TV? Domingo 27 de noviembre de 2022
    Las series de agosto de 2022: ‘La casa del dragón’ en HBO Max; ‘Sandman’ en Netflix y otras
    Nueve capítulos para recordar ‘The Wire’ en su 20º aniversario
    Harry Palmer: el tercer vértice del mágico triángulo de espías británicos
    Las series de junio de 2022: ‘The Boys’ en Amazon Prime Video; ‘Peaky Blinders’ en Netflix y otras
    Llega la nueva serie de Jeff Bridges, que no da un minuto de tregua
    Las abuelas que han viralizado el arte de elaborar la pasta italiana 
    El misterio de Manuel Carrasco: cómo salir de una barriada de pescadores y acabar siendo un cantante que llena estadios
    Muchos hombres, una sola mujer
    Ishida, los ‘dioses’ de la cocina japonesa: “Tenemos que dejar de desear tantas cosas, y hay que hacerlo ya”  
    Humaredas mediáticas, monotonía, discursos vacíos y otras amenazas y retos de la gastronomía 
    Los guardianes de la ensaladilla rusa, la tapa popular que subió a los altares ‘gourmet’ 
    Cerdo pío negro, el inesperado rival del ibérico
    Narcisistas, ansiosos, pasivo-agresivos… Cinco claves para tratar con personas difíciles
    Al fondo, invisibles, las pirámides
    Viaje al sabor de la tradición
    Todo es mejor con chocolate y estas cinco recetas lo demuestran
    Crecer bajo las bombas
    El secreto del maíz gigante mexicano que bajó del volcán
    Quién era Abarth y por qué un escorpión es su emblema 
    El milagro alemán
    Consuelo
    Sin tiempo
    La bióloga que se propuso repoblar los bosques de Brasil
    Un parche para conseguir que las vacunas sean más baratas y accesibles
    Cerdo pío negro, el inesperado rival del ibérico
    Ishida, los ‘dioses’ de la cocina japonesa: “Tenemos que dejar de desear tantas cosas, y hay que hacerlo ya”  
    El secreto del maíz gigante mexicano que bajó del volcán
    ‘Mis primeros recuerdos’, por Daniel Barenboim
    El indómito espíritu creativo de Picasso
    Medio siglo sin Picasso
    Paloma Picasso se confiesa con Nuccio Ordine
    El amigo de Picasso sin el que no estaría en España el ‘Guernica’
    Tommy Hilfiger: “Muchos de nuestros clientes van a vivir en el metaverso. De hecho, ya lo hacen”
    Storm Pablo: el estilista que convirtió a Bad Bunny en icono también de la moda
    El hombre que cultiva las flores más caras para los perfumes más especiales
    Una casa junto al lago Como que es pura diversión 
    Desayuno a la mexicana entre hípsters de mañaneo y polis con más apetito que buena fama
    El misterio Picasso
    Isabel II: el reinado de la imagen
    Un día en la vida de un país: San Sebastián-Cádiz en 16 horas
    Luces y sombras de Robert Mapplethorpe
    A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:
    Feminismo
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    El feminismo se fractura en Madrid en las protestas contra la violencia machista que recorren España
    Igualdad
    El caso de Georgia, en EE UU: becar sin importar la renta agranda la desigualdad
    Mujeres
    Otras mujeres
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    ¿Protege más a las mujeres elevar las penas?
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    El embarazo transforma el cerebro de las mujeres para favorecer el vínculo con sus hijos
    Otras mujeres
    El primer protagonista homosexual de Disney y un ejército de mujeres capitaneada por Viola Davis, entre los estrenos de la semana
    Mujer
    Otras mujeres
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    ¿Protege más a las mujeres elevar las penas?
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    El embarazo transforma el cerebro de las mujeres para favorecer el vínculo con sus hijos
    Otras mujeres
    El primer protagonista homosexual de Disney y un ejército de mujeres capitaneada por Viola Davis, entre los estrenos de la semana
    Confesiones de la mujer que lleva 40 años decidiendo quién será James Bond
    Muchos hombres, una sola mujer
    Brecha salarial
    
    Machismo
    
    Violencia
    Otra forma de violencia política
    La violencia verbal de Vox desborda el Congreso español
    
    Otra forma de violencia política
    Contra la violencia machista 
    Otra forma de violencia política
    Abascal defiende la violencia verbal de Vox y llama “enloquecida” a la ministra Irene Montero 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    El feminismo se fractura en Madrid en las protestas contra la violencia machista que recorren España
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    328 mensajes de tu ex o cómo la violencia machista entra por el móvil
    La violencia machista entre los adolescentes, el drama que ni ellos quieren reconocer
    Maltrato
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    Homicidio
    
    Género
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Por primera vez un juez declara nulo un contrato de alquiler por aplicación de la perspectiva de género
    Visitas a centros de acogida y muchas horas de estudio: así se forman los jueces en materia de género
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Asesinato
    Crónica del asesinato de una niña en la Francia rural
    Crónica del asesinato de una niña española en la Francia rural
    Sexo
    
    

Luego Tenemos que instalar las Librerías para realizar el web scraping


```python
pip install requests bs4 pandas termcolor
```

    Requirement already satisfied: requests in c:\users\gabri\anaconda3\lib\site-packages (2.28.1)
    Requirement already satisfied: bs4 in c:\users\gabri\anaconda3\lib\site-packages (0.0.1)
    Requirement already satisfied: pandas in c:\users\gabri\anaconda3\lib\site-packages (1.4.4)
    Requirement already satisfied: termcolor in c:\users\gabri\anaconda3\lib\site-packages (2.1.1)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (1.26.11)
    Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (2.0.4)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (2022.9.14)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\gabri\anaconda3\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: beautifulsoup4 in c:\users\gabri\anaconda3\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: pytz>=2020.1 in c:\users\gabri\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: six>=1.5 in c:\users\gabri\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\gabri\anaconda3\lib\site-packages (from beautifulsoup4->bs4) (2.3.1)
    Note: you may need to restart the kernel to use updated packages.
    

### Librerías

#### Librerías internas

- CSV:(Valores Separados por Comas) es el formato más común de importación y exportación de hojas de cálculo y bases de datos.
- RE:Este módulo proporciona operaciones de coincidencia de expresiones regulares similares a las encontradas en Perl.
- TIME:Este módulo proporciona varias funciones relacionadas con el tiempo. Para la funcionalidad relacionada, consulte también los módulos datetime y calendar.
- OS:Este módulo provee una manera versátil de usar funcionalidades dependientes del sistema operativo. 


#### Librerías externas 

- Termcolor: Es una biblioteca que sirve para imprimir mensajes de colores en el terminal.
- bs4: Beautiful Soup (bs4) es una biblioteca de la cual podemos obtener datos en formato HTML y XML
- requests: Se usa para hacer solicitudes y peticiones a la página de la que extraeremos datos.
- pandas: Es una herramienta de análisis de datos de código, de lectura rápida en el lenguaje de programación de Python.

Luego Importamos las librerias para que los siguentes comandos puedan trabajar 


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

### Variables 

Creamos una variable llamada **resultado**


```python
resultados = []
```

Para organizar en forma de lista los datos que nos del código de resultado utilizaremos *Type*


```python
type(resultados)
```




    list



El paso siguiente solicitar el acceso de los datos del portal Web para imprimir los titulares **El PAÍS**

### Solicitud de acceso 

req = requests.get("https://resultados.elpais.com")

Despues 


```python
type(req)
```




    requests.models.Response



Para solo usar valores iguala a 200 se debe usar el elemnto **if** para que nos muestre solo los estados satisfactorios.

### Beautiful Soup

Se agrega la variable Beautiful para guardar los *Tags* para que se añadan en lista los titulos

Añadimos la variable para encontrar las **h2** através de un **for** y se impriman las etiquetas y sus textos.


```python
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')
```


```python
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
    Las protestas se extienden en China contra la política de covid cero
    La gestión del frío enfrenta a Zelenski y al alcalde de Kiev
    La vida bajo los bombardeos rusos
    Así se vive en un refugio invernal durante la guerra
    Pobreza en el Olimpo académico de EE UU: la huelga que cimbra a la Universidad de California 
    El caótico primer mes de Elon Musk en Twitter
    ‘Argentina, 1985’, un debate nacional entre la ficción y la memoria
    Alemania rescata un empate contra España sobre el final del partido
    Un empate socialdemócrata
    Datos y gráficos | Alemania explota un error de España para empatar un partido equilibrado
    Croacia da vuelta el partido y elimina a Canadá (4-1)
    Marruecos da un batacazo a Bélgica sobre el final (0-2)
    Costa Rica se redime ante un Japón sin puntería (0-1)
    Madrid, la nueva Miami: así se han hecho con la capital española los ricos latinoamericanos
    López Obrador saca músculo en las calles con una manifestación masiva en México
    El Bosque, el pueblo mexicano que se tragó el mar
    Argentina contra la impunidad de los feminicidios
    Neofascistas, nacionalpopulistas, tecnosoberanistas. ¿Cómo llamamos a las nuevas derechas radicales? 
    Las abuelas que han viralizado el arte de elaborar la pasta italiana
    Pepa Bueno: “Las páginas de EL PAÍS tienen que ser el lugar donde los diferentes se encuentren”
    Videoanálisis | La FIL mastodóntica y popular está de vuelta
    La FIL de Guadalajara pone una vela al libro y otra al balón
    Concepción Company: “De todos los mexicanismos me quedo con apapachar”
    El acoso invernal de Putin 
    Por el bien de todos
    Otra forma de violencia política
    Yo te vi, papá, emocionarte con Messi
    Ideas de regalos para el jardinero
    Guía de regalos para el ‘foodie’
    Bolsonaro reaparece en una ceremonia militar tras batallar su derrota desde la trastienda
    El sueño hecho realidad del refugiado sirio del selfi con Merkel
    Crónica del asesinato de una niña en la Francia rural
    La violencia verbal de Vox desborda el Congreso español
    
    El negocio de las chicas imagen en las discotecas: “La misión es sonreír y que los hombres beban más”
    Las guatemaltecas que estudian ingeniería para llevar luz a sus comunidades
    Impresiones 3D y Telegram: el premiado proyecto de estudiantes colombianos para potabilizar agua
    La ‘ciudad esponja’: diez soluciones para resolver el problema del agua en México
    Cómic y energía nuclear: el superventas francés que sacude el debate sobre el cambio climático
    En la biblioteca de Almudena Grandes
    Otras mujeres
    Adiós a Ellen Pompeo, la funcionaria de la tele
    ¿Selfie sí o selfie no en Art Basel?
    De las galerías a las calles: así se hizo importante Miami para el arte del mundo
    La bestial tensión sexual entre Bruce Willis y Cybill Shepherd en ‘Luz de luna’, la serie en la que la actriz tuvo mucho que decir
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    Alessandro Michele, crónica de una salida anunciada
    Leonor Lavado: “Somos como hablamos: la voz es nuestro ADN psicológico”
    De la carnicería de su padre en España a la estrella Michelin en Chicago
    Macondo Inundado: el pueblo donde nunca deja de llover 
    Dormir en una caja a 200 euros la noche para asistir al Mundial de Qatar
    Retrato de Pablo Milanés a través de sus 10 canciones más decisivas
    De Honduras a Ucrania: cuando un niño crece bajo las bombas
    Qatar 2022, el único mundial donde es posible ver dos partidos en un mismo día
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Enredados en el Mundial | Los jugadores iraníes vuelven a cantar el himno y ha nacido una estrella en EE UU
    Al menos 500 alpacas mueren por una ola de frío en Perú
    Los partidarios de Bolsonaro utilizan sus móviles para pedir un golpe “extraterrestre” 
    Cuatro carceleros dan un brutal paliza a un hombre negro en Georgia
    Protests spread across China as anger builds over Xi Jinping’s zero-Covid policy 
    War in Ukraine: The battle to survive sub-zero temperatures 
    The story of a crypto scammer that ended in suicide
    To boost oil supplies, US looks to lift sanctions on Venezuela
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Toda la actualidad científica en el boletín de Materia
    Letras Americanas: la actualidad literaria de un continente vista por el escritor Emiliano Monge
    Ideas: reportajes y entrevistas para entender el mundo
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    El primer ministro de Rumania: “Necesitamos un esfuerzo común en la OTAN para defender cada centímetro de territorio frente a Rusia”  
    La justicia investiga si el Gobierno de Macron favoreció a consultoras privadas en las dos últimas campañas presidenciales en Francia
    Aquí puede buscar si ha sido engañado por la estafa internacional de las criptomonedas
    El secreto de la pirámide
    El futuro de las compras: más redes sociales, pago a plazos y vuelta de la tienda física
     El Papa detecta fallos en Caritas Internationalis y cesa a sus responsables 
    La Iglesia italiana da por primera vez cifras de los abusos cometidos por el clero
    El Senado de EE UU da un paso clave para blindar el matrimonio homosexual frente al Supremo
    Muere Hans Magnus Enzensberger, gran intelectual alemán del siglo XX
    ‘Close’, una mirada conmovedora a la fragilidad de la preadolescencia
    La gran retrospectiva de Vermeer en Ámsterdam aviva la polémica sobre la autoría de ‘Muchacha con flauta’
    Vivir con un trastorno alimentario: “Me di cuenta cuando me miré al espejo y vi la muerte”
    Josefa Ros Velasco, filósofa: “Si alguien se aburre suele darse a la botella, cuando le pasa a un país suele darse una revuelta”
    La insólita historia de la mujer que descubrió el primer antibiótico español
    Canadá conquista su primera Davis a lomos de Aliassime
    La selección femenina de baloncesto se clasifica para el próximo Eurobasket
    La trituradora del Barcelona no tiene piedad con el Atlético (1-6)
    Operación ‘OS35’: cómo rescatar un gigante de 40.288 toneladas varado a la sombra de Gibraltar
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    La izquierda retira por sorpresa y a última hora la propuesta para abolir los toros en Francia 
    Mastodon: qué es y cómo funciona la red social en la que los usuarios deciden qué está permitido
    Así serán las nuevas marcas de verificación en Twitter: azul, oro y gris
    Gafas con funciones de un móvil, ‘Photoshop’ instantáneo y otros inminentes avances gracias a los nuevos chips
    Sánchez pide a la patronal que negocie con los sindicatos un acuerdo salarial
    El pasado franquista pervive en Santa Cruz de Tenerife
    La federación de la España Vaciada busca implantarse en todo el país 
    El ‘bon vivant’ acorralado de la FIFA que grabó a sus amigos
    ¿Qué ocurre tras la edad de oro de la televisión? El mismo oro, aunque enterrado bajo una oferta masiva
    ‘This England’, por Carlos Boyero
    Windsor desvela su decoración navideña en las primeras festividades sin Isabel II y con Carlos III como rey
    Camila y los 1.000 osos Paddington: la reina entrega a una ONG infantil los peluches en homenaje a Isabel II
    Stallone vs. Schwarzenegger, la “competición” eterna: “Éramos antagonistas. Soñaba con pegarle y él con pegarme a mí”
    El misterio de Manuel Carrasco: cómo salir de una barriada de pescadores y acabar siendo un cantante que llena estadios
    Los guardianes de la ensaladilla rusa, la tapa popular que subió a los altares ‘gourmet’ 
    Erri De Luca, escritor: “Construir una vida es más difícil que contarla”
    Descansar está mal visto: el arte perdido del reposo
    Perdidos en el laberinto del paro
    Su vecino lo timaba con la calefacción central
    En la cuneta del sueño americano
    Descuidos de seleccionador: los lectores agregan libros de fútbol que no entraron en la lista
    Mi combate contra la ablación y el VIH en Senegal
    Masacre en Melilla: la peligrosa decisión de socialistas y populares
    Oyambre, Son Bou y otras nueve playas españolas para un baño de historia
    Cómo actuar ante el caos de los aeropuertos: qué hacer frente a retrasos y cancelaciones de un vuelo
    Samantha Hudson: “Me va bien económicamante, pero no soy Paula Echevarría. Nunca seré normativa”
    Alaska: “No entiendo la cultura de la cancelación”
    ¿Es buena idea masturbarse antes de salir? Las verdades y mentiras de la relajación posorgasmo
    El dilema Kit Connor: ¿debe conocerse la sexualidad de un actor para interpretar un papel gay?
    Vender carne... y un estilo de vida: así son las nuevas hamburgueserías
    ¿Cuál es la mejor receta de puré de patatas?
    Las nuevas jubilaciones: más retiros parciales, casi a los 65 años y cobrando 1.258 euros
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Macarena Olona sorprende a todos al publicar este mensaje sobre Begoña Gómez
    Le van a llover los palos: la cantada de Courtois que mete en un lío gordo a Bélgica
    Ocho mil millones de cursis
    Las 10 mejores películas y sagas posapocalípticas
    

Este proceso se repetirá en cada sección del periódico digital 


```python
req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


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


```python
req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python

req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```


```python
req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

para limpiar los resultados usamos **os.system("clear")**


```python
os.system("clear")
```




    1



con print(colored) se mostrarn los titulos con estilo **BOLD**

### Color

A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:
Feminismo


```python
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))
```

    A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:
    Feminismo
    

Utilizando la funcion **For** para comprobar que tengan las palabras claves, este se repite una y otra vez 


```python
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
```

    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    El feminismo se fractura en Madrid en las protestas contra la violencia machista que recorren España
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
    El caso de Georgia, en EE UU: becar sin importar la renta agranda la desigualdad
    Mujeres
    Otras mujeres
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    ¿Protege más a las mujeres elevar las penas?
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    El embarazo transforma el cerebro de las mujeres para favorecer el vínculo con sus hijos
    Otras mujeres
    El primer protagonista homosexual de Disney y un ejército de mujeres capitaneada por Viola Davis, entre los estrenos de la semana
    Otras mujeres
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    Mujer
    Otras mujeres
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    ¿Protege más a las mujeres elevar las penas?
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    El embarazo transforma el cerebro de las mujeres para favorecer el vínculo con sus hijos
    Otras mujeres
    El primer protagonista homosexual de Disney y un ejército de mujeres capitaneada por Viola Davis, entre los estrenos de la semana
    Confesiones de la mujer que lleva 40 años decidiendo quién será James Bond
    Muchos hombres, una sola mujer
    Otras mujeres
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Brecha salarial
    
    Machismo
    
    Violencia
    Otra forma de violencia política
    La violencia verbal de Vox desborda el Congreso español
    
    Otra forma de violencia política
    Contra la violencia machista 
    Otra forma de violencia política
    Abascal defiende la violencia verbal de Vox y llama “enloquecida” a la ministra Irene Montero 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    El feminismo se fractura en Madrid en las protestas contra la violencia machista que recorren España
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    328 mensajes de tu ex o cómo la violencia machista entra por el móvil
    La violencia machista entre los adolescentes, el drama que ni ellos quieren reconocer
    Otra forma de violencia política
    La violencia verbal de Vox desborda el Congreso español
    
    Maltrato
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    Homicidio
    
    Género
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Por primera vez un juez declara nulo un contrato de alquiler por aplicación de la perspectiva de género
    Visitas a centros de acogida y muchas horas de estudio: así se forman los jueces en materia de género
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Para acabar con la violencia de género, necesitamos más mujeres en posiciones de poder 
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Asesinato
    Crónica del asesinato de una niña en la Francia rural
    Crónica del asesinato de una niña española en la Francia rural
    Crónica del asesinato de una niña en la Francia rural
    Sexo
    
    
