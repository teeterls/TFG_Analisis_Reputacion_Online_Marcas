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







Los datos iniciales han sido extraídos del siguiente dataset de Kaggle: [Tweets about the Top Companies from 2015 to 2020](https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020/data)
