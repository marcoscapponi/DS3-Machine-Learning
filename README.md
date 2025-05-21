# DS3-Machine-Learning

En este proyecto buscaremos predecir en una manera general, de que esta hablando la noticia.
Estamos analizando un dataset de 7600 noticias, en las que tenemos 1900 noticias de deportes(sports), ciencia y tecnologia(sci/tech), negocios(business) y mundial(world).
Buscaremos predecir si las noticias de business o de world son de indole positivas o negativas. Para las noticias de sports predeciremos si se trata de resultados de partidos o de noticias generales sobre algun deporte. Y para las noticias de sci/tech queremos averiguar si la noticia tiene que ver o habla de inteligenicia artificial, o si la noticia es sobre otra tematica.
Aqui va una breve descripcion de como vamos a abarcar el proyecto, luego en este haremos una descripcion de cada paso que vayamos realizando, para que el trabajo sea lo mas entendible y practico posible.
Primero cargaremos e importaremos todsa las librerias necesarias para el trabajo, como sklearn, nltk, spacy, pandas, entre otras.
Cargamos el archivo csv donde contiene el todas las noticias, y luego le haremos un breve analisis exploratorio a estos datos.
Creamos una copia del dataset, para trabajar con mas tranuqilidad, sin riesgo de perdida o mala manipulacion de datos que nos coste perdida de informacion.
Aqui comenzamos con el procesamiento del lenguaje natural, donde usaremos algunas de las tecnicas mas comunes como tokenizacion, cambiar todos los caracteres a minuscula, lematizacion, stemming, removemos las stopwords, y todos los signos de puntuacion.
Por ultimo daremos paso a la prediccion y el deep learning, donde con metedos de prediccion como RandomForest, o LogisticRegression, mas las tecnicas de TF-IDF o Bag of Words, buscaremos lograr un entrenamiento acorde para la buena prediccion de las noticias.
Finalmente haremos una conclusion final sobre el trabajo y nuestro resultado obtenido.

Conclusion
Como conclusion podemos notar que nuestros dos metodos de deep learning funcionaron con eficacia y nos dieron buenos resultados. Nos inclinamos mas por el metodo tf-idf, y el metodo de prediccion que mejor accuaracy nos dio fue el XG-Boost.
En el analisis para determinar si las noticias de business o world eran positivas o negativas, utilizamos Sentiment Intensity Analyzer, y una funcion para separar el valor del texto en positivo o negativo segun su valor/peso.
En el caso de la noticias de sports, usamos la metodologia de tf-idf y comparamos entre tres modelos de prediccion para seleccionar cual es el que mejor resultado nos brinda, que en este caso fue el XG-Boost con un accuaracy de 0.92.
Para el ultimo caso de estudio, quisimos buscar si las noticias de sci/tech hablaban de inteligencia artificial o no. Para esto vectorizamos las palabras y luego con el modelo random forest classifier y un uso de gridsearchCV para obtener mejor presicion en la busqueda, obtenemos resultados casi perfectos con accuaracy de 0.99.
Como proyeccion a futuro, si usamos un dataset de mayor tamanio, con mas noticias, debemos analizar y de necesitarlo, ajustar parametros o probar modelos nuevos para no perder nuestros valores de accuaracy.
