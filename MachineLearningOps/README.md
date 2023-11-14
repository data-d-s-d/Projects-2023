<img src="https://c4.wallpaperflare.com/wallpaper/577/286/481/steam-logo-hd-wallpaper-preview.jpg" alt="Logo de Steam" width="1200">

# Proyecto Individual Machine Learning Operations Steam Games
# Índice
1. [Descripción del Proyecto](#descripcion-del-proyecto)
2. [Resumen del Proceso](#resumen-del-proceso)
   - [Adquisición y Limpieza de Datos](#adquisicion-y-limpieza-de-datos)
   - [Ingeniería de Características](#ingenieria-de-caracteristicas)
   - [Desarrollo de la API](#desarrollo-de-la-api)
   - [Implementación](#implementacion)
   - [Análisis Exploratorio de Datos (EDA)](#analisis-exploratorio-de-datos-eda)
   - [Modelo de Aprendizaje Automático](#modelo-de-aprendizaje-automatico)
   - [Presentación en Video](#presentacion-en-video)
3. [Video de Presentación](#video-de-presentacion)
4. [Conclusión](#conclusion)
5. [Tecnologías utilizadas] (#tecnologias-utilizadas)
# README del Proyecto MVP - Análisis y Recomendación de Juegos <a name="descripcion-del-proyecto"></a>

## Descripción del Proyecto

Este proyecto está orientado al análisis y recomendación de juegos. 
El objetivo principal es abordar el procesamiento de datos relacionados con juegos a través de la lectura, limpieza y disponibilidad 
de estos datos a través de una API, así como desarrollar un sistema de recomendación basado en aprendizaje automático.

## Resumen del Proceso <a name="resumen-del-proceso"></a>

El proyecto se ha desarrollado en varias etapas clave:

### 1. Adquisición y Limpieza de Datos <a name="adquisicion-y-limpieza-de-datos"></a>

En esta fase, se trabajó con tres archivos JSON que contenían datos relacionados con juegos. Se llevaron a cabo las siguientes acciones:

- Descompresión de los archivos JSON.gzip
- Importación de los datos en Python utilizando dataframes (pandas).
- Limpieza de los datos, incluyendo la eliminación de columnas innecesarias y la preparación de los datos para su análisis posterior.

### 2. Ingeniería de Características <a name="ingenieria-de-caracteristicas"></a>

El proyecto incluyó la creación de una nueva característica llamada 'sentiment_analysis' mediante el análisis de sentimiento basado en procesamiento 
de lenguaje natural (NLP) aplicado a las reseñas de los usuarios. Esta característica asigna valores '0' para sentimiento negativo,
'1' para sentimiento neutral y '2' para sentimiento positivo. Además, esta nueva característica reemplaza la columna 'user_reviews.review' 
para facilitar el análisis de datos y el uso en modelos de aprendizaje automático.

### 3. Desarrollo de la API <a name="desarrollo-de-la-api"></a>

Se implementó una API utilizando el marco FastAPI para proporcionar acceso a los datos procesados. 
Se crearon los siguientes endpoints con los decoradores adecuados (@app.get('/')):

- developer: Devuelve la cantidad de elementos y el porcentaje de contenido gratuito por año para un desarrollador específico.
- userdata: Proporciona información sobre un usuario, incluyendo el dinero gastado, el porcentaje de recomendación basado en reseñas y la cantidad de elementos.
- UserForGenre: Ofrece el usuario con más horas jugadas para un género específico y una lista de horas jugadas por año de lanzamiento.
- best_developer_year: Devuelve los 3 mejores desarrolladores con los juegos más recomendados por los usuarios para un año determinado.
- developer_reviews_analysis: Proporciona un diccionario con el número total de reseñas de usuarios categorizadas como positivas y negativas para un desarrollador específico.

### 4. Implementación

La API desarrollada se implementó en la plataforma Render, para que sea accesible a través de un browser.

### 5. Análisis Exploratorio de Datos (EDA)
Se realizó un Análisis Exploratorio de Datos manual para explorar relaciones, detectar valores atípicos o anomalías, y descubrir patrones interesantes en los datos. Además, se crearon nubes de palabras para visualizar las palabras más frecuentes en los títulos de los juegos, entre otras visualizaciones.

### 6. Modelo de Aprendizaje Automático
Se construyó un sistema de recomendación basado en aprendizaje automático. Pudimos elegir entre un sistema de recomendación de ítem-ítem o de usuario-ítem. Decidí realizar la primera opción:
recomendacion_juego: Dado un ID de producto, devuelve una lista de 5 juegos similares.
Para probar el funcionamiento tanto del modelo de machine learning como de todos los endpoints del proyecto: https://proyecto-steam-games.onrender.com/docs

Considero necesario dar cuenta de que realicé un recorte de la matriz de datos para realizar el modelo, ya que no podía subirla a Render. Utilicé 4000 juegos aproximadamente, en lugar de 10000 que tenía inicialmente.

### 7. Presentación en Video
Se creó una presentación en video para demostrar el funcionamiento de los puntos finales de la API y proporcionar una breve descripción del modelo de aprendizaje automático utilizado para las recomendaciones.


## Video de Presentación <a name="video-de-presentacion"></a>

- El video debe mostrar los puntos finales de la API en funcionamiento y proporcionar una breve descripción del modelo de aprendizaje automático utilizado para las recomendaciones. El video debe tener una duración máxima de 7 minutos.

- [video: https://proyecto-steam-games.onrender.com/docs](https://drive.google.com/file/d/1f0ri2eLVHPHSWGqOCzbSTpigaazKGwFm/view?usp=sharing)

## Conclusión <a name="conclusion"></a>
A modo de conclusión, creo que es posible sostener que el resultado del proyecto fue un éxito, a pesar de todas las dificultades que se presnetaron a lo largo del camino. Todos los requisitos del proyecto han sido cumplidos, es decir que todos los endpoints requeridos fueron satisfechos, y el modelo de machine learning de recomendación funcionó a la perfección. 


Muchas gracias por el interés.


## Contacto: 

<a href="https://www.linkedin.com/in/diego-saint-denis/">
  <img src="https://cdn1.iconfinder.com/data/icons/logotypes/32/circle-linkedin-512.png" width="25" height="25">
</a>


## Tecnologías utilizadas
Python | Pandas | Matplotlib | Seaborn | Scikit-Learn | Difflib | FastAPI | Render
