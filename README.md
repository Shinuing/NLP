# Natural Language Processing
For NLP Analysis:
- Get the text(strings)
- Tokenize the text
- Stopwords, stemming/lemmatization
- Map tokens to integers
- Convert into CountVectors/TF-IDF
- Do ML task(recommend, detect spam, summarize, topic model...)

## NLP Algorithms
#### TF-IDF 
https://github.com/Shinuing/NLP/blob/main/Algorithms/TF-IDF%20From%20Scratch.ipynb  
- with TensorFlow ANN 
  - Binary Classification https://github.com/Shinuing/NLP/blob/main/Algorithms/TF2%20Linear%20regression%2C%20Binory%20classification.ipynb   
  - multi-classification https://github.com/Shinuing/NLP/blob/main/Algorithms/TF2%20ANN%20with%20TF-IDF.ipynb   
Data Resourse: BBC News Text https://www.kaggle.com/shivamkushwaha/bbc-full-text-document-classification  
#### Word Embeddings
https://github.com/Shinuing/NLP/blob/main/Algorithms/Word%20Embeddings.ipynb  
Method: Word2Vec
Data Resourse: GoogleNews-vectors-negative300
#### Latent Semantic Analysis/Indexing (LSA/LSA)
https://github.com/Shinuing/NLP/blob/main/Algorithms/Latent%20Semantic%20Analysis%20CountVectorizer.ipynb  
Clustering by book titles
#### Latent Dirichlet Allocation (LDA)
https://github.com/Shinuing/NLP/blob/main/Algorithms/Latent%20Dirichlet%20Allocation.ipynb  
Topic Modelling BBC news
#### Non-Negative Matrix Factorization(NMF)
https://github.com/Shinuing/NLP/blob/main/Algorithms/Non-Negative%20Matrix%20Factorization%20(NMF).ipynb  
Topic Modelling BBC news

## NLP Applications
#### Movie Recommendataion system
https://github.com/Shinuing/NLP/tree/main/Movie%20Recommendation%20System  
Based on the movie gernes and keywords statistics to build a recommendation system and recommend the other 5 most relevant movies  
Data Resourse:tmbd https://www.kaggle.com/tmdb/tmdb-movie-metadata
- Text preprocessing and vector models
- TfidfVectorization
#### Markov Text Classifier
https://github.com/Shinuing/NLP/tree/main/Markov%20Text%20Classifier  
Build a classifier between two authors
Data Resourse: Edgar Allen Poe and Robert Frost Poetry Collection
- Word2Idx
- Markov Model
- Confusion Matrix, F1-score
#### Markov Poetry Generator
https://github.com/Shinuing/NLP/tree/main/Markov%20Poetry%20Generator  
Based on Robert Frost Poetry Collection to generator a four-line poetry
- List2Dict
- Cumulative Probability
- Second-order Markov Model
#### Spam Detection
https://github.com/Shinuing/NLP/tree/main/Spam%20Detection  
Build a classifier to predict if the SMS message spam or not  
Data Resourse: https://www.kaggle.com/uciml/sms-spam-collection-dataset  
- CountVectorizer + Lemma & wordnet
- Naive Bayes (MultinomialNB)
- Confusion Matrix, F1-score, ROC/AUC
- WordCloud
#### Sentiment Analysis
https://github.com/Shinuing/NLP/tree/main/Sentiment%20Analysis  
Build a classifier for a sentiment analysis about the problems of each major U.S. airline based on tweets  
Data Resourse: Twitter US Airline Sentiment https://www.kaggle.com/crowdflower/twitter-airline-sentiment  
- CountVectorizer
- Logistic Regression (multi-class, weighted)
- Confusion Matrix, F1-score, ROC/AUC
- WordCloud
#### Text Summarization
https://github.com/Shinuing/NLP/tree/main/Text%20Summarization  
BBC News summarization based on sentence scores and textrank  
Data Resourse: BBC News Text https://www.kaggle.com/shivamkushwaha/bbc-full-text-document-classification  
- Method 1: TF-IDF 
  - averaging non-zero means and return top scoring sentences
- Method 2: TextRank (based on Google PageRank)
  - sumy.TextRankSummarizer
  - sumy.LsaSummarizer
