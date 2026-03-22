### PROJECT: Customer Segmentation using Clustering



#### OVERVIEW:



This project focuses on analyzing customer purchasing behavior and grouping customers into distinct segments using clustering techniques. The goal is to help businesses better understand their customers and improve marketing strategies, services, and overall decision-making.



#### 

#### PROBLEM STATEMENT:



A XYZ company has provided a dataset containing customer demographics, purchasing behavior, and interaction data.



The objective is to:	



* Identify meaningful patterns in customer behavior
* Segment customers into distinct groups using clustering algorithms
* Provide actionable business insights for targeted marketing and customer retention



#### 

#### DATASET INFO:



The dataset contains information about customers, including:



**Customer Information**

* ID: Unique customer identifier
* Year\_Birth: Birth year
* Education: Education level
* Marital\_Status: Marital status
* Income: Yearly household income



**Household Information**

* Kidhome: Number of children
* Teenhome: Number of teenagers
* Customer Activity
* Dt\_Customer: Date of enrollment
* Recency: Days since last purchase



**Spending Behavior**

&#x09;MntWines, MntFruits, MntMeatProducts, etc.



**Purchase Behavior**

&#x09;NumDealsPurchases, NumWebPurchases, etc.





### Exploratory Data Analysis (EDA)



##### Numerical Features:

* Income is right-skewed with outliers
* Year\_Birth shows some unrealistic values (outliers)
* Spending features are heavily skewed
* Recency follows a roughly normal distribution



##### Categorical Features:

* Most customers are Graduates
* Majority are Married
* Very few belong to rare categories like YOLO or Absurd



#### DATA PREPROCCESSING:



* Handled missing values with median due to data skewness 
* Removing outliers by IQR limits
* Feature engineering

  * Created new features such as- Age, Year, AvgMnt, Total\_purchase 
* Encoding categorical variables
* Feature scaling by StandardScaler



#### CLUSTERING TECHNIQUES USED:



* K-Means Clustering
* Agglomerative (Hierarchical) Clustering
* DBSCAN







#### MODEL EVALUATION:



Clustering performance was evaluated using:



* **Silhouette Score**
* **Visual cluster separation (plots)**





#### MODEL SELECTION:

K- MEANS performed the best with silhouette score of 0.5546 with 2 clusters and PCA = 2







#### RESULTS:



* Customers were successfully segmented into distinct groups
* Each cluster represents a unique customer profile based on:

  * Spending habits
  * Income
  * Family structure
  * Purchase behavior





#### BUSINESS INSIGHTS:



Cluster-0:

&#x20;   - Budget Customers

&#x20;   - More interested in deals for product purchase



Cluster - 1:

&#x20;   - Premium Customers 

&#x20;   - Heavy Purchase and Least Visitors



