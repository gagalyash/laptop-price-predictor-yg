# Laptop Prices Predictor
<ul>
  <li>Designed a web app that predicts the price of the laptop given the configurations. </li>
  <li>Scraped the laptops data from kaggle using python and Opendatasets package.</li>
  <li>Developed Linear, Lasso, and Random Forest Regressors using GridsearchCV to get the best model.</li>
  <li>Deployed the Machine Learning model using streamlit library on Heroku.</li>
</ul>

# Links and Resources Used
<li>Streamlit Library: <a href="https://www.streamlit.io/">https://www.streamlit.io/</a>
<li>Dataset Link: <a href="https://www.kaggle.com/ionaskel/laptop-prices/">https://www.kaggle.com/ionaskel/laptop-prices/<a>
<li>heroku Platform: <a href="https://www.heroku.com/">https://www.heroku.com/</a>
<li>Packages: pandas, numpy, matplotlib, seaborn, sklearn, pickle, streamlit</li>


# Feature Engineering
We go through all the features one by one and keep adding new features. I have made the following changes and created new variables:
- RAM - Made columns for Ram Capacity in GB  <br>
- Processor - Made columns for Name of the Processor, Type of the Processor, Generation <br>
- Operating System - Parsed the Operating System from this column and made a new column <br>
- Storage - Made new columns for the type of Disk Drive and the capacity of the Disk Drive <br>
- Display - Made new columns for the size of the laptop(in inches) and touchscreen <br>
- Description - Made new columns for the company and IPS <br>

# Data Preprocessing
There are a few columns which are categorical here but they actually contain numerical values.So we need to convert few categorical columns to numerical columns. These are ram, weight, hdd, ssd.

# Model Building
<li>Traditional Method</li>
Used scikit-learn library for the Machine Learning tasks. Applied label encoding and converted the categorical variables into numerical ones.Then I splited the data into training and test sets with a test size of 20%. I tried different regression models ( Linear Regression, Random Forest Regression, XGBoost) and evaluated them using Mean Absolute Error. 

# Model Deployment
- I have deployed the model using Streamlit library on Heroku which is a Platform As A Service(PAAS)

- Web application: <a href="https://laptop-price-predictor-yg.herokuapp.com/">https://laptop-price-predictor-yg.herokuapp.com/</a>
