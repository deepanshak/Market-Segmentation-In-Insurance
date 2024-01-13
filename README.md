# Market-Segmentation-In-Insurance
## Project Overview
This case  study makes use of machine learning algorithms to develop a market segmentation to give recommendations like saving plans, loans, wealth management, etc. on target customer groups. 

- [Introduction](#Intoduction)
- [Data Description](#Data-Description)
- [Methodology](#Methodology)
    - [Data Cleaning](#Data-Cleaning)
    - [EDA](#Exploratory-Data-Analysis)
    - [Model Building](#Model-Building )
 - [Conclusion and Key Insights](#Conclusions-And-Key-Insights) 


## Intoduction
In this case study, exploratory data analysis was carried out along with using machine learning algorithms a market segmentation was created where we are taking the customer details & identifying which cluster the customer belongs to and provide suggestions for target consumer groups regarding loans, savings plans, wealth management, and other related services. 

## Data Description
The sample Dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.
Data  set can be accessed from[ here]()
## Methodology
### Data Cleaning
- Checking for null and duplicate values.
- Filling mean values inplace of missing values.
- dropping unnecessary variables.
### Exploratory Data Analysis 
For complete analysis refer to file:
-  Checking for descriptive statistics.
-  Creating a set of Kernel Density Estimation (KDE) plots for numerical variables.
-  Creating a set of distribution plots for each numerical variable in a DataFrame. 

### Model Building 
#### Data Prepration
- scaling the data frame.
- Dimensionality reduction.
- Hyperparameter tuning
  
#### Algorithms Used:
In this dataset i've used five clustering algorithm to perform segmentation.These algorithms are given below.
- [K-Means Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- [Agglomerative Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
- [Spectral Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.SpectralClustering.html)
- [DBSCAN Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html)
- [GaussianMixture Model based clustering](https://scikit-learn.org/stable/modules/mixture.html)
- [Decision Tree Classifire]()
#### Steps Taken
- Model building using K means.
- Visualizing the clustered data frame.
- Creating a target column "Cluster" for storing the cluster segment.
- Visualizing the cluster count.
- Histogram grid subplots for different variables corresponding to different clusters.
- Training and testing model with Decision tree.
#### Saving the model 
 Saving the kmeans clustering model and the data with cluster label.

