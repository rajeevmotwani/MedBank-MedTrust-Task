# MedBank-MedTrust-Repository

The dataset consists of two files. Train set and Test set.

I performed exploratory data analysis on the dataset in order to understand the dataset. Although it might not be present in the jupyter notebook, the tasks performed include:
1. Processing of categorical variables using pandas.get_dummies() and continuous variables using sklern.StandardScaler.
2. Removal of variables which had either higher null values or had errors.
3. The target variable had imbalanced class distribution. Hence, I performed oversampling followed by undersampling using imblearn.smotetomek package in order to get equal class distribution.
4. I performed Principal Component Analysis(PCA) for feature selection.
5. I built model on the cleaned dataset by dividing them into train set and test set using Logistic Regression, Decision Trees and Random Forest Classifier.
6. I performed grid search cv in order to find best parameters for Randomforest classifier.
7. (Not Used in the Notebook) I also performed outlier removal in order to reduce the noise from the dataset but that resulted in loss of information. Hence, I did not use that in the final model.
8. Ultimately, I performed the data preprocessing tasks on the test dataset and predicted values for the ids present in the dataset.
9. I saved the result in the format ID, expected in the csv file.

There are two files present in the repository. 

1. The file Medbank-Explained includes the jupyter notebook for the understanding on the user.
2. The file Medbank-Final consists of all the tasks in the for of functions in order to be used on the other files. All the functions are tested and run.
