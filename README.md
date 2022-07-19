# Document_Clustering

## Introduction:

Document clustering (or text clustering) is the application of cluster analysis to textual documents. In this project, the documents are clustered using a gensim Word2Vec model and the MiniBatchKmeans algorithm.

## Data:
The data used comes from the Janatahack NLP hackathon. Originally the competition was about a supervised learning classification problem, however, in this project, the same data is used for an unsupervised learning problem.

## Requirements:

```pandas:``` Data analysis and manipulation tool.

```matplotlib:``` Visualization library.

```seaborn:``` Data visualization library based on matplotlib, it enhances the style of matplotlib plots.

```Numpy:``` Numerical analysis library.

```scikit-learn:``` Machine Learning library.

```NLTK:``` The Natural Language Toolkit is a suite of libraries and programs for symbolic and statistical natural language processing (NLP).

```string:``` Common string operations module.

```re:``` This module provides regular expression matching operations.

```gensim:``` Open-source library for unsupervised topic modelling, document indexing, retrieval by similarity, and other natural language processing functionalities, using modern statistical machine learning. 

## First part:

Cleaning data: Common preprocessing steps as removing punctuation marks and non-alphanumeric characters,  tokenization or lemmatization.

After the cleaning process, a gensim Word2Vec model is trained with the tokenized documents to create the word vectors.

Once the Word2Vec model is created, document vectors are generated using the average of the word vectors.

## Second part:

An unsupervised clustering algorithm is applied to the document vectors. In this case, MiniBatchKmeans has been chosen to reduce the computational cost.

The clusters’ quality is measured using metrics like Inertia and the Silhouette Coefficient. It’s also verified by looking for the most representative words and documents per cluster, i.e. the word vectors and document vectors closest to the clusters’ centroids.

Finally, each document label is compared to the target variable to evaluate the model’s performance.  
