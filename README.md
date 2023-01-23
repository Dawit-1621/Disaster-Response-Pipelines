
# Disaster Response Pipelines

## Installation
**Importing Libraries**</br>
* numpy
* pandas
* matplotlib
* sklearn
* Flask web app framework
### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.
    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`
2. Run the following command in the app's directory to run the web application 
    `python run.py`

3. Go to http://0.0.0.0:3001/

## Project Motivation
This project is about disaster response. I’m interested to build this project because it shows a detailed data engineering skills process. In this project, there are three basic components of data engineering. The first one is the ETL pipeline, which is a type of data integration process. The second, ML pipeline describes the ML process: writing code, releasing it to production, performing data extractions, creating training models, and tuning the algorithm. The last one is the deployment process using the Flask web application. The Flask provides tools, libraries, and technologies that allow us to build web applications. To run the web app using Flask, import the Flask module and create a Flask web server from the Flask module.
## Porject Descriptions 
There are three components in this project. </br>
**1. ETL(Extract, Transform, Load) Pipeline a data pipeline that:** 
* Loads the messages and categories datasets
* Merges messages and categories datasets
* Cleans the datasets
* Stores it in a SQLite database
* After ETL pipeline done then the database link to ML pipeline to develop the model

**2.ML Pipeline: a Machine Learning pipeline that:**
* Loads data from the SQLite database
* Splits the dataset into training and test sets
* Builds a text processing and machine learning pipeline
* Trains and tunes a model using GridSearchCV
* Outputs results on the test set
* Exports the final model as a pickle file
 
**3.Flask Web App**
Python web framework that provides useful tools and features that make creating web applications

## Licensing, Authors, Acknowledgements
I Acknowledge the www.udacity.com and https://www.figure-eight.com/
