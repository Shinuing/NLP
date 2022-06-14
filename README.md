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
Data Resourse: BBC News Text
#### Word Embeddings
https://github.com/Shinuing/NLP/blob/main/Algorithms/Word%20Embeddings.ipynb  
Method: Word2Vec
Data Resourse: GoogleNews-vectors-negative300

## NLP Applications
#### Movie Recommendataion system
https://github.com/Shinuing/NLP/tree/main/Movie%20Recommendation%20System  
Based on the movie gernes and keywords statistics to build a recommendation system and recommend the other 5 most relevant movies
Data Resourse:tmbd
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
- CountVectorizer + Lemma & wordnet
- Naive Bayes
- Confusion Matrix, F1-score, ROC/AUC
- WordCloud
