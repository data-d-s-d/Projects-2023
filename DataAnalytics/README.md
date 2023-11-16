# Proyecto Individual 2: Análisis de Datos de Telecomunicaciones.
<img src="https://images7.alphacoders.com/108/1087509.jpg" alt="conexion" width="1200">

## Índice

1. [Introducción](#introduccion)
2. [Descripción del Proyecto](#descripción-del-proyecto)
3. [Contenido del Repositorio](#contenido-del-repositorio)
4. [Fuente de Datos](#fuente-de-datos)
5. [Conclusiones](#conclusiones)
6. [Contacto](#contacto)
7. [Tecnologías Utilizadas](#tecnologías-utilizadas)

## Introducción
Este repositorio contiene un proyecto de análisis de datos que tiene como objetivo evaluar una serie de datasets originarios de https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/ acerca de las telecomunicaciones en Argentina.
El objetivo general del proyecto es preparar los dataset a través de un proceso de ETL (Extract, Transform and Load),  el EDA (Exploratory Data Analysis) correspondiente para tratar los valores nulos,
eliminar datos duplicados y revisar outliers, para así poder crear un dashboard en Power BI de los datos más relevantes, y poder graficar el KPI propuesto (aumentar el acceso al servicio de internet para el próximo trimestre, específicamente para cada 100 hogares, en las diferentes provincias de Argentina), así como uno creado por mí, que tuvo como objetivo aumentar un 8% los accesos a internet por hogar para las regiones noroeste y noresete del país, dado que allí era donde se presentaban las cifras más bajas de accesos a internet.

El proyecto se ha desarrollado utilizando herramientas como Python, SQL, Power BI y técnicas de análisis de datos.

## Descripción del Proyecto
El proyecto se centra en el cálculo de dos KPI (Indicador Clave de Desempeño):
- El primero mide el aumento en el acceso a Internet por cada 100 hogares en distintas provincias de Argentina. El cálculo se realiza mediante las siguientes fórmula:

KPI_1 = ((Nuevo acceso - Acceso actual) / Acceso actual) * 100
Donde:

"Nuevo acceso" se refiere al número de hogares con acceso a Internet después del próximo trimestre.
"Acceso actual" se refiere al número de hogares con acceso a Internet en el trimestre actual.
El resultado del KPI_1 indica el porcentaje de aumento en el acceso a Internet en cada provincia para el próximo trimestre.

- El segundo Kpi(KPI_2) plantea como objetivo un crecimiento de 8% de los accesos a internet cada 100 hogares, para el año 2022 con respecto al año 2021 para las zonas de noroeste y nordeste del país, ya que de acuerdo al análisis hecho sobre los datos y la información extraída de estos, son las regiones del país que presentan un índice de conectividad y acceso a internet más bajo. Me pareció importante hacer este análisis, ya que hoy en día la posibilidad de conexión y acceso a internet pueden ser consideradas marcas de una sociedad igualitaria, dada la magnitud de esta herramienta y el impacto que puede tener, y de hecho tiene, en la vida de las personas. 
 
## Contenido del Repositorio
El repositorio contiene los siguientes elementos:

- ETL en Python: Un proceso de Extracción, Transformación y Carga de datos en Python para preparar y limpiar los datos originales.

- Exploratory Data Analysis (EDA) en Python: Un análisis exploratorio de datos en Python que examina y visualiza las tendencias y patrones en los datos. Es importante recalcar que algunos procesos correspondientes al ETL, principalmente el cambio de unidades de algunas tablas, fueron realizadas en el EDA.

- KPIs: Dos KPIs clave, uno de acuerdo a la consigna y otro adicional que busca aumentar el acceso a Internet en las regiones noroeste y noreste de Argentina.

- Dashboard en Power BI: Un informe interactivo en Power BI que muestra visualizaciones de los KPIs y otros datos relevantes.

- Dataset: Los conjuntos de datos utilizados en el proyecto, con información sobre el acceso a Internet por provincia y año.

Cómo Calcular el KPI
Para calcular el KPI, se utiliza la fórmula mencionada previamente. El KPI se calcula para cada provincia y se interpreta como el porcentaje de aumento en el acceso a Internet en esa provincia para el próximo trimestre. El informe en Power BI proporciona visualizaciones claras de estos KPIs y sus tendencias a lo largo del tiempo.

Una de las conclusiones interesantes que pude extraer de los datos es que las tecnologías que más crecimiento han sufrido en los últimos años son el cablemodem y la fibra óptica. Sin enbargo, la fibra óptica tiene muchísimo más potencial para crecer en los próximos años, especialmente en áreas donde su acceso no resulta tan complicado, por lo que es una oportunidad de inversión que no debe ser pasada por alto. Es importante recalcar que la fibra óptica no sólo va a llenar los espacios donde no haya conexiones preexistentes a internet, sino que tiene el potencial, y de hecho también lo está haciendo, de reemplazar a las tecnologías anteriores que presentan rendimientos muy inferiores.

## Dashboard
El dashboard del proyecto consiste en un informe interactivo en Power BI que muestra visualizaciones de los KPIs y otros datos relevantes para el análisis. Lamentablemente no se puede compartir acá directamente, pero a continuación voy a mostrar algunas fotos de cómo se veía.

![image](https://github.com/data-d-s-d/Projects-2023/assets/109982575/42e0286b-71e1-44dd-8b81-7b6f33e893df)


## Fuente de Datos
Los datos se han obtenido a través de conjuntos de datos principales y complementarios. Se ha utilizado una API para traer los datos necesarios. La combinación de estos conjuntos de datos ha permitido realizar un análisis más completo.

## Conclusiones
El proyecto demuestra la capacidad de calcular y visualizar KPIs clave para evaluar el aumento en el acceso a Internet en diferentes provincias de Argentina. Además, a partir de la información extraída de los datos, queda claro que la conectividad a través de internet en Argentina tiene mucho crecimiento por delante. Mi tarea era desempeñar un papel como empleado de una empresa de internet, y en ese rol pude concluir que hay un potencial inmenso de mercado en Argentina en lo que respecta, no sólo a la expansión de las conexiones (principalmente en las áreas alejadas de las ciudades grandes del país), sino también a las nuevas tecnlogías que ofrecen una inmensa mejoría en la calidad de las conexiones, como la fibra óptica, para las áreas ya conectadas al paradigma del internet.

Espero que este proyecto sea de utilidad y que sirva como ejemplo de análisis de datos en un entorno simulado. Si tienes alguna pregunta o comentario, no dudes en ponerte en contactarme a través de este repositorio o mi linkedin. ¡Muchas gracias por visitar el proyecto!

## Contacto: 

<a href="https://www.linkedin.com/in/diego-saint-denis/">
  <img src="https://cdn1.iconfinder.com/data/icons/logotypes/32/circle-linkedin-512.png" width="25" height="25">
</a>


## Tecnologías utilizadas:
Python | Pandas | Matplotlib | Seaborn | SQL | Power BI |
