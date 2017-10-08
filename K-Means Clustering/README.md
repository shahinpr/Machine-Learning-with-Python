# K-Means Clustering     
**Description**
* K-means clustering is a method of vector quantization, which is popular for cluster analysis.  
* K-Means method is numerical, unsupervised, non-deterministic and iterative.  
* The algorithm works iteratively to assign each data point to one of K groups  
* The choice of initial partition can greatly affect the final clusters  
* With fewer samples of data, inaccurate clustering can occur.  
* K-means and KNN are different algorithms. But result of K-Means can be valuable for classification using KNN  
* The results of the K-means clustering algorithm are:  
  1. The centroids of the K clusters, which can be used to label new data
  2. Labels for the training data

**Algorithm**
1. Pick a number k of random cluster centers
2. Assign every item to its nearest cluster center using a distance metric
3. Move each cluster center to the mean of its assigned items
4. Repeat 2-3 until convergence 

**Methods for selecting K value**  
- Elbow Method  
- Information Criterion Approach  
- Silhouette method  
- Jump method  
- Gap statistic  

**Assumptions**  
- Balanced cluster size within the datasets  
- Clusters are spherical  
- Clusters have similar density  

**Pros & Cons**  
* Pros:  
  - Practically work well even some assumptions are broken  
  - Simple and easy to implement  
  - Fast and efficient in terms of computitional cost  
  - K-means becomes a great solution for pre-clustering  
* Cons:
  - Sensitive to outliers
  - Sesitive to initial points and local optimal
  - K value is not known
  - Doesn't work well when clusters are not spherical 
  - Doesn't work well when clusters have different density
  - We never know which variable contributes more to the clustering process


**Improvements**  
- Include as many samples of data as possible
- Use median instead of mean for minimizing effect of outliers
- Use dimension reduction techniques to get data with fewer features
- Choose better method for initialization of the centroids
- Apply feature scaling/normalization