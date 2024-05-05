
# PriceBulldozerAI


## Introduction
For this coding project, I've chosen to manipulate data from a Kaggle competition and construct a fictional backstory. The project entails predicting the auction sale price for specific heavy equipment, considering its usage, type, and configuration. The data comes from auction results, offering deep insights into equipment usage and configurations. The ultimate aim is to assist Fast Iron's initiative to create a "blue book for bulldozers," which would help customers assess the value of their heavy equipment fleet at auction.

The project data is sourced from a public Kaggle competition, which can be accessed through the following URL: [Blue Book for Bulldozers] (https://www.kaggle.com/c/bluebook-for-bulldozers/overview)

## Table of Contents
- [Table of Content](#table-of-contents)
    - [PriceBulldozerAI](#pricebulldozerai)
    - [Introduction](#introduction)
    - [ML Business Case](#ml-business-case)
    - [Dataset Content](#dataset-content)
    - [Project Hypothesis and Validation](#project-hypothesis-and-validation)
    - [Explanation for linking business needs to Data Visualizations and ML tasks](#explanation-for-linking-business-needs-to-data-visualizations-and-ml-tasks)
    - [Dashboard Design](#dashboard-design)
    - [Unfixed Bugs](#unfixed-bugs)
    - [Deployment](#deployment)
        - [Heroku](#heroku)
    - [Main Data Analysis and Machine Learning Libraries](#main-data-analysis-and-machine-learning-libraries)
    - [Credits](#credits)
    - [Acknowledgements](#acknowledgements)

## ML Business Case
1. What are the business objectives?
    1. The objective of this project is to precisely forecast the auction prices of bulldozers. Specifically, the aim is to ascertain the degree of accuracy with which the future sale price of a bulldozer can be predicted, considering its features and the past sale prices of comparable bulldozers.
2. What does the client consider as a successful project outcome?
    1. The evaluation metric for the client is the Root Mean Squared Log Error (RMSLE). The target is to achieve a score lower than 0.25612 between the actual and predicted auction prices.
3. Does the data suggest a particular model?
    1. Since the goal is to predict a number, the project model will be a regression problem. It will use a RMSLE (root mean squared log error), as requested by the client.
4. Is there any business objective that can be answered with conventional data analysis?
    1. Indeed, conventional data analysis can be employed to examine the correlation between bulldozer attributes and their sale price.
5. Can you break down the project into Epics and User Stories?
    1. Information gathering and data collection.
    2. Data visualization, cleaning, and preparation
    3. Model training, optimization and validation.
    4. Dashboard planning, designing, and development.
    5. Dashboard deployment and release.
6. What are the model's inputs and intended outputs?
    1. Upon reviewing the client's dataset, it's clear that it presents a time-series regression problem, indicating that there is a time attribute associated with the dataset.
    2. In particular, our reference data comes from past bulldozer sales records. These records include information such as model type, size, sale date, and more.
    3. There are 3 datasets:
        1. **Train.csv** - Historical bulldozer sales examples up to 2011 (close to 400,000 examples with 50+ different attributes, including `SalePrice` which is the **target variable**).
        2. **Valid.csv** - Historical bulldozer sales examples from January 1 2012 to April 30 2012 (close to 12,000 examples with the same attributes as **Train.csv**).
        3. **Test.csv** - Historical bulldozer sales examples from May 1 2012 to November 2012 (close to 12,000 examples but missing the `SalePrice` attribute, as this is what we'll be trying to predict).
7. How will the client benefit?
    1. This is very helpful for our client because it allows them to plan their finances and budget accurately based on the estimated selling price.
    2. It helps them decide when to sell their equipment for the highest profit.
    3. Also, our predictions give a fair, data-based valuation.
    4. This helps buyers understand how much the equipment is worth and negotiate a fair price.
8. Does the client need a dashboard or an API endpoint?
    1. The client needs a dashboard
9. Are there any ethical or privacy concerns?
    1. There are no ethical or privacy concerns since the Kaggle competition data is publicly published.
10. What are the criteria for the performance goal of the predictions?
    1. The client has established the evaluation measure as the Root Mean Squared Log Error (RMSLE). The aim is to achieve the smallest possible score, indicating a more accurate prediction.

## Dataset Content

[Back to Table of contents](#table-of-contents)

## Project Hypothesis and Validation

[Back to Table of contents](#table-of-contents)

## Explanation for linking business needs to Data Visualizations and ML tasks

[Back to Table of contents](#table-of-contents)

## Dashboard Design

[Back to Table of contents](#table-of-contents)

## Unfixed Bugs

[Back to Table of contents](#table-of-contents)

## Deployment
### Heroku
* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ <!-- TODO:Replace with actual app heroku address  -->
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. At the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.

[Back to Table of contents](#table-of-contents)

## Main Data Analysis and Machine Learning Libraries

[Back to Table of contents](#table-of-contents)

## Credits 
### Recognizing Contributions
### Ensuring Compliance with Legal and Ethical Standards
This project doesn't involve any ethical or privacy issues since the data used is publicly available from a Kaggle competition. The data for this project can be accessed from the following Kaggle competition: https://www.kaggle.com/c/bluebook-for-bulldozers/overview.

[Back to Table of contents](#table-of-contents)

## Acknowledgements 

[Back to Table of contents](#table-of-contents)

---


