---
title: Graph Analytics and Data Science
tags: [graphdb, cypher]
style: fill
color: secondary
description: Introduction to Graph Analytics and Data Science
---
## Why Graph Analytics and Data Science?

We are in the era of data abundance. Most of businesses try to find insights on their data for better decision making. Data lakes are **Silo Ponds** with Terra bytes of data but not connected. Find the patterns, trends, and anomalies from unrelated data is always a challenge. Graph Analytics and Data Science is a new way of looking at the data were **relationships** are first class citizens. 

![Silo Ponds](/assets/images/graph-data-analytics/silo-ponds.png)

## What is a Graph?
Graphs are mathematical structures consisting of nodes (vertices) connected by edges (links), and they are used to model and represent complex relationships and networks. 

### Basic Terminology
**Definitions**
A graph $G = (V, E)$ consists of two sets V and E.

The elements of V are called vertices (or nodes).
The elements of E are called edges (or relationship).

![vertex-edges](/assets/images/graph-data-analytics/vertex-edges.svg)

Each edge has a set of one or two vertices associated to it, which are called its endpoints. An edge is said to join its endpoints.
We can find graph structures in almost all the domains. Road, networks, telecom have good uses of Graphs.

## What is Graph Analytics and Algorithms?

Graph Analytics is the process of analyzing data stored in graph format. Graph Analytics is used to find patterns and insights from the data. Graph Analytics is a stream of analytics that uses algorithms to find the shortest path, find the most influential person in the network, find the communities in the network, fraud detection, social networks, supply chain, and many more.

### Shortest Path Algorithm
Shortest Path algorithm is used to find the shortest path between two nodes. This the foundation of the navigation systems like google maps. Network Routing, Transportation planning, Robotics and Automous Vehicles, Game development, Emergency Services, Circuit Design, Social Network Analysis, and Urban Planning are some of the other use cases.

#### Reference
[Shortest Path Algorithm](https://neo4j.com/docs/graph-algorithms/current/algorithms/shortest-path/)

### PageRank
PageRank algorithm is used to find the most influential nodes in the network. PageRank algorithm is used in search engines to find the most relevant pages for a given search term. The PageRank algorithm was developed by Larry Page and Sergey Brin, who are the co-founders of Google. They introduced PageRank in their research paper titled "The Anatomy of a Large-Scale Hypertextual Web Search Engine" in 1996 while they were Ph.D. students at Stanford University. PageRank was a fundamental component of the Google search engine, which they later developed. The algorithm was designed to rank web pages in search engine results based on their importance and relevance, as determined by the links and connections between web pages on the World Wide Web. 

#### Reference
[PageRank](https://en.wikipedia.org/wiki/PageRank)

### Community Detection
Community detection algorithms are computational techniques used to identify and analyze communities or groups of nodes within a network or graph. These algorithms help uncover hidden structures and patterns in complex networks, such as social networks, citation networks, and biological networks.
There are several community detection algorithms, each with its own approach and strengths. Here are some prominent community detection algorithms:

| Community Detection Algorithms | Description |
| --- | --- |
|Modularity-based Algorithms | aim  of these algorithms are to identify communities or groups of nodes within a network by optimizing a quality function called "modularity." Modularity measures the strength of division of a network into communities based on the density of connections within communities compared to the expected density if the network were randomly connected. In other words, it quantifies the extent to which a network is more clustered than what would be expected by chance. Newman-Girvan and Louvain are popular in this group.|
| Label Propagation | Label Propagation is a fast algorithm for detecting communities in networks. It is based on the observation that labels tend to converge to a consensus in networks consisting of multiple communities. |
| Hierarchical Clustering | Hierarchical clustering is a method of cluster analysis that builds a hierarchy of clusters. It is a bottom-up approach where each node starts in its own cluster, and pairs of clusters are merged as one moves up the hierarchy. |
| Graph Partitioning Algorithms | These algorithms are used for finding clusters in data. It is based on the idea that a graph can be partitioned into clusters by cutting edges between clusters and maximizing the number of edges between nodes in the same cluster. |
| Random Walk-based Algorithms | These algorithms analyze the patterns of node traversal. These algorithms are based on the idea that nodes within the same community are more likely to be visited successively during random walks than nodes in different communities. Random walk-based algorithms are particularly useful for uncovering communities in networks where nodes have strong local connections but weaker global connections. |
| Density based Algorithms | These algorithms are based on the idea that communities are dense subgraphs. group data points into clusters based on their proximity and density in the feature space. Unlike some other clustering algorithms (e.g., k-means or hierarchical clustering), density-based algorithms do not require specifying the number of clusters in advance. Instead, they identify clusters as regions of high data point density separated by areas of lower density. One of the most well-known density-based clustering algorithms is DBSCAN (Density-Based Spatial Clustering of Applications with Noise). These algorithms are particularly useful for uncovering communities in networks where nodes have strong local connections but weaker global connections.  |

#### Reference
[Comparative Analysis of Community Detection Algorithms](https://www.analyticsvidhya.com/blog/2022/08/a-comparative-analysis-of-community-detection-algorithms/)

[A Comparative Analysis of Community Detection Algorithms on Artificial Networks](https://www.nature.com/articles/srep30750)

### Similarity
A similarity graph algorithm is a method used to construct a graph where nodes represent data points, and edges represent the pairwise similarities or dissimilarities between these data points. These algorithms are commonly used in various data analysis and machine learning tasks, including clustering, dimensionality reduction, and data visualization. The primary goal of constructing a similarity graph is to capture the underlying structure or relationships in the data based on the notion of similarity or distance. Similarity graph algorithms are also known as similarity network algorithms, similarity-based algorithms, or distance-based algorithms.

Document clustering in NLP is the most common use case for similarity graph algorithms. In this case, each document is represented as a vector in a high-dimensional feature space, and the similarity between two documents is measured by the cosine similarity between their corresponding vectors. The similarity graph is constructed by connecting documents whose cosine similarity exceeds a specified threshold. The resulting graph can then be used for clustering, dimensionality reduction, or visualization.

#### Reference
[Algorithms for Graph Similarity and Subgraph Matching](https://www.stat.cmu.edu/~aramdas/reports/DBreport.pdf)


## Centrality
Centrality algorithm is used to find the most important nodes in the network. These algorithms help to reveal which nodes in a network are the most influential, central, or critical based on various criteria. Centrality measures are commonly applied in fields such as social network analysis, transportation, biology, and information retrieval. 

| Centrality Detection Algorithms | Description |
| --- | --- |
| Degree Centrality |Degree centrality is the simplest centrality measure and is based on the number of connections a node has. Nodes with a high degree centrality are considered central because they are directly connected to many other nodes.|
| Closeness Centrality | Closeness centrality is based on the idea that nodes that are close to other nodes can access information or resources more quickly and efficiently. Nodes with a high closeness centrality are considered central because they are close to many other nodes.|
| Betweenness Centrality | Betweenness centrality is based on the idea that nodes that lie on many shortest paths between other nodes are important because they control the flow of information or resources between other nodes. Nodes with a high betweenness centrality are considered central because they lie on many shortest paths between other nodes.|
| Eignvector Centrality | Eigenvector centrality is based on the idea that connections to high-scoring nodes contribute more to the score of the node in question than equal connections to low-scoring nodes. Nodes with a high eigenvector centrality are considered central because they are connected to many other nodes that are themselves central.|
| Harmonic Centrality | Harmonic centrality is based on the idea that nodes that are close to many other nodes are important because they can access information or resources from many other nodes. Nodes with a high harmonic centrality are considered central because they are close to many other nodes.|
| Katz Centrality | Katz centrality is based on the idea that connections to high-scoring nodes contribute more to the score of the node in question than equal connections to low-scoring nodes. Nodes with a high Katz centrality are considered central because they are connected to many other nodes that are themselves central.|

#### Reference
[Centrality Algorithms](https://neo4j.com/docs/graph-algorithms/current/algorithms/centrality/)


## Flow Analysis
Flow Analysis algorithms are used to find the flow of information in the network. These algorithms help to reveal how information or resources flow through a network. Flow analysis algorithms are commonly applied in fields such as social network analysis, transportation, biology, and information retrieval.

| Flow Analysis Algorithms | Description |
| --- | --- |
|Max Flow - Min Cut Algorithm| The Max Flow - Min Cut algorithm is used to find the maximum flow from a source node to a sink node in a network. The maximum flow is the maximum amount of flow that can be sent from the source node to the sink node. The minimum cut is the minimum amount of flow that must be removed from the network to disconnect the source node from the sink node.|
|Ford-Fulkerson Algorithms | The Ford-Fulkerson algorithm is used to find the maximum flow from a source node to a sink node in a network. The maximum flow is the maximum amount of flow that can be sent from the source node to the sink node.|
|Edmonds-Karp Algorithm | The Edmonds-Karp algorithm is used to find the maximum flow from a source node to a sink node in a network. The maximum flow is the maximum amount of flow that can be sent from the source node to the sink node.|
|Dinic's Algorithm| Dinic’s algorithm is used to solve maximum flow problems. Maximum flow problems can be described as trying to find an attainable “flow” through a single source, single-sink flow network that is also a max. |





