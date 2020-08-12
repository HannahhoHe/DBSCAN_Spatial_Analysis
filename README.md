# Data Wrangling Scripts

Written particularly to analyze types of cells after applying clustering algorithm (see [DBSCAN script](https://github.com/HannahhoHe/DataWrangling-ImageData-Clusters/blob/master/DBSCAN.ipynb)). 
To use the scripts, structure your datasets into columns of sample ID (or patient ID, slide ID), cell position X, cell position Y, and cell phenotype. Each row is one unique cell from the image. For clustering data, add an extra column of cluster ID that the cells are assigned to. For example, if there are 5 clusters, the cluster ID can be labelled as 1, 2, 3, 4, 5. For the neighborhood analysis, some of the following scripts can walk you through and prepare the format for the subsequent wrangling. 


See [the script](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/tree/master/DataCleaning) for data cleaning prior running the following scripts.
# Analyze the DBSCAN clusters
- [Types of clusters, cells comprising the clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/tree/master/Types%20of%20clusters)
- [Counting how many clusters (and types of) in each specimen](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cluster%20count.ipynb)
- [Calculating the cluster size (and types of) in each specimen](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cluster%20Size.ipynb). The cluster size is the total number of cells. 
- [Portion (percent) of cells found in clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Portion%20of%20cells%20found%20in%20the%20cluster.ipynb) 
  
# Delaunay triangulation algorithm
  - [Run the Delaunay algorithm, plot a representative figure](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Neighborhood%20(Delaunay).ipynb)
  
# Merge the DBSCAN clusters with Delaunay neighbors  
 - [The scripts](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Combine%20DBSCAN%20and%20Delaunay.ipynb) (1) merge the results from the Delaunay algorithm with that from the DBSCAN clustering, (2) plot graphs showing the number of neighbors (of different type of cells) for cells in DBSCAN cluster, (3) perform statistical analysis (p-value) testing the null hypothesis for cells having different numbers of neighbors when involving in types of clusters, (4) plot the number of neighbors (of different type of cells) against the size of heterotypic cluster and from which, (5) perform linear regression based off it.         

# Changes of functional markers 
- Cells participating DBSCAN clustering
  - [by Types of clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cells%20participating%20DBSCAN%20clustering.ipynb)
  - [by Numbers of neighbors](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cells%20participating%20DBSCAN%20clustering-Numbers%20of%20Neighbors.ipynb)
  - [by Size of clusters](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cells%20participating%20DBSCAN%20clustering-by%20heterocluster%20size.ipynb)
- Other cells within the clusters (also see registration for consecutive specimen sections)  
  - [Register two whole-slide cartesian data](https://github.com/HannahhoHe/DataWrangling-ImageData-Clusters/blob/master/WSI%20Registration.ipynb)
  - [Find if cells are within a cluster](https://github.com/HannahhoHe/DataWrangling-ImageData-Clusters/blob/master/Find_prolifCD8_withinCluster.ipynb)
  - [Calculate cell proliferation rate](https://github.com/HannahhoHe/DataWrangling-ImageData-Clusters/blob/master/Calculating%20CD8%20proliferation%20in%20different%20clusters.ipynb)
  


# Cox Regression Analysis
- [ROC curve, Cox Hazard Ratio, logrank, and Kaplan-Meier plots](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/blob/master/Cox%20survival%20regression.ipynb): feature engineering that converts features to classification by an optimal cutoff, determined by ROC curve, is included.
