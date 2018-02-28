# Quora Question Pairs 
Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question.

In this project, we apply sequence model to identify pairs of sentences which have same semantic meaning. This is part of the [competition](https://www.kaggle.com/c/quora-question-pairs) posted on Kaggle by Quora. We have used pre-trained GloVe word embeddings to encode word-vectors into a 300 dimensional space. An LSTM layer is further used to encode the semantics of sequence of words into a 50 dimensional space. Manhattan distance is used to define the similarity in semantics between two vectors.

## Requirements
This project requires **python3** and following libraries are specifically needed.

1. NumPy
2. Pandas
3. Keras

## Data
We have used GloVe word embeddings which can be downloaded [here](http://nlp.stanford.edu/data/glove.42B.300d.zip). 
Quora has provided pairs of questions with labels (1 if they have same meaning, 0 otherwise) provided by human experts for training purpose.


