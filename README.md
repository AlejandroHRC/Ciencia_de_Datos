# Ciencia_de_Datos
 Proyectos
Proyecto unidad 4 - Analisis de sentimientos
El dataset usado contiene las reviews de la serie One piece estrenada 31 de agosto de 2023.
Este proyecto busca que podelo de machine learning tiene un mejor desempeño para la prediccion de la columna Rating, entrenando el modelo
con los comentarios de las reviews de los usuarios.

Paso 1
Hacemos una breve exploracion de los datos conociendo su tipo si existen datos nulos y un breve vistazo de los datos en las columnas.
Realizamos una distincion de los datos nulos existentes en el dataset, ademas de mostrar una grafica con la distribucion de los datos,
con la intencion de ver su comportamiento.

Paso 2
Analisis de sentimientos, fue necesario crear una funcion que puediera obtener las palabras mas importantes las cuales nos ayudarian a poder predecir una polaridad en la intencion de los usuarios y asi clasificar el comentario, algunas herramientas utilizadas fue la libreria NLTK para el procesamiento de lenguaje natural.
Se hizo un prepocesamiento de las columnas Review y Title para tokenizar las palabras ademas de eliminar Stopwords.
Se hizo un analisis de sentimientos a estas dos columnas y se agrego el resltado obtenido a el dataframe.

Paso 3
Entrenamiento de los modelos de Machine Learning para la prediccion de la columna Review
Se Utilizaron 3 modelos KNN, SVM Y Random Forest, cada uno con sus respectivos parametros.
Se hizo una division de los datos con una distribucion de 85 - 15 para entrenamiento y pruebas respectivamente.
Como metrica de validacion se utilizo Accuracy, con la cual obtubimos resultados desfavorables asi que se utilizo RMSE para validadar los resultados, se comprobo la ineficiencia de los modelos creados, se concluyo que existen algunas posibles razones, la escaces de datos, o una eleccion equivoca de parametros en los modelos.