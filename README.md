# Twitter Analisis de Sentimiento

## ¿Que hace el proyecto?

### Primera parte
El proyecto consiste en entrenar diferentes modelos para el reconocimiento de lenguaje natural y hacer una clasificación dependiendo si el texto es positivo o negativo.
Para la primera parte del proyecto se realizo siguiendo el siguiente tutorial: https://www.youtube.com/watch?v=FLZvOKSCkxY&list=PLQVvvaa0QuDf2JswnfiGkliBInZnIC4HL. Cambiando
la información que se estaba usando para entrenar los modelos a una proporcionada por Kaggle de Tweets.

Una vez construidos los modelos, se realiza el analisis de sentimiento en los Tweets en tiempo real usando la API de Twitter y se grafican también en tiempo real a manera de ver si los tweets de un tema en especifico son más negativos o más positivos o neutral

---
## Extras del proyecto
Se realizaron diferentes funcionalidades aparte del modelo principal como parte de la exploración del proyecto

### Red Neuronal Recurrente 
Con el fin de desarrollar una opción paralela al modelo utilizado, se desarrolló un model C-LSTM el cuál emplea una capa CNN y una LSTM. La primera permite una extración de las caracteristicas más importantes, mientras que la segunda, resuelve un problema de las RNN y permite reconocer dependencias de largo plazo. Para el preprocesamiento de los datos se utilizó la librería de Keras y para la asociación de palabras con su contexto se usó un modelo pre-entrenado: GloVe. El resultado fue un modelo con una precisión de 78%.

Durante el desarrolló una gran dificultad fue el sobreajuste, sin embargo, por la cantidad de datos utilizados y las técnicas de regularización se obtuvo un modelo estable a través de su entrenamiento y testeo. En expectativa, se buscaba obtener una precisión mayor a 80%, aunque se realizaron mejoras, no se pudo alcanzar esta meta. Sin embargo, comparado con trabajos similares es un buen rendimiento. No se incluirá en el modelo actual debido a que no se considera que aporta significativamente a lo establecido, sino como una opción paralela. 

### Analisis de Comentarios de Amazon

### Analisis de Comentarios de Youtube relacionado a likes y dislikes
El documento de sentiment analysis en YouTube emplea diversos modelos de clasificación de texto entrenados con la base de datos de Twitter para realizar dicha clasificación en comentarios de videos de YouTube. La intención de dicho programa no es de analizar el rendimiento de estos modelos (esto se realizó anteriormente obteniendo valores de accuracy cercana al 80%), sino de analizar la relación entre el porcentaje de comentarios positivos (100 * positivos / (postivios + negativos)) y el mismo de likes (100 * likes / (likes + dislikes)).

En cuanto a los resultados, se esperaba obtener una tendencia relativamente lineal que demostrase algún grado de correlación. No obstante, no se encontró ninguna tendencia o relación entre ambas variables, aunque esto no necesariamente significa que no valió la pena el desarrollo del modelo, puesto a que se pueden realizar diversas observaciones sobre los resultados (como una mayor tendencia en comentarios negativos que dislikes), el tipo de texto en los comentarios (como el hecho que son más cortos que Twitter y tienen una peor redacción y claridad), y acerca de los propios modelos (como las limitaciones de emplear algoritmos entrenados en una red social en otra).

### Reconocimiento de voz para el analisis de sentimiento


## ¿Por qué es útil el proyecto?
El proyecto nos permite ver las diferentes técnicas que existen para el reconocimiento de Lenguaje Natural y ver las ventajas y desventajas de cada uno de ellas. 
En los extras del proyecto intentamos a aplicar nuestros modelos a otros dominios para intentar hacer una predicción en un diferente contexto, sin embargo vemos que el rendimiento no es el esperado al que estabamos viendo con los tweets.
Esto se puede deber a múltiples factores ya que la información no esta muy bien balanceada o puede ser que el lenguaje informal y cotidiano de Twitter no se pueda aplicar a las reseñas de productos en Amazon o a comentarios en videos de Youtube.

## ¿Como empezar a desarrollar para el proyecto?
Se realizaron diferentes notebooks donde cada una esta relacionada a las diferentes técnicas o fuentes de información que se realizaron por cada integrante del equipo

## Para más información del proyecto
Para más información de este proyecto y de las aplicaciones que se investigaron dejamos unos links con las fuentes que resultaron de mucha ayuda para el desarrollo de este proyecto

https://www.kaggle.com/datasnaek/youtube?select=USvideos.csv
https://www.kaggle.com/c/twitter-sentiment-analysis2

## Contribuidores del proyecto
- Luis Daniel Vazquez (luis_060198@hotmail.com)
- Johan André Caballero (Johan.morlesin@gmail.com)
- Oscar Peña (oscarp_98@hotmail.com)
- Rodrigo Montero Castro (a01177008@itesm.mx)

