# Data Analysis-Predicting whether a user clicks on an advertisement or not

# Aim of the project
In this case study ,I determine the number of users who are likely to click on an advertisement given information about the user.

# Python Libraries needed:
* Pandas
* Numpy
* Matplotlib
* Seaborn

# File Description
* The Code folder consists of the Jupyter Notebook that contains the code and visualization of the entire project working.
* The Dataset folder contains advertisement.csv file that contains the dataset.


# Dataset Description
This dataset consists of 9 feature columns and 1 target column 'Clicked on Ad' that we want to predict.
## Feature Columns
* Daily Time (Float)
* Age (Integer)
* Area Income (Float)
* Daily Internet Usage (Float)
* Ad Topic Line ( String)
* City (String)
* Male (Boolean)
* Country (String)
* Timestamp ( Date)

# Step-by-step instructions on how I approached the project
1. The first and foremost step before any data science project is to analyze the data i.e do an EDA(Exploratory Data Analysis).

    1.a  Checked if the data consisted of Null values.
  
    1.b  Built a correlation matrix between the different columns in the dataset which can be seen by a beautiful correlation matrix in          the notebook.
  
    1.c Used pandas_profiling to get a deep sense of each feature column and target attribute.
  
2.  The second step is to preprocess the data before feeding it into the model.
    2.a Label encoded the String columns since Machine lerning models are all about dealing with numbers! Exciting!
    2.b Used a scatterplot to visualize the transformed data.
3.  The third step is to feed the data to the model
    3.a I start off by training my data on a simple Logistic Regression model which gave me an accuracy of 91% with number of True    Positives as 89 and number of True Negatives as 93. (Total number of test data-200). Precision-90%, Recall-92%, F-1 score-91%.
  
    3.b Then I trained my data on a more powerful model( Decision trees). Accuracy-94%, TP- 90 TN- 95 Precision-93%, Recall-94%.
  
    3.c Using the powerful bagging classifier- Random Forest model(100 decision trees)- Accuracy- 97% TP-95 TN- 98, Precision- 94%,   Recall - 95%.
  
The above results are also backed up by a ROC curve that depicts the True positive and False positive rate.

# Conclusion
I was able to successfully predict the users who are likely to click the advertisemnt data with an accuaracy of 97% using the Random Forest model with 100 decision trees.


  
  
