# Catching Crude Comments

## Abstract

Growing up, we were all introduced to the dangers of cyberbullying. We learned that a hateful comment or targeted insult could hold a lot of power. In today’s society, where most interactions are at least digitally adjacent, the impact and risk of toxic and hateful language online is all too real-and all more common. This project seeks to address this issue by accurately identifying trends across comments, and using to those trends to accurately predict comment toxicity. Using Natural Language Processing, supervised learning, and unsupervised learning, toxic comments will hopefully become much more trackable. And just for fun, maybe we create a comment generator to see how the language works!

## Design

The project is based off of a Kaggle data set found here: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge. The data looks at various wikipedia comments, seeking to classify them based on their toxicity. The goal is to accurately classify whether or not a comment falls into one of those toxicity categories, and what features are responsible for that classification.

## Data

The data is pulled from the Jigsaw Kaggle competition. It is data set of over 150,000 wikipedia comments, between 6 and 5000 characters in length. These wikipedia comments are classified into 6 categories, shown below. 
- Toxic
- Severe Toxic
- Obscene
- Threat
- Insult
- Identity Hate
In order to focus on the NLP nature of the project, I chose not to use these classifications in my models, but rather group them into a “Unsafe” bucket.

## Algorithms:
Feature Engineering:
- LDA
- SVC
- NMF
- KMeans Clustering 

## Models:
Naive Bayes, Logistic Regression, Random Forest, 
### Model Selection:
All data was first preprocessed using Regex, spaCy, and TextBlob. Preprocessing removed all punctuation, numbers, and other erroneous values in the string. Different preprocessing methods were attempted to identify best preprocessing technique. Lemmatization and stemming were both applied for best fit.
Data was vectorized using CountVectorizer and TfidfVectorizor, tokenized by word.

### Logistic Regression Scores
- Accuracy: 0.9552
- Precision: 0.8821
- Recall: 0.6455
- ROC AUC Score: 0.8179
- F1 Score: 0.7455

## Tools
- Pandas and Python to download, clean, and perform exploratory analysis.
- spaCy, Regex, NLTK, and TextBlob were used for preprocessing and tokenization
- sklearn and Gensim were used for modeling
- Matplotlib, Seaborn, ScatterText, and pyLDAvis were used for visualizations

## Visualization

![Unknown-3](https://user-images.githubusercontent.com/67508938/133799470-7efeac50-9f0d-414d-8b0d-e61febf33fe0.png)


![Unknown](https://user-images.githubusercontent.com/67508938/133799475-e0bf75d6-6861-46d1-ac31-21d1e07be134.png)

