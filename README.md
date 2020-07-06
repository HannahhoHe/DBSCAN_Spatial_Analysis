# Data Wrangling Scripts

Written particularly to analyze types of cells after applying clustering algorithm or Delaunay triangulation algorithm (neighborhood). 
To use the scripts, structure your datasets into columns of sample ID (or patient ID, slide ID), cell position X, cell position Y, and cell phenotype. Each row is one unique cell from the image. For clustering data, add an extra column of cluster ID that the cells are assigned to. For example, if there are 5 clusters, the cluster ID can be labelled as 1, 2, 3, 4, 5. For the neighborhood analysis, some of the following scripts can walk you through and prepare the format for the subsequent wrangling. 


[See the script](https://github.com/HannahhoHe/Data-Wrangling-Multidimensional-Image-Data/tree/master/DataCleaning)for data cleaning.
### Group cells by DBSCAN clustering
- Cells comprising the clusters 
- Percent of cells found in the clusters
  
### Delaunay triangulation algorithm
  - Apply the algorithm 
  - Add and append the results 
  
### Combining the results from DBSCAN clustering and Delaunay triangulation algorithm 
### Manually register two images and assign cluster ID to the cells in the new image slide  
