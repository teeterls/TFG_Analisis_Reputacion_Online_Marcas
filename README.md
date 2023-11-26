# Online reputation analysis of several brands using transformers
In this project, NLP techniques of topic modeling and sentiment analysis with transformers are used to analyze the online reputation of several brands - Apple, Tesla, Amazon, Google and Microsoft - from content published on X (Twitter) between 01-06-2019 and 01-01-2020. 
For topic modeling the [BERTopic](https://maartengr.github.io/BERTopic/index.html) model (based on BERT) ,designed specifically for this task, was used, while for sentiment analysis [BERTweet](https://huggingface.co/finiteautomata/bertweet-base-sentiment-analysis) model (based on RoBERTa) hosted on Huggingface was the one used, which is suitable for analyzing sentiment underlying English tweets. 

The analysis methodology was as follows:
1. Data selection
2. Cleaning and pre-processing
3. Descriptive analysis of N-frames (unigrams, bigrams, trigrams) using the TF-IDF algorithm.
4. Topical modeling
5. Sentiment analysis

As for the content of the repository, it contains the following files:
- [Descriptive data analysis](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Analisis_Descriptivo_Datos.ipynb): in this file the initial data is loaded, the temporal and company filtering is performed and the content distribution by company or the temporal evolution of the number of tweets is analyzed, among others.
  
* [N-Grams Analysis Apple and Tesla](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_NGramas_Apple_Tesla.ipynb): in this file the N-Grams analysis of the sets of tweets about Apple and Tesla is performed, applying the TF-IDF algorithm to obtain the most relevant unigrams, bigrams and trigrams. The most repeated terms are also visualized using word clouds.
  
+ [Amazon, Google and Microsoft N-Grams analysis](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_NGramas_Google_Amazon_Microsoft.ipynb): in this file the same N-Grams analysis procedure is repeated for the Amazon-Google-Microsoft set.
  
+ [Apple topic modeling](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Apple.ipynb): this file performs the topic modeling with the BERTopic model, obtaining the optimal number of the most relevant topics about Apple. It also includes multiple visualizations included in the model, such as intertopic distance, hierarchical clustering, similarity matrix or temporal evolution of the topics along the time span.
  
+ [Tesla topic modeling](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Tesla.ipynb): in this file the same topic modeling procedure is repeated for the Tesla ensemble.
+ [Amazon-Google-Microsoft topic modeling](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Modelado_de_To%CC%81picos_Amazon_Google_Microsoft.ipynb)::in this file the same topic modeling procedure is repeated for the Amazon-Google-Microsoft set.

+ [Sentiment analysis](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Ana%CC%81lisis_de_sentimientos.ipynb): this file contains the sentiment analysis of the 3 sets using the BERTweet model, in which for each tweet a positive (POS), negative (NEG) or neutral (NEU) categorization is obtained, as well as the corresponding confidence score or index.
+ [Sentiment Analysis - Graphs](https://github.com/teeterls/TFG_Analisis_Reputacion_Online_Marcas/blob/main/Analisis_Sentimientos_Gra%CC%81ficas_Todos_los_Conjuntos.ipynb): this file contains the code used for : overall distribution and temporal evolution of sentiment across sets, evolution of the model's confidence score, and distribution of sentiment and temporal evolution of sentiment for a set of relevant topics.

The initial data has been extracted from the following Kaggle dataset: [Tweets about the Top Companies from 2015 to 2020](https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020/data)
