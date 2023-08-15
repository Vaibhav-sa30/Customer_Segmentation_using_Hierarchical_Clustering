# Customer Segmentation using Hierarchical Clustering

A small scale project which largely focuses on Documentation and Exploratory Data Analysis. 

## Project Description
Hierarchical Cluster Analysis Capstone Project is an integral part of 4 years Data Science with Python program from Coincent.ai
This is an independent Exploratory Data Analysis(EDA) project. 

## Project Thoery

In machine learning, there are numerous algorithms that can be used to model data depending on various use cases, most of which fall under 3 categories: Supervised Learning, Unsupervised Learning and Reinforcement Learning. 
Clustering comes under **Unsupervised Learning**.


### What is Clustering?

As of general English meaning, Clustering is a group of similar things growing or held together, or a group of people or things that are close together.
And that’s really all that is in Machine Learning too. It is grouping of unlabeled data. Clustering is a machine learning ‘technique’ that groups the data we provide such that, datapoints within a cluster are more similar to each other (or we can say homogeneous) than the datapoints from other clusters. That is, datapoints from different clusters should be as dissimilar as possible.
We do clustering to understand the underlying structure in the data that may not be detectable at first sight.  


### Types of Clustering Technique

Clustering are basically of two types: **Flat Clustering** and **Hierarchical Clustering**

- Flat Clustering: In flat clustering, the data is partitioned into a fixed number of non-overlapping clusters. Each data point belongs to exactly one cluster. Flat clustering algorithms typically require the user to specify the number of clusters in advance. Examples of flat clustering algorithms include K-Means, K-Medoids, and Fuzzy C-Means. 

- Hierarchical Clustering: This type of clustering creates a hierarchical decomposition of the dataset. The two main types of hierarchical clustering are agglomerative (bottom-up) and divisive (top-down). Agglomerative clustering starts with each data point as a separate cluster and iteratively merges the most similar clusters until a single cluster is formed. Divisive clustering starts with the entire dataset as a single cluster and recursively divides it into smaller clusters until each data point is in its own cluster.

Our focus with this project is on Hierarchical Clustering so let's understand it a bit more deeply.


### Hierarchical Clustering

As the name suggests, in Hierarchical Cluster there is some sort of hierarchy maintained in the decomposition of the dataset into clusters. This hierarchical decomposition is what gives Hierarchical Clustering an edge over other clustering techniques. Because in hierarchical clustering we not just get clusters of the data, we also get extra information as in what order the algorithm formed those clusters. This extra information can be helpful in determining some relation between groups within data. That is, we get to know which group is a closer cluster to which group and what is the next closer cluster. Hierarchical Clustering shows all the possible linkages between different clusters.

### Types of Hierarchical Clustering

The two main types of hierarchical clustering are agglomerative (bottom-up) and divisive (top-down). 

#### Divisive Clustering

Divisive clustering starts with the entire dataset as a single cluster and recursively divides it into smaller clusters until each data point is in its own cluster. 

Divisive clustering is a "greedy" algorithm, as it makes a locally optimal choice at each step by dividing the cluster that has the largest dissimilarity among its data points. This can lead to a suboptimal clustering, as it may not consider the global structure of the data.
Despite its potential limitations, divisive clustering is a useful technique for exploring the structure of high-dimensional datasets and identifying clusters that can help in tasks such as pattern recognition and anomaly detection.

#### Agglomerative Clustering

This bottom up algorithm treat each datapoint as a single cluster at the initial step and then successively merge (or agglomerate) pairs of clusters until all clusters have been merged into a single cluster that contains all datapoints.Bottom up hierarchical clustering is therefore called  Hierarchical Agglomerative Clustering or HAC.

HAC is more frequently used in information retrieval than top-down clustering and is the main subject of this project.
The question now here is, How do we visualize this hierarchical decomposition of data into clusters? ---> This is where...

#### Dendrograms

comes into picture. Dendrogram is a tree-like diagram which records the sequences of merges or splits happen as the algorithm runs. By moving up from the bottom layer to the top node, a dendrogram allows us to reconstruct the history of merges that resulted in the depicted clustering.
In a dendrogram, the vertical axis represents the distance or dissimilarity between the objects being clustered, and the horizontal axis shows the objects themselves or the groups of objects at each level of the hierarchy. As you move down the dendrogram, the branches represent the groups of objects that are more and more similar to each other. The height of each branch in the dendrogram represents the distance or dissimilarity between the groups of objects being joined together. 

...[continue reading](https://vaibhavsatish.substack.com/p/learn-and-implement-hierarchical?justPublished=true&embeddedPostPublications=&autoSharedOnTwitter=true)

