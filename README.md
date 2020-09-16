# AzureML Predictive maintenance Hackathon

This repository is set up to get you up and running with AzureML as a first prep for the DP-100 exam. 
To give this hackathon more body we will focus on a predictive maintenance use case (or technically: predicting production failures). 
We wil use a steelplate faults dataset retrieved from https://archive.ics.uci.edu/ml/datasets/Steel+Plates+Faults.

## Data preprocessing
Since predictive maintenance is focused on forecasting potential unhealthy results (machine/production failures), we will adjust the dataset to comply with this goal. 
The original dataset does not include healthy data by default. 
Therefore, we will consider one fault type as 'healthy' ('Other_faults') and another one as 'unhealthy' ('Stains'). 
Of course, this is a decision you might want to change according to new insights.
To make sure we have enough data left after these adjustments, a new, larger dataset was synthesized. 
The data can be found in the `data` folder.
Apart from the healthy/unhealthy division, this also requires some additional preprocessing to sync its characteristics to the original dataset and prepare it for training.

All the preprocessing steps described are performed in the first notebook, Data preprocessing. 
This notebook will not only get you acquainted with the data, but also learn you some concepts of working with data in Azure ML.

## Training models
Once the data is prepared, it is time to get started with the actual machine learning part. As an example, a basic xgboost model was trained to get some first results.
Along the way you will learn different concepts of AzureML and how to use them as you build and train your ML models.

After you get to know some of AzureML's most important concepts, it's time to start building yourself and let AzureML (studio) help you to get to the optimal model.
