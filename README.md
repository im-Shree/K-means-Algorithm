# Implement the K-means clustering algorithm on a synthetic data set

We will implement the standard k-means algorithm by iteratively updating the centroids and reassigning data points to the closest centroids until convergence.

### Data Pre-processing
  We use the X.dat file to read the data.
  We will read the file and write it inot an data frame to preprocess the data.
  Write the updated data frame into an CSV file
  The data types are stored as a Series object, which is a one-dimensional labeled array.
  We will create a dictionary which will map column names to desired data types.
  Then we will change data type to float for data in every column
  
### K-means function
  We will build the logic on which k-means algorithm runs. 
  We will feed our data from pre-processed dataframe. 
  Generate random value for centroid within range of our data. 
  Find euclidean distance between our centroids and data point and select the min distance.

  For each cluster index, it calculates the mean of the data points that are assigned to that cluster. 
  The calculated mean becomes the updated centroid for the corresponding cluster, and it is appended to the centroids list. 
  Stacks the updated centroid values vertically to form the final centroid array.

  Compute the Euclidean distance between each data point in X and the final centroids. 
  Assigns each data point to the closest centroid using the final centroid positions. 
  Finally, the function returns the updated centroid positions (centroids) and the assigned cluster indices for each data point (points).

### Visualize function
  Call this function by passing your data matrix X and the desired value of k. 
  It will perform the K-means clustering, visualize the data points in different colors based on their assigned clusters, 
  and plot the centroids as yellow-colored diamonds.
  
![k3](https://github.com/im-Shree/K-means-Algorithm/assets/90651908/dd20f61d-8a69-42e1-acfb-51122373da05)
![k4](https://github.com/im-Shree/K-means-Algorithm/assets/90651908/b75468c6-ae54-440d-a257-619185f37c8d)
![k5](https://github.com/im-Shree/K-means-Algorithm/assets/90651908/f36e260f-4d75-4bb5-b778-75feb6357e64)


