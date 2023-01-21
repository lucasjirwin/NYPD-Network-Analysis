Research project completed as part of my Machine Learning coursework at Princeton. 

<b>NYC_Network_Analysis.pdf</b> contains the LateX file outlining the project goals and outcomes. 

<b> COS424_HW3.ipynb </b>  contains the code used to perform network analysis. First, we read in the data as csv files using Pandas. We then create a custom data set by dropping all rows apart from the names of the officers and the complaint IDs. We then drop all N/A rows. By importing the networkx library, we create an empty undirected graph. We then create a graph with officers as nodes and add an edge between every officer who is involved in the same complaint, resulting in a graph of 35760 nodes and 71425 edges. 

Having created the graph, we run several centrality measures on the graph (Degree, Eigenvector and Pagerank). For each centrality measure, we sort the officers (nodes) by centrality and plot subgraphs of the officers with highest scores. We were particularly impressed to see that the use of Eigenvector centrality allowed us to identify 15% of the complaints by isolating 10% of the officers with the highest Eigenvector Centrality score. This proved the use of centrality measures in identifying particularly abusive officers. 

To extend our results, we also studied the connectivity of specific officers accused of certain allegations (e.g those classified as "punch/kick", "black", "hispanic" etc). 

<b> Pagerank.png </b>, <b>Degree.png </b> and <b> Eigenvector.png </b> contain images of the graphs of the 100 officers sorted by highest pagerank, degree and eigenvector centrality scores respectively. 
