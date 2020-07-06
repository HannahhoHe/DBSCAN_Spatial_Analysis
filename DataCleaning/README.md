# What is the script for?
- There are 50-60 files of images from different specimens, all with DBSCAN cluster ID appended (after DBSCAN clustering). The script is to uniform the column names and the phenotype names, originally labelled with various forms.
- In addition, there are two steps of assigning cluster ID to the cells. In the first step, we performed the DBSCAN clustering based on a subset of cell types (of our interest), with which the results were shown in the column called "DBSCAN Cluster". In the second step, we followed the cells at the resultant cluster periphery, and we further assigned the cluster ID to the rest of cells which are not participating in the first clustering. In the latter step, columns with the name of "Belong to DBSCAN0" are used. Some cells can belong to more than one unique cluster due to the cluster overlap. In such case, an additional column named "Belong to DBSCAN1"... are generated. 


