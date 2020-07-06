# Description of scripts

Data Wrangling scripts: written particularly to analyze types of cells after applying clustering algorithm or neighborhood, Delaunay triangulation. 
To use the scripts, structure your datasets into columns of sample ID (or patient ID, slide ID), cell position X, cell position Y, and cell phenotype. Each row is one unique cell from the image. For clustering data, add an extra column of cluster ID that the cells are assigned to. For example, if there are 5 clusters, the cluster ID can be labelled as 1, 2, 3, 4, 5. For neighborhood analysis, some of the following scripts can walk you through and prepare the format for the subsequent wrangling. 

