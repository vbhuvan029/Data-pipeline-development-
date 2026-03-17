# Data-Pipeline-Development
Company : CODETECH IT SOLUTIONS 

Name : V BHUVAN

Intern ID : CTIS6533

Domain : Data Science

Duration : 4 Weeks

Mentor : Neela Santhosh

Description about the Task :

This program demonstrates how to build a simple data preprocessing pipeline using the Python libraries Pandas and Scikit-learn. The purpose of the program is to clean, transform, and prepare a dataset so that it can be used for data analysis or machine learning tasks. In real-world datasets, the data may contain missing values, inconsistent formats, or features with different scales. Therefore, preprocessing the data is an important step before performing any analysis.

The first step in the program is importing the required libraries. Pandas is used for handling and manipulating datasets, while Scikit-learn provides tools for data preprocessing and machine learning. From Scikit-learn, the program imports Pipeline, SimpleImputer, and StandardScaler. The Pipeline class allows multiple preprocessing steps to be combined into a single workflow. This makes the code more organized and easier to manage.

After importing the libraries, the program loads the dataset from a CSV file using the read_csv() function from Pandas. The dataset is stored in a variable called data. This dataset may contain different types of columns, such as text and numeric values. For example, a dataset might include columns like Name, Age  and Attendance. The program prints the original dataset so the user can see the data before preprocessing.

The next step is selecting only numeric columns from the dataset. Machine learning algorithms generally work with numerical data, so it is important to separate numeric columns from text columns. Using the select_dtypes() function, the program extracts columns that contain integer or floating-point values. These columns are stored in a new variable called numeric_data.

Once the numeric data is selected, the program creates a data preprocessing pipeline using the Pipeline class from Scikit-learn. The pipeline contains two important steps. The first step uses SimpleImputer to handle missing values in the dataset. Missing values are common in real datasets and can affect the performance of machine learning models. The SimpleImputer replaces missing values with the mean (average) of the respective column. This ensures that the dataset becomes complete and can be processed further.

The second step in the pipeline uses StandardScaler to standardize the numeric data. Standardization converts the data so that it has a mean of zero and a standard deviation of one. This process helps bring all features to a similar scale. Many machine learning algorithms perform better when the input features are standardized because it prevents one feature from dominating others due to larger numerical values.

After defining the pipeline, the program applies it to the numeric dataset using the fit_transform() method. This method first learns the necessary values, such as the mean and standard deviation, and then applies the transformations to the dataset. The output of this step is the processed data in a numerical format.

Finally, the processed data is converted back into a Pandas DataFrame with appropriate column names. The cleaned and transformed dataset is then saved as a new CSV file called prepared_data.csv. This new dataset can be used for further data analysis, visualization, or machine learning model development. The program also prints a message indicating that the data pipeline has been successfully completed.

Overall, this program demonstrates a simple and effective approach to building a data preprocessing pipeline. It automates the steps of handling missing values, scaling numerical features, and saving the cleaned dataset, making the data ready for further analytical tasks.

Output 

