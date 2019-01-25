# Code a K-means Algorithm from Scratch

The function will take the following arguments:

• myScatterInput: a data frame with n rows and m columns, where all entries will be real numbers

• myClusterNum: an integer value greater than or equal to 2 but less than or equal to n
– 2 < myClusterNum < n

The funciton will take the following steps:
1. Randomly assign each of the points in myScatterInput to some value between 1 and myClusterNum.
2. Compute the cluster centroid for each cluster 1 to myClusterNum.
3. Compute the Euclidean distance from each cluster centroid to each data point.
4. Assign each point to the cluster centroid which minimizes the Euclidean distance.
5. Repeat steps 2, 3 and 4 until one of two stopping conditions are met

   • subsequent cluster assignments are unchanged
   
   • have repeated steps 2, 3 and 4 maxIter number of times

6. Once reaching a terminating condition, compute the sum of all Euclidean distances from each
point to their respective centroids.
7. Repeat steps 1-6 100 times.
8. Identify the replication with the lowest sum of Euclidean distances from points to centroids as
best result and print the value to the console.
