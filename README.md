# topic_modeling





Topic Modelling:
Topic Modeling is an unsupervised learning approach to clustering documents, to discover topics based on their contents. 
It is very similar to how K-Means algorithm and Expectation-Maximization work. 
Because we are clustering documents, we will have to process individual words in each document to discover topics, 
and assign values to each based on the distribution of these words. This increases the amount of data we are working with, 
so to handle the large amount of processing required for clustering documents, we will have to utilize efficient sparse data structures.
I (Rehan) will implement two different approaches for topic modeling, and compare their results. These approaches are LDA (Latent Derilicht Analysis), 
and NMF (Non-negative Matrix factorization).

Latent Derilicht Analysis (LDA)
LDA, or Latent Derelicht Analysis is a probabilistic model, and to obtain cluster assignments, it uses two probability values: P( word | topics) and P( topics | documents). 
These values are calculated based on an initial random assignment, after which they are repeated for each word in each document, to decide their topic assignment. 
In an iterative procedure, these probabilities are calculated multiple times, until the convergence of the algorithm. LDA is good in identifying coherent topics:

