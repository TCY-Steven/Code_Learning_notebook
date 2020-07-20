# Machine Learning with Python
## Classification algorithms in Machine learing

1. Decision tree
2. Naive Bayes
3. Linear discriminat analysis
4. k-nearst neighbor
5. Logistic regression
6. Neural network
7. Support vector machines (SVM)

## Acurracy measurement

1. Jaccard index
2. F1-score
    Precision = TP/(TP+FP)
    Recall = TP/(TP+FN)
    F1-score = 2*(prc * rec)/(prc+rec)
3. Log loss

## Machine Learning Algorithms
### K-Nearst Neighbor
**Data Normalization**
X = preprocessing.StandardScaler().fit(X).transform(X.astype(float))

### Decision Tree
Calculation the entropy as criteria of each feature categories
Evaluation the accuracy by sklearn metrics.accuracy_score

### Logistic Regression
**Suitable condition**
1. Data is binary
2. Need probabilistic result
3. Need a linear decision boundary 
4. Need to understand the impact of a feature

**Training process**
1. initialize the parameters randomly $\theta$
2. Calculate $\hat{y}$ = $\sigma$($\theta^T$X)
3. Feed the cost function with training set and calculate error
4. Calculate the gradient of cost function (**Gradient descent**)
5. Update weight with new values
6. Go to step 2 until cost is small enough
7. Predict the new customer X

### Support Vector Machine (SVM)
SVM is a supervised algorithm that classifies case by finding a separator.
Mapping data to high-dimensional feature space, and finding a separator.

Advantage :
* Accurate in high-dimentional space
* Memory efficient

Disadvantage : 
* Prone to over-fitting
* No probability estimation
* Small dataset

### k-Mean Clustering
Med and large size database (relativly efficient)
Produces sphere-like clusters
Need number of clusters(k)

### Hierarchical clustering
Agglomerative algorithm
1. Create n clusters, one of each data point
2. Compute the proximity Matrix
3. Repeat 
    * Merge the two closet clusters
    * Update the proximity matrix
4. Until only a single cluster remains

Distance between clusters
1. Single-Linkage clustering (minimum)
2. Complete-Linkage clustering (maximum)
3. Average Linkage clustering 
4. Centroid Linkage clustering 

### Density-Based Spatial Clustering of Applications with Noise
