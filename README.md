# Data Wrangling Scripts

Written particularly to analyze types of cells after applying clustering algorithm or Delaunay triangulation algorithm (neighborhood). 
To use the scripts, structure your datasets into columns of sample ID (or patient ID, slide ID), cell position X, cell position Y, and cell phenotype. Each row is one unique cell from the image. For clustering data, add an extra column of cluster ID that the cells are assigned to. For example, if there are 5 clusters, the cluster ID can be labelled as 1, 2, 3, 4, 5. For the neighborhood analysis, some of the following scripts can walk you through and prepare the format for the subsequent wrangling. 


See [the script](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/tree/master/DataCleaning) for data cleaning prior running the following scripts.
### Analyze the DBSCAN clusters
- [Types of clusters, cells comprising the clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/tree/master/Types%20of%20clusters)
- [Counting how many clusters (and types of) in each specimen](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cluster%20count.ipynb)
- [Calculating the cluster size (and types of) in each specimen](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cluster%20Size.ipynb). The cluster size is the total number of cells. 
- [Portion (percent) of cells found in clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Portion%20of%20cells%20found%20in%20the%20cluster.ipynb) 
  
### Delaunay triangulation algorithm
  - [Run the Delaunay algorithm, plot a representative figure](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Neighborhood%20(Delaunay).ipynb)
  
### Combine the outputs from DBSCAN cluster and Delaunay algorithm  
 - [This script](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Combine%20DBSCAN%20and%20Delaunay.ipynb) first merge the results from the Delaunay algorithm with that from the DBSCAN clustering, plot the graph showing the number of neighbors (of different type of cells) for cells in differnt type of DBSCAN cluster, perform the statistical analysis (p-value) testing the null hypothesis for cells having different number of cells (of different type of cells), plot the size of heterotypic cluster against the number of neighbors (of different type of cells) and perform linear regression based off it.         
