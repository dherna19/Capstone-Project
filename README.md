# Capstone-Project
Udacity Data Scientist Nanodegree Capstone

# Project Motivation
For this Udacity project, I will analyze customer mailing data and compare it to the general population data for Germany in order to cluster customers into segments
and see which type of people are more likely to purchase. Another dataset with the actual responses of a mailout campaign
will be used to train a supervised machine learning model that will predict the liklehood of someone becoming a customer. 

# Main notebook: Arvato
The Python script, process_data.py, is data cleaning pipeline that:

- Loads customer and general population data
- Cleans the data
- Prepares/processes the data
- Customer Segmentation Report: Shows cluster of different buyers
- Supervised Machine Learning Model: Uses RandomForestClassifier to predict customers responding to mail-out campaign


# Kaggle_competition_2
A .csv file with two columns, LNR, for the identification number, and RESPONSE, with the prediction probabilities of my model. I had originally saved my predictions
using an index=False parameter which I then went back to change and therefore renamed my submission .csv file to _2.



# Installation
This project requires Python 3.6 and the following Python libraries installed:
- Pandas
- Sci-kit learn
- NumPy
- IPython
- Matplotlib
- Seaborn


# Data
Data was provided by Arvato and Udacity 
File Descriptions
These were the files used for the notebook, however, this is not public data and therefore cannot be shared.

Jupyter Notebook, CSV files:
-	udacity_azdias.csv: Describes demographic data for general German population. Data dimensions: 891211 observations and 366 features, 6 outlier columns with more than 40% of data missing. Mixed-data types
- udacity_customers.csv : Describes demographic data for the mail-order company
Data dimensions: 191652 observations and 369 features
The three additional features include CUSTOMER_GROUP, ONLINE_PURCHASE and PRODUCT_GROUP. Some of these are binary features and some can be dropped

- missing_vals.csv: using two excel sheets provided by Udacity, I was able to create this .csv file that maps the missing/unknown value to columns in order to 
use them in a cleaning function that converts the missing values in that column to np.Nan


# Acknowledgement
This dataset is part of Arvato and Udacity. It is not data for public use
I have answered a lot of my questions relating to data cleaning and preparation using different sources from StackOverFlow and other websites:
https://stackoverflow.com/questions/27719407/pandas-concat-valueerror-shape-of-passed-values-is-blah-indices-imply-blah2
https://www.analyticsvidhya.com/blog/2015/06/tuning-random-forest-model/
https://stackoverflow.com/questions/33700626/how-to-convert-tuple-of-tuples-to-pandas-dataframe-in-python/33700770
https://stackoverflow.com/questions/35359969/typeerror-tuple-indices-must-be-integers-not-str
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.reset_index.html

# Blog
I made a blog on Medium to show my findings. This can be found [here](https://medium.com/@deniseher44/customer-segmentation-and-supervised-learning-with-arvato-data-2065ef5a57f3?sk=3e65a826df5a8f0bf00f09cc50fe2e85)
