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
- Continue progression: Random Forest Classifier
- Create a Random Forest Classifier with balanced class weights
- Define a parameter grid for hyperparameter tuning -> testing several case to keep data quality but reduce time consume 
- Create a grid search using cross-validation to find the best hyperparameters for the classifier
- Fit the grid search to find the best hyperparameters for the classifier
- Get the best estimator (model) from the grid search
- Create the 'data' directory & Save the best model to a file using pickle
- Get the best hyperparameters from the grid search
- Calculate the accuracy score of the best model on the training data & testing data
- Make predictions on the testing data using the best model
- Create a confusion matrix to evaluate the model's performance on the testing data
- Calculate the ROC AUC score to evaluate the model's performance on the testing data
- Continue progression: Logistic Regression
- Define a parameter grid for hyperparameter tuning for Logistic Regression
- Create a Logistic Regression classifier with balanced class weights and increased maximum iterations
- Create a grid search using cross-validation to find the best hyperparameters for the logistic regression classifier
- Get the best estimator (model) from the grid search for logistic regression
- Save the best logistic regression model to a file using pickle
- Retrieve the best hyperparameters found by the grid search for the logistic regression model
- Use the best logistic regression model to predict on the test data
- Create a confusion matrix to evaluate the logistic regression model's performance on the testing data
- Calculate the ROC AUC score to evaluate the logistic regression model's performance on the testing data
- testing more due eficiency in running time
- Continue progression: XGBoost
- Create an XGBoost Classifier with a specified scale_pos_weight
- Define a parameter grid for hyperparameter tuning
- Create a grid search using cross-validation to find the best hyperparameters for the XGBoost classifier
- Get the best estimator (model) from the grid search
- Predict using the best XGBoost model
- Create a confusion matrix to evaluate the XGBoost model's performance on the testing data
- Calculate the ROC AUC score to evaluate the XGBoost model's performance on the testing data
- Continue progression: Models evaluation
- Create a confusion matrix with specified labels to evaluate the model's performance
- Calculate accuracy from a confusion matrix.
- Create a summary DataFrame with evaluation metrics for different classifiers
- Findings (7): Evaluating ROC AUC and Accuracy Metrics
- Bundling previous work into a function
- Plots the learning curve of a machine learning model using the provided estimator, train_sizes, and cross-validation strategy.
- Try different approach to make computation time better
- Still working on learning_curves function due to computation limit
- Plotting learning curves for different models
- Visualizing ROC curves for different models
- Visualizing Confusion Matrix for different models
- Final Conclusions
- Understand Customer Behavior
- Predict and Prevent Problems
- Optimize Resource Allocation
- Continuous Improvement & Adaptability
- Creating Happy Customers
- finishing script for conclusions and future improvement
- Find technical Improvements possibility
- Future Improvements
- Keep Updated Real-Time Data
- Enchance Data Knowledge
- Explore Advanced Analytics
- Collaboration is Key
- Technical Improvements
- Review Data Quality
- Feature Engineering
- Model Improvement
- Class Imbalance
- Domain Expert Consultation
- Regular Model Evaluation
- Explore External Factors
- Customer Segmentation
- Experimentation and Prototyping
- Closure
- added Acknowledgments
- added Table of Contents
- edit script for business questions
- double check and edit script to make sure introduction an final conslusions linear
- restructure sub-section from project workspace

