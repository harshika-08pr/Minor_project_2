MINOR PROJECT REPORT 

Title : 
Customer Segmentation using K-Means Clustering 

Submitted By: 

Name: ______Harshika____________________ 

Roll Number: ___202501100400151_________________ 

Course: Machine Learning 


  
Problem Statement

Customer segmentation is one of the most useful applications of machine learning in businesses. Shopping malls have customers with different purchasing habits, spending capacities, and age groups. It becomes difficult for the management to identify similar types of customers manually. 
The main purpose of this project is to group customers into different clusters based on their characteristics such as Age, Annual Income, and Spending Score using the KMeans Clustering algorithm. These customer groups can help businesses understand customer behaviour and make better marketing decisions.

  
 Project Objective 
 
The main objectives of this project are: 
•	To understand the complete machine learning workflow.  
•	To preprocess a real-world dataset.  
•	To perform Exploratory Data Analysis (EDA).  
•	To apply the K-Means Clustering algorithm.  
•	To evaluate the clustering model using suitable evaluation techniques.  
•	To save the trained model for future use.  

  
Dataset Description 

Dataset Name: Mall Customers Dataset 

Source: Kaggle 

https://www.kaggle.com/datasets/shwetabh123/mall-customers 	

Python notebook link : 

https://colab.research.google.com/drive/1ecjJvSySGM3XRU7608w7JXGevk_PWXp a?usp=sharing 	 

Dataset Information 

•	Total Records: 200  

•	Total Features: 5  

Features 

Feature 	Description 

CustomerID 	Unique ID of each customer 
Genre 	Gender of the customer 
Age 	Age of the customer 
Annual Income (k$) 	Annual income of the customer 
Spending Score (1100) 	Score assigned by the mall based on customer spending behaviour 
  
Data Preprocessing 

The following preprocessing steps were performed: 
•	Loaded the dataset using Pandas.  
•	Displayed the first five rows of the dataset.  
•	Checked the shape of the dataset.  
•	Displayed dataset information.  
•	Checked missing values.  
•	Checked duplicate records.  
•	Displayed statistical summary.  
•	Encoded the Gender/Genre column using LabelEncoder.  
•	Removed the CustomerID column as it is not useful for clustering.  
•	Applied StandardScaler to normalize the feature values.  
These preprocessing steps prepared the dataset for clustering and improved the performance of the K-Means algorithm. 
  
Exploratory Data Analysis (EDA) 

EDA was performed to understand the dataset before training the model. 
The following visualizations were created: 
•	Histogram
<img width="2483" height="2042" alt="Histogram graph" src="https://github.com/user-attachments/assets/78139fe2-3a64-4af6-9a60-ff02b89b983a" />

•	Boxplot  
<img width="2493" height="1517" alt="Boxplot" src="https://github.com/user-attachments/assets/2fa26c36-db64-497b-b8c9-5dd20cd62a1e" />

•	Correlation Heatmap  
<img width="2361" height="1983" alt="Heatmap" src="https://github.com/user-attachments/assets/e2dffdc3-dda0-4094-8991-b8841f1b4484" />

•	Elbow Method Graph  
<img width="1854" height="1407" alt="Elbow method" src="https://github.com/user-attachments/assets/53003708-b7b1-4ae5-80c0-f08c7b5705d4" />

•	Customer Cluster Visualization  
<img width="2087" height="1638" alt="Customer clusters" src="https://github.com/user-attachments/assets/d5c8a3ca-edfe-452a-b7e9-5c8e83075738" />

  
Observations 

•	The dataset contains customers of different age groups and income levels.  
•	No missing values or duplicate records were found.  
•	Annual Income and Spending Score showed different customer spending patterns.  
•	The Elbow Method suggested that 5 clusters are suitable for this dataset. 
  
 Model Used 
 
The machine learning algorithm used in this project is K-Means Clustering. 
Why K-Means Clustering? 
•	Simple and easy to understand.  
•	Suitable for customer segmentation.  
•	Groups customers with similar characteristics.  
•	Fast to train on small and medium-sized datasets.  
•	Beginner-friendly unsupervised learning algorithm.  
  
Training Process 

The following steps were followed: 
1.	Import the required libraries.  
2.	Load the dataset.  
3.	Perform data preprocessing.  
4.	Encode the categorical feature.  
5.	Apply feature scaling using StandardScaler.  
6.	Use the Elbow Method to find the optimal number of clusters.  
7.	Train the K-Means Clustering model.  
8.	Assign cluster labels to each customer.  
9.	Evaluate the model using the Silhouette Score.  
  
Evaluation Metrics and Results 

Since this is an unsupervised learning project, the model was evaluated using: 
•	Elbow Method  
•	Silhouette Score  
Results Metric 	Result 
Total Records 	200 
Missing Values 	0 
Duplicate Records 0 
Number of Clusters 5 
Silhouette Score 	0.2719 
Cluster Distribution Cluster Number of Customers 
Cluster 0 51 
Cluster 1 20 
Cluster 2 42 
Cluster Number of Customers 
Cluster 3 49 
Cluster 4 38 
Result Analysis 
The Elbow Method indicated that 5 clusters were suitable for this dataset. After training the K-Means model, customers were successfully grouped into five different clusters based on their age, annual income, and spending score. 
The obtained Silhouette Score of 0.2719 indicates that the model was able to form meaningful customer groups. These clusters can help shopping malls identify different types of customers and plan suitable marketing strategies.
  
Conclusion 

In this project, the K-Means Clustering algorithm was used to perform customer segmentation using the Mall Customers dataset. 
The dataset was successfully preprocessed, explored through data visualization, and used to train the clustering model. The model divided the customers into five different clusters based on their purchasing behaviour. The clustering performance was evaluated using the Silhouette Score, and the trained model was saved as a .pkl file for future use. 
This project helped in understanding the complete workflow of an unsupervised machine learning project, including data preprocessing, visualization, clustering, evaluation, and model saving. 
  
Future Scope 

The project can be improved by: 
•	Using larger customer datasets.  
•	Applying other clustering algorithms such as DBSCAN and Hierarchical Clustering.  
•	Adding more customer features for better segmentation.  
•	Deploying the saved model using Streamlit or Flask.  
•	Comparing the performance of different clustering algorithms. 
  
References 

1.	Kaggle – Mall Customers Dataset  
2.	Scikit-learn Documentation  
3.	Pandas Documentation  
4.	NumPy Documentation  
5.	Matplotlib Documentation  
6.	Seaborn Documentation  
 
 Answers to Theory Questions 
 
Q1. Differentiate between Semantic Segmentation, Instance Segmentation and Panoptic Segmentation. 
Semantic 
Instance Segmentation Panoptic Segmentation Segmentation 
It identifies each object 

It classifies every pixel into a category. 
It combines both semantic and separately, even if they belong instance segmentation. to the same category. 

Objects of the same 
Each object gets a separate class are not 
label. separated. 	Every pixel is classified and each object is uniquely identified. 
Example: All cars are 	Example: Every car is marked as one class. 	detected individually. 	Example: Every car is detected separately while also classifying roads, buildings, etc. 
  
Q2. Differentiate between Fuzzy Logic and Boolean Logic. 
Fuzzy Logic 	Boolean Logic 
Values can range between 0 and 1. 	Values are only 0 or 1 (True or False). 
It works only with exact true or false It handles uncertainty and partial truth. conditions. 
Used in smart systems like washing machines 	Used in digital circuits and computer and air conditioners. 	programming. 
  
Q3. Why is this dataset suitable for K-Means Clustering? 
The Mall Customers dataset contains customer information such as age, annual income and spending score. These features help group customers with similar behaviour. Since the dataset does not contain target labels, K-Means is a suitable algorithm for finding natural customer groups. 
  
Q4. Why was K-Means chosen for this project? 
K-Means was selected because: 
•	It is simple and easy to understand.  
•	It is suitable for customer segmentation.  
•	It works well with numerical data.  
•	It is fast and beginner-friendly.  
•	It creates meaningful customer groups.  
  
Q5. What are the applications of Customer Segmentation? 
Customer segmentation is useful in many business applications, such as: 
•	Targeted marketing  
•	Personalized offers and discounts  
•	Customer relationship management  
•	Business decision-making  
•	Improving customer satisfaction  
  
  
Declaration 

I hereby declare that this project has been completed by me as part of the Minor Project for the Machine Learning course. The work submitted is based on my understanding of the concepts learned during the course and the references mentioned above. 
 
 

