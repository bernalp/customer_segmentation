# customer_segmentation

** this is still draft repositories, I working on code in other workspaces.
sorry for inconvenience from unfinished page.

### Introductions

### Project Motivation

### File Descriptions

### Results
- found findings about aged group proportion, **will upload the result once my workbook finished
- found insights when comparing the proportions from financial type between general population and the customer group.
- findings in proportions based on income distribution

### Acknowledgemnts

### Last progress on other workbook
- continue analytics using some visualization
- aggregate and visualize the distribution values
- preparing data cleaning and data preprocessing steps
- woking on clean_data function due to memory limitaitons
- solved try clean_data function using this scenario
    - Cleaning specific columns
    - Handling unknown values
    - Dropping unnecessary columns
    - Creating dummy variables for categorical columns
    - Removing rows and columns with a high percentage of missing values
    - Handling outliers in the 'ANZ_HAUSHALTE_AKTIV' column
    - And limiting fraction by 2% of dataframe for efficiency
- drop "AGER_TYP" column since it has high 76.4% missing values, and impute missing values in other columns.
- editing MinMaxScaler script
- create an instance of PCA and calculate principal components
- create figure 'Cumulative Explained Variance Ratio by PCA Components'
- create an instance of PCA class with 180 principal components
- calculate the principal components while retaining only 180 components
- create a list of component labels for the principal components obtained from PCA analysis
- create a DataFrame (df_pca_180) to store the principal components as rows and features as columns
- calculate the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters
- create a plot to visualize the Within-Cluster Sum of Squares (WCSS) for different numbers of clusters
- fixing silhouette_score calculations due to memory limitations
- create list containing the results of the MiniBatchKMeans clustering algorithm
- predict the cluster labels using 5 clusters
- create a countplot using the predicted cluster labels obtained from KMeans
- create a DataFrame containing the mean values of the features in azdias_clean
- calculate the mean values of features for each cluster in the 'kmeans_cluster' column
- rename the index of the 'cluster_means' DataFrame to make it more descriptive
- Findings (5): Cluster-Based Profiles: How Clusters Differ from Overall Dataset
- Clean the customers dataset & Keep the same columns as in azdias dataset
- Check & handling missing values in customers dataset
- Scale the customers' data using the same scaler as applied to the azdias dataset
- Create dataframes for cluster labels of both general population and customers datasets & add 'type' column to distinguish between them
- Calculate the number of data points in each cluster for both general population and customers datasets
- Calculate the total number of data points for each dataset
- Merge the counts of data points per cluster with the total counts per dataset
- Calculate the proportion of data points in each cluster for both datasets
- Create a bar plot to visualize cluster proportions
- Calculate cluster proportions for customers
- Calculate cluster proportions for the general population
- Display percentages for each cluster for both customers and the general population
- Findings (6): Cluster Analysis: Comparing Customer and General Population Segment
- Continue progress on Part 2: Supervised Learning Model
- summary basic info and statistic drom mailout_train dataset
- Clean the 'mailout_train' dataset using a custom 'clean_data' function
- Extract the 'RESPONSE' column as the target variable
- Remove the 'RESPONSE' column from the training dataset as it's the target variable
- check and display missing values and percentages
- Replace NaNs with the mean value in mailout_train_clean
- Apply scaling to the 'mailout_train_clean' data using the fitted scaler
- Apply dimensionality reduction to the 'mailout_train_scaled' data using the learned PCA model with 100 components
- Split the data into features (X) and the target variable (y)
- Split the dataset into training and testing sets
- Calculate the counts of unique elements in y_test & y_train
