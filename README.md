# Natural Language Processing
For NLP Analysis:
- Get the text(strings)
- Tokenization
  - Type
    - 1. Word Tokenization (based on a certain delimiter)
      - Pretrained Word Embeddings
        - Word2Vec
        - GloVe
      - Issue
        - Out-of-Vocabulary (OOV) words
          - can be rescue with Unknown Token(UNK)
          - entity info may lost and every OOV gets same representation
        - Size
    - 2. Character Tokenization
      - overcomes the drawbacks about Word Tokenization (OOV, size)
      - increase the length of inputs and outputs rapidly
      - character do not contain info
    - 3. Sub-word Tokenization (n-gram characters)
  - Methods
    - split()
    - Regular Expressions (RegEx)
    - NLTK -> tokenize() -> word/sent_tokenize
    - TensorFlow.keras
    - Gensim
  - Parameters
    - punctuation, casing, accents
    - stop words, stemming, lemmatization
- Vectorization
  - CountVectorizer
  - TF-IDF
- ML task(recommend, detect spam, summarize, topic model...)

## NLP Algorithms
#### TF-IDF 
https://github.com/Shinuing/NLP/blob/main/Algorithms/TF-IDF%20From%20Scratch.ipynb  
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
#### Aritificial Neural Networks(ANN)
Tensorflow
- Binary Classification https://github.com/Shinuing/NLP/blob/main/Algorithms/TF2%20Linear%20regression%2C%20Binory%20classification.ipynb   
Data Resourse: Twitter US Airline Sentiment https://www.kaggle.com/crowdflower/twitter-airline-sentiment
- Multi-classification https://github.com/Shinuing/NLP/blob/main/Algorithms/TF2%20ANN%20with%20TF-IDF.ipynb   
Data Resourse: BBC News Text https://www.kaggle.com/shivamkushwaha/bbc-full-text-document-classification  
- Continuous Bag-of-Words(CBOW) https://github.com/Shinuing/NLP/blob/main/Algorithms/CBOW.ipynb  
Take the average of all embeddings
#### Convolutional Neural Networks(CNN)
Text Classification in Tensorflow https://github.com/Shinuing/NLP/blob/main/Algorithms/CNN%20Text%20Classification.ipynb   
Data Resourse: BBC News Text https://www.kaggle.com/shivamkushwaha/bbc-full-text-document-classification  
#### Recurrent Neural Netword(RNN)
- Text Classification in Tensorflow https://github.com/Shinuing/NLP/blob/main/Algorithms/RNN%20Text%20Classification.ipynb    
Data Resourse: BBC News Text https://www.kaggle.com/shivamkushwaha/bbc-full-text-document-classification    
- Part of Speech (POS) Tagging https://github.com/Shinuing/NLP/blob/main/Algorithms/Part%20of%20Speech%20(POS)%20Tagging.ipynb      
- Named Entity Recognition (NER) https://github.com/Shinuing/NLP/blob/main/Algorithms/NER%20TF2.ipynb  

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
#### IMDB Text Classification
https://github.com/Shinuing/NLP/blob/main/IMDB_text_classification.ipynb   
Sentiment analysis based on the review of movies
- transformers
