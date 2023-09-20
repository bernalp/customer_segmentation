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
