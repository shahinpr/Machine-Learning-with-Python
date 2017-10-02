# The Nearest Neighbor Classifier
### Description
* kNN is one of the simplest Machine Learning algorithms. 
* By nature it falls in the supervised family of algorithms. 
* Mostly used for classification, also can be used for regression tasks.  
  **Regression :** Value of test example calculated by (weighted) avarage of k nearest test points  
  **Calssification :** Majority vote of k closest training points used to determine class
* It is a non-parametric and instance-based (lazy) learning algorithm.  
  **Non-parametric** means no explicit assumptions on data distibution   
  **Instance-based** learning means training data is not used for generalization. 
* Often used as a benchmark for more complex classifiers such as Artificial Neural Networks (ANN) and Support Vector Machines (SVM)
* kNN doesn't explicitly compute decision boundaries. The boundaries between distinct classes form a subset of the Voronoi diagram of the training data.   
* Different distance metrics can be used to determine k neirest neigbors (Euclidean,Manhattan,Minkowski etc)
* Works with – Numeric values, nominal values


### Pros & Cons
* **Pros**
 * Very easy to understand and implement
 * Can quickly respond to changes in input
 * Does not assume any probability distributions on the input data
 * Naturally handles multi-class cases
 * Can do well in practice with enough representative data
* **Cons**
 * kNN can suffer from skewed class distributions
 * High dimentional data can cause problems when finding nearest points 
 * Large search problem to find nearest neighbours  
 * Affected by local structure
 * Sensitive to noise, irrelevant features 
 * Must know we have a meaningful distance function
 * Storage of data

### Improvements
* The distance measure has to be meaningful – attributes should be scaled.
* Changing the distance metric for different applications may help improve the accuracy of the algorithm
* Dimensionality reduction techniques like PCA should be executed prior to appplying KNN and help make the distance metric more meaningful.
* A good value for K can be determined by considering a range of K values.
* Use a distance-based voting scheme, where closer neighbors have more influence.
* Pre-sort training examples into fast data structures (Approximate Nearest Neighbor,locality sensitive hashing (LHS))
* Remove redundant data
* Address missing Data
