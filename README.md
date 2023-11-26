# Analisis de la reputación online de varias marcas utilizando transformers
En este proyecto se utilizan técnicas NLP de modelado de tópicos y análisis de sentimientos con transformers para analizar la reputación online de varias marcas -Apple, Tesla, Amazon, Google y Microsoft- a partir de contenido publicado en X (Twitter) entre 01-06-2019 y 01-01-2020. 
Para el modelado de tópicos se ha utilizado el modelo [BERTopic](https://maartengr.github.io/BERTopic/index.html) (basado en BERT) diseñado específicamente para esta tarea, mientras que para el análisis de sentimientos se ha utilizado el modelo [BERTweet](https://huggingface.co/finiteautomata/bertweet-base-sentiment-analysis) (basado en RoBERTa) alojado en Huggingface, idóneo para analizar sentimiento subyacente a tweets en inglés. 

La metodología de análisis ha sido la siguiente:
1. Selección de datos
2. Limpieza y pre-procesamiento
3. Análisis descriptivo de N-Gramas (unigramas, bigramas, trigramas) mediante el algoritmo TF-IDF
4. Modelado de tópicos
5. Análisis de sentimientos

En cuanto al contenido del repositorio, este contiene los siguientes archivos:
- [Análisis descriptivo de datos](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Analisis_Descriptivo_Datos.ipynb) : en este archivo se cargan los datos iniciales, se realiza el filtrado temporal y por empresa y se analiza la distribución de contenido por empresa o la evolución temporal del número de tweets, entre otros. 
* [Análisis N-Gramas Apple y Tesla](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_NGramas_Apple_Tesla.ipynb) : en este archivo se realiza el análisis de N-Gramas de los conjuntos de tweets sobre Apple y Tesla, aplicando el algoritmo TF-IDF para obtener los unigramas, bigramas y trigramas más relevantes. También se visualizan los términos más repetidos mediante nubes de palabras.
+ [Análisis N-Gramas Amazon, Google y Microsoft](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_NGramas_Google_Amazon_Microsoft.ipynb) : en este archivo se repite el mismo procedimiento para el conjunto sobre Amazon-Google-Microsoft.
+ [Modelado de tópicos Apple](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Apple.ipynb)
+ [Modelado de tópicos Tesla](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Tesla.ipynb)
+ [Modelado de tópicos Amazon-Google-Microsoft](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Amazon_Google_Microsoft.ipynb)
+ [Análisis de sentimientos](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_de_sentimientos.ipynb)
+ [Análisis de sentimientos - Gráficas](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Analisis_Sentimientos_Gra%CC%81ficas_Todos_los_Conjuntos.ipynb)  

Los datos iniciales han sido extraídos del siguiente dataset de Kaggle: [Tweets about the Top Companies from 2015 to 2020](https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020/data)
