# Market-Segmentation-In-Insurance
![market segment](https://github.com/deepanshak/Market-Segmentation-In-Insurance/assets/139687677/bbbe1503-e243-4e59-8c7f-dcb5ce745146)


## Project Overview
This case  study makes use of machine learning algorithms to develop a market segmentation to give recommendations like saving plans, loans, wealth management, etc. on target customer groups. 

- [Introduction](#Intoduction)
- [Data Description](#Data-Description)
- [Methodology](#Methodology)
    - [Data Cleaning](#Data-Cleaning)
    - [EDA](#Exploratory-Data-Analysis)
    - [Model Building](#Model-Building )
 


## Intoduction
In this case study, exploratory data analysis was carried out along with using machine learning algorithms a market segmentation was created where we are taking the customer details & identifying which cluster the customer belongs to and provide suggestions for target consumer groups regarding loans, savings plans, wealth management, and other related services. 

## Data Description
The sample Dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.
Data  set can be accessed from[ here](https://github.com/deepanshak/Market-Segmentation-In-Insurance/blob/main/Customer%20Data.csv)
## Methodology
### Data Cleaning
- Checking for null and duplicate values.
- Filling mean values inplace of missing values.
- dropping unnecessary variables.
### Exploratory Data Analysis 
For complete analysis refer to [file](https://github.com/deepanshak/Market-Segmentation-In-Insurance/blob/main/Market_Segmentation_Customer.ipynb)
-  Checking for descriptive statistics.
-  Creating a set of Kernel Density Estimation (KDE) plots for numerical variables.
-  Creating a set of distribution plots for each numerical variable in a DataFrame. 
- Heat map depicting correlation between different variables.
![heatmap ms](https://github.com/deepanshak/Market-Segmentation-In-Insurance/assets/139687677/f13fdb39-3339-4d71-802b-aa98909cda59)

  
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
- [Decision Tree Classifire](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
#### Steps Taken
- Model building using K means.
  
- Visualizing the clustered data frame.
  
   ![clustring using k means](https://github.com/deepanshak/Market-Segmentation-In-Insurance/assets/139687677/aba95cc4-3e5a-43e3-ac64-83ff48207187)

-  Creating a target column "Cluster" for storing the cluster segment.
  
- Visualizing the cluster count.
  
  ![count cluster](https://github.com/deepanshak/Market-Segmentation-In-Insurance/assets/139687677/41b380ff-d5b7-46ac-bd33-f7d0107fca10)

- Histogram grid subplots for different variables corresponding to different clusters.
  
  ![grid plot with all variables](https://github.com/deepanshak/Market-Segmentation-In-Insurance/assets/139687677/85445c8d-1ab5-48c2-b173-0fc1c54df821)

- Training and testing model with Decision tree.
#### Saving the model 
 Saving the kmeans clustering model and the data with cluster label.

