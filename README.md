# Sentence-Pairs-Classification

Human language is a complex form of communication and understanding natural language with computers can become extremely challenging. The field of Natural Language Understanding (NLU) focuses on unfolding all the aspects of language, so we can develop machines capable to represent and process textual data. In this project, we test three Natural Language Processing (NLP) models that are assume to provide good results for representing textual data, such as: tf-idf, GloVe and BERT. 

The data that is has been used is the Stanford Natural Language Inference (SNLI) corpus, a widely known dataset about sentence pairs and their label. For every pair of sentences, the table guesses their correspondent entailment label (e.g., 'entailment', 'neutral' or 'contradiction'). Due to computer performance limits, we need to take a subset of this large dataset, where the final shape becomes: (1000, 3) for training and (2500, 3) for testing. The source to download the SNLI corpus, is the following:

<https://nlp.stanford.edu/projects/snli/>

## TF-IDF

Tf-idf is a type of Vector Space Model (VSM) that is extremely good for performing tasks related to information retrieval. It is able to extract the topic of a document or a sentence and it is based on the word frequency in each document. However, it tends to output sparce vectors with a large number of zero values. Also, it is not able to recognize synonims or other lexical semantics from a text. 

## GloVe

Word embeddings such as GloVe are popular in any kind of NLP application. This particular embedding was made by the Stanford University and it has a large lexicon, where every word has their pre-trained embedding. The GloVe package contains multiple sizes of those vector embeddings, but in this project we will focus only on the biggest one (300 dimensions). Then main advantage of using word embeddings is that they have some knowledge about the language, they perform well on finding the lexical semantics of a text. Yet, the main drawback is that we need to handle out of vocabulary words.   

## BERT

Artificial neural networks have become a huge step for the analysis of big data. BERT is relatively new and it already provides with state-of-the-art benchmark results in various downstream tasks (e.g., question answering, sentence classification and sentiment analysis). For this project we will test how well it performs, compared to the two previous models. Even though extracts most of the semamntics of a sentence, it is highly expensive to train, hence we need to make use of a GPU to run its code.  
