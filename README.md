# Disaster-Response-Pipelines

## Project Description

"Data Science Nanodegree Program" by Udacity.
The given dataset contains pre-labelled tweets and messages from real-life disaster. 
The aim of the project is to build a Natural Language Processing tool that categorize messages and predict disaster relationship.
The project includes the following sections:

1. Data Processing ETL Pipeline: to extract data from source, clean data and save them into a proper databse structure
2. Machine Learning Pipeline: to train a model able to classify text message in categories
3. Web App: to show model results in real time. 

*process_data.py: This code extracts data from both CSV files: messages.csv (containing message data) and categories.csv (classes of messages) and creates an SQLite database containing a merged and cleaned version of this data.
*train_classifier.py: This code takes the SQLite database produced by process_data.py as an input and uses the data contained within it to train and tune a ML model for categorizing messages. The output is a pickle file containing the fitted model. 
*run.py: This code runs and visualizes model, also provides the user interface.


### Dependencies
* Python 3.7.6
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK
* SQLlite Database Libraqries: SQLalchemy
* Web App and Data Visualization: Flask, Plotly

## Executing Program:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://localhost:3001/


### Installing
Clone this GIT repository:
```
git clone https://github.com/huanghang111/Disaster-Response-Pipelines.git
```