# Disaster-Response-Pipelines

## Project Description

"Data Science Nanodegree Program" by Udacity.
The given dataset contains pre-labelled tweets and messages from real-life disaster. 
The aim of the project is to build a Natural Language Processing tool that categorize messages and predict disaster relationship.
The project includes the following sections:

1. Data Processing ETL Pipeline: to extract data from source, clean data and save them into a proper databse structure
2. Machine Learning Pipeline: to train a model able to classify text message in categories
3. Web App: to show model results in real time. 

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