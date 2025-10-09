Example: Alexa, Sentiment Analysis, Notebook LLM, Spam Filters


Basic terms used in NLP preprocessing - AI part to understand human language

Segnmentation - A paragraph into sentences by the . Or ; etc.
Tokenising - splitting each word in segmentation
Lowercasing - Unify text
Stop words - like is are "am, the, are" called Stop words 
Stemming - We need to teach "skiping skips skipped are" same this is called or part of same word SKIP
Lemmatization - Am are Is - Be s the lemma
Speech Tagging  - What is noun verb preposition
Pop Culture references - Named Entity Tagging  

Then ML algo is used - Ex Naive Bayes

Challenges in NLP
Ambiguity : bank = mone or river bank 
Slang :
Context: I saw her duck - bird or actio
Sarcasm: "Oh great"
Kanguage structure differences 
Messy text

EVOLUTION ON NLP:
1. RuleBased(1950-1980) Hand Coded rules ELIZA
2.Statistical (1990-2010) - Learn patterns from data(HMM, Naive Vayes)
3. Neural and Transformers (2015-present)
Context aware, near human - BERT, GRP

every pipeline stage solves real challenges.
Understanding workflow = easier debugging 

The NLP Assembly Line
Data Collection 
Preprocessiong
Feature Extraction
Model Training 
Evaluation
Deployment

Ex: Spam Detection

Feature Extraction 
1. Bag of Words
2. TF-IDF
3. Embedding 

Bag of words - word counts - how many times each words appear
TF-IDF - scale of importance
Term frequency Inverse Document Frequency 
It helps in assigning values 

Embeding

WHAT ARE THE SOME MODELS
1. naive bayes - simple fast
2. Logistic regression - binary classification
3. random Forests /Boosted Trees - structured features
4 Deep Learning - LSTM, Transformer for complex tasks

EVALUATION
Measure Performance
1. Accuracy -- Correct predictions %
2. Precision -- Spam flagged correctly
3. Recall -- Spam captured out of all spam
4. F1Score - Balance of precision and recall.

Deployment
1. Integrate into applicatiob
2. Classify new input in real time data 

==================================================

How do you normalise the data
punkt:
punkt is a pretrained model included in NLTK used for tokenization.
NLTK (Natural Language Toolkit)

import nltk 
nltk.download('punkt')
from nlkt.tokenize import word_tokenize
text = "Natural Language Processing is fun!"
tokens = word_tkenize(text)
print(tokens)
#output - ['Natural','','']


===============
Library	Type of Tokenization	Speed	Best for
NLTK	Rule-based & pre-trained	Slow	Learning, simple tasks
SpaCy	Rule + statistical	Fast	Production NLP pipelines
Hugging Face	Subword (BPE, WordPiece)	Very fast	Transformer models, deep learning
Gensim	Simple word tokenization	Fast	Word embeddings, topic modeling
TextBlob	Rule-based (NLTK)	Moderate	Beginner-friendly NLP tasks
===============

Lowecasing is important 
from nklt.corpus import stopwords  -- Helps to remove the words.

For feature extraction can be used as a part of sklearn
=============
NLP in security --
