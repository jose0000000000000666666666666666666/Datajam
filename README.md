# DataJam-Project: The Witness

Este es el repositorio del proyecto de investigación en el ámbito de la trata de personas del equipo Aleph Mind. Esto incluye todas las ideas o proyectos a futuro que se pueden desarrollar con nuestro proyecto. 
Así mismo esta es una guía del proyecto e incluye lo siguiente.

This is the repository of the Aleph Mind team's research project in the field of human trafficking. This includes all ideas or future projects that can be developed with our project.
This is also a project guide and includes the following: This is the repository of the Aleph Mind team's research project in the field of human trafficking. This includes all ideas or future projects that can be developed with our project.
Also this is a project guide and includes the following.

### Español

# Planteamiento del Problema

La trata de personas es una industria delictiva que constituye una de las violaciones mas grandes de derechos humanos. Esta ocurre cuando una persona es manipulada, controlada y explotada con la finalidad de obtener ganancias económicas. Una forma en la que se puede presentar la trata de personas es la explotación sexual. Esta consiste en forzar, engañar o coaccionar a una persona para que participe en actividades sexuales. Uno de los problemas más grandes es que la trata de personas se puede camuflar en la industria de Burdeles y agencias de acompañantes, modelaje webcam, hoteles y residencias privadas, salones de masaje, etc. Ahora bien, actualmente, la explotación sexual online y la explotación en viajes y turismo es de las formas mas frecuentes de trata de personas, por lo que se plantea una forma organización de la información que se puede encontrar en las diferentes paginas web de estos servicios, junto con el análisis de comunicados de prensa y sentencias judiciales, con el fin de generar una red que pueda guiar a encontrar los diferentes casos que puedan ser de trata de personas.

Con lo dicho anteriormente, la problemática que se aborda en este proyecto, se basa en el reto número 2 planteado por el datajam: "Enfoques de la NLU. Soluciones para procesar, clasificar, transformar y traducir grandes volúmenes de datos, como comunicados de prensa, sentencias judiciales, informes y declaraciones de víctimas". En este sentido, se considera que existe un problema en terminos de obtención y procesamiento de grandes volúmenes de información, de forma que permita analizar la información de comunicados de presa, informes, e incluso sentencias judiciales, esto enfocado al tráfico de personas en su forma de explotación sexual. Así mismo, en este proyecto se busca no solo en datos relacionados a los expuestos anteriormente sino que también se utiliza información de páginas web, que prestan servicios sexuales.


# Objetivo

#### - Objetivo General:
Análizar el subgrafo del internet que presenta posibles casos de trata de personas en su forma de explotación sexual.

#### - Objetivos Específicos:
- Obtener información de la web acerca de problemas relacionados con explotación sexual mediante un método denominado webscraping. 
- Realizar un grafo, que permita exponer las diferentes relaciones de la información recolectada en forma de red. 
- Hacer un análisis del grafo sobre la conexión de los diferentes conceptos, sentencias de autoridades judiciales, comunicados de prensa, reportes de ONGs, así como de información de las diferentes páginas web que prestan estos servicios.
- Proveer de una nueva fuente de información con los datos recolectados a travéz del internet
- Abrir el espacio, para que el modelo del grafo pueda ser utilizado en diferentes sectores y formas de trata de personas, no solo en su forma de explotación sexual.


# Solución / Descripción del uso de datos

La solución planteada por el equipo Aleph Mind consiste en realizar una búsqueda, por medio webscrapping y computación en paralelo, a traves de la web de servicios sexuales. Una vez recolectados estos datos, se almacenan en un grafo, que permite relizar las diferentes relaciones entre estas páginas, ya sea por numeros de telefonos repetidos, direcciones, links de referencia de una a otra página web. O por otro lado, porque mediante los comunicados de prensa referentes al tráfico de personas en su forma de explotación sexual, se ha hecho cierta mención a diferentes nombre u organizaciones.

# Pitch
Descripción del video: 
Entender las redes de trata de personas a través de un objeto matemático que capture la existencia y esencia de las relaciones que existen entre las diferentes personas, organizaciones o entidades que intervienen en la ejecución del delito resulta muy apropiado, pues, nos permite entre otras cosas, visualizar y encontrar patrones en la estructura de estas redes criminales, estudiando medidas de centralidad, influencia, existencia de comunidades y clusters, contactos, relaciones entre victimarios y victimas, puntos de concentración de los crímenes, rutas por las cuales se llevan a cabo las operaciones criminales, entre otras.

Ésto se conoce como Análisis de Redes Criminales y es precisamente el objetivo de The Witness: construir y estudiar el subgrafo del internet, en donde se enmarcan estas redes de trata personas.

The Witness utiliza modelos avanzados de Ciencia de datos e Inteligencia artificial para la obtención, procesamiento y análisis de grandes volúmenes de datos de la red, con el objetivo de extraer la información que sea de valor para las diferentes partes que intervienen en la lucha contra la trata de personas.

Adicionalmente, The Witness se propone conectarse a las principales plataformas y herramientas que ya han sido desarrolladas por distintas organizaciones que trabajan contra este delito como el Traffik Analysis Hub, facilitando la comunicación y el trabajo colaborativo entre organizaciones.


# Datos

Los datos son
- Datos recolectados a traves del websrcapping realizado.
- Comunicados de prensa obtenidos a traves de https://visual-insights.bluemix.net/?query=Sexual%20Explotation%20Colombia

# Código del proyecto

El proyecto está desarrollado en python, y para su funcionamiento se deben instalar las siguientes librerias por consola:
    - urllib: $ pip install urllib
    - requests: $ pip install requests
    - re: $ pip install re
    - hashlib: $ pip install hashlib 
    - langdetect: $ pip install langdetect
    - spacy: $ pip install spacy
             $ python -m spacy download es_core_news_sm
             $ python -m spacy download en_core_web_sm
    - networkx: $pip install networkx
    - $ pip install more-itertools
    - $ pip install nltk
    - $ pip install gensim
    - $ pip install beautifulsoup4

El código se divide en tres grandes modulos: un modulo tiene que ver con todo el algoritmo del webscrapping realizado, donde se encuentran las clases TheWitness y Website, cuyas funcionalidades consisten en extraer la infomación y almacenarla, respecctivamente para cada una de las clases.El segundo módulo hace uso de técnicas de Web Scraping junto con una aplicación de modelos de NLP (Procesamiento del lenguaje natural) con el objetivo de obtener información de valor de fuentes en la red. En este modulo se encontraran dos archivos: text_clustering_final, este módulo carga las funciones relacionadas con el uso del modelo NLP junto con el modelo en sí, y text_clustering, que se encarga del entrenamiento del modelo y se muestra la información de una forma interactiva de este entrenamiento. Finalmente, el tercer módulo consiste en la implementación del modelo, este es el módulo de los resultados del modelo, así mismo incluye ayudas visuales (visualización del grafo) y su análisis, este módulo contiene un solo archivo denominado Graph_Algorithm.

# Documentos Adicionales (Opcional) 

- PowerPoint presentation
- Flayers 
- Additional videos/demo
- Protocols  
- Guides 

# El Futuro de The Witness

Con The Witness consideramos que se pueden hacer muchos proyectos a futuro, pues como vimos en una de las charlas del evento, el problema del tráfico de personas se debe dejar de ver sectorizado para pensarse en contexto con todos sus posibles actores. Este proyecto más allá de exponer una nueva forma de visualización de la información, con nuevos datos sobre la tráfica de personas, busca que a futuro pueda ser utilizado y entrenado con más información, como sentencias judiciales de diferentes paises (que normalmente no son de facil acceso), para ser conectadas con toda la información que se puede conseguir en la red. Con esto en mente, se busca crear un modelo con la mayor cantidad de información para determinar los posibles centros de tráfico de personas y sus relaciones con otras entidades, para que así sea más sencillo para las autoriades, ONGs y organizaciones que trabajan en la temática de la trata de personas, ver y analizar la información.
Así mismo, se abre la posibilidad para que The Witness sea también una herramienta a ser utilizada en la Deep Web, pues este al ser un sitio donde se presenta gran cantidad de crímenes relacionados a la trata de personas, debe ser un sitio que se debe analizar, monitorear y pensar desde diferentes ramas del conocimiento, siendo así, The Witness tiene el objetivo de ser ese testigo, ese vigilante de la red, que pueda ayudar a que menos personas sean afectadas por la trata de personas.


### English

# Problem Statement

Human trafficking is a criminal industry that constitutes one of the largest human rights violations. This occurs when a person is manipulated, controlled and exploited in order to obtain financial gain. One way in which human trafficking can be presented is sexual exploitation. This consists of forcing, tricking or coercing a person into participating in sexual activities. One of the biggest problems is that human trafficking can be camouflaged in the brothel industry and escort agencies, webcam modeling, hotels and private residences, massage parlors, etc. Now, currently, online sexual exploitation and exploitation in travel and tourism is one of the most frequent forms of human trafficking, which is why a form of organizing the information that can be found on the different web pages of these services is proposed. , together with the analysis of press releases and court rulings, in order to generate a network that can guide finding the different cases that may be human trafficking.

With the aforementioned, the problem addressed in this project is based on challenge number 2 posed by the datajam: "NLU approaches. Solutions to process, classify, transform and translate large volumes of data, such as press releases , court decisions, reports and statements of victims ". In this sense, it is considered that there is a problem in terms of obtaining and processing large volumes of information, in a way that allows analyzing the information from press releases, reports, and even court decisions, this focused on human trafficking in its form of sexual exploitation. Likewise, this project seeks not only data related to those previously exposed but also uses information from web pages that provide sexual services.

# Objective

#### - General objective:
Analyze the subgraph of the internet that presents possible cases of human trafficking in the form of sexual exploitation.

#### - Specific objectives:
- Obtain information from the web about problems related to sexual exploitation through a method called webscraping.
- Make a graph that allows exposing the different relationships of the information collected in the form of a network.
- Make an analysis of the graph on the connection of the different concepts, judgments of judicial authorities, press releases, NGO reports, as well as information from the different web pages that provide these services.
- Provide a new source of information with the data collected through the internet
- Open the space, so that the graph model can be used in different sectors and forms of human trafficking, not only in its form of sexual exploitation.

# Solution/Data use case description 

The solution proposed by the Aleph Mind team consists of conducting a search, through webscrapping and parallel computing, through the sexual services website. Once these data are collected, they are stored in a graph, which allows the different relationships between these pages to be realized, either by repeated telephone numbers, addresses, reference links from one to another web page. Or on the other hand, because through press releases referring to human trafficking in its form of sexual exploitation, some mention has been made of different names or organizations.

# Pitch
Video description: Understanding human trafficking networks through a mathematical object that captures the existence and essence of the relationships that exist between the different people, organizations or entities involved in the execution of the crime is very appropriate, as it allows us, among other things, , visualize and find patterns in the structure of these criminal networks, studying measures of centrality, influence, existence of communities and clusters, contacts, relationships between perpetrators and victims, concentration points of crimes, routes by which the crimes are carried out. criminal operations, among others.

This is known as Analysis of Criminal Networks and it is precisely the objective of The Witness: to build and study the subgraph of the internet, where these human trafficking networks are framed.

The Witness uses advanced models of Data Science and Artificial Intelligence to obtain, process and analyze large volumes of data from the network, with the aim of extracting information that is of value to the different parties involved in the fight against human trafficking.

Additionally, The Witness intends to connect to the main platforms and tools that have already been developed by different organizations that work against this crime, such as the Traffik Analysis Hub, facilitating communication and collaborative work between organizations. 

# Datasets
The data is
- Data collected through the websrcapping performed.
- Press releases obtained through https://visual-insights.bluemix.net/?query=Sexual%20Explotation%20Colombia

# Project Code

The project is developed in python, and for its operation the following libraries must be installed per console:
    - urllib: $ pip install urllib
    - requests: $ pip install requests
    - re: $ pip install re
    - hashlib: $ pip install hashlib 
    - langdetect: $ pip install langdetect
    - spacy: $ pip install spacy
             $ python -m spacy download es_core_news_sm
             $ python -m spacy download en_core_web_sm
    - networkx: $pip install networkx
    - $ pip install more-itertools
    - $ pip install nltk
    - $ pip install gensim
    - $ pip install beautifulsoup4

The code is divided into three main modules: one module has to do with the entire webscrapping algorithm performed, where the TheWitness and Website classes are found, whose functionalities consist of extracting the information and storing it, respectively for each of the classes. The second module makes use of Web Scraping techniques together with an application of NLP (Natural Language Processing) models in order to obtain valuable information from sources on the network. In this module you will find two files: text_clustering_final, this module loads the functions related to the use of the NLP model together with the model itself, and text_clustering, which is in charge of training the model and displays the information in an interactive way. training. Finally, the third module consists of the implementation of the model, this is the module of the results of the model, it also includes visual aids (visualization of the graph) and its analysis, this module contains a single file called Graph_Algorithm.

# Additional docs (Optional) 

- PowerPoint presentation
- Flayers 
- Additional videos/demo
- Protocols  
- Guides 

With The Witness we believe that many projects can be done in the future, because as we saw in one of the talks at the event, the problem of human trafficking should no longer be seen as sectorized to be considered in context with all its possible actors. This project, beyond exposing a new form of information visualization, with new data on human trafficking, seeks that in the future it can be used and trained with more information, such as judicial decisions from different countries (which are usually not easy access), to be connected with all the information that can be obtained on the network. With this in mind, it seeks to create a model with the greatest amount of information to determine the possible centers of human trafficking and their relationships with other entities, so that it is easier for the authorities, NGOs and organizations that work on the subject. of human trafficking, view and analyze the information.
Likewise, the possibility is opened for The Witness to also be a tool to be used on the Deep Web, since this being a site where a large number of crimes related to human trafficking are presented, it must be a site that must analyze, monitor and think from different branches of knowledge, thus, The Witness has the objective of being this witness, this vigilant of the network, who can help to make fewer people to be affected by human trafficking.