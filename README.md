# Description of My Idea in this Project

This repository outlines my progress in developing my own Machine Learning (ML) Model Using the library XGboost which uses gradient boosting to create a powerful committee from weak classifiers. It also details my development of a sequential Neural Network (NN) using the Keras library. In this project, I aimed to demonstrate how we can use Machine Learning and Neural Networks to aid in predicting Parkinsons disease in individuals. I aimed to demonstrate this as Parkinsons is a very complex disease with large amounts of uncertainty in regards to how its caused, how it can be identified and how it can be cured or prevented. But with the help of AI/ML, we can make more informed decisions about these uncertainties and these decisions may end up saving lives.

My idea for the ML/AI project in the MSA 2020 Bootcamp was to create an ML model which used a dataset of Parkinsons patients to determine which people had Parkinsons, I managed to create this model with a ~95% accuracy which is something that I am proud of. I made this model with the use of the following libraries:

•	numpy 

•	pandas

•	os, sys

•	sklearn.preprocessing, MinMaxScaler

• xgboost, XGBClassifier

•	sklearn.model_selection, train_test_split

•	sklearn.metrics, accuracy_score

This was a really intriguing and immersive experience from which I learned about gradient boosting and how to create ML models to help improve the quality of life of people around the world

However, I wasn't satisfied with just having a working ML model so I did some in-depth research into how to program a sequential neural network so that I could detect Parkinsons from the UPDRS dataset which was given. UPDRS stands for Unified Parkinson's disease rating scale, it is a scale which General Practitioners and clinics use to determine whether patients have Parkinsons disease. This scale is scored from 0-199, with 199 meaning the most severe case of Parkinsons. From this total_UPDRS dataset, I aimed to create a Neural network which would be able to identify patients with Parkinsons. I succeeded in creating this NN by using tanh activation, sgd optimiser and mean squared error for my loss. This network managed to predict Parkinsons disease with a ~63% accuracy. Despite being significantly less accurate then my ML model the Neural network performed well given how the data set required the NN to be performed on largely positive numbers. 

Overall, I'm really happy with what My ML and NN models achieved with the Parkinsons datasets, and I'm really keen to create more ML models in the future :)

### **Environment Setup and Dependencies**
All development was done within Microsoft Azure Notebooks, writing all code into a Jupyter notebook (using Python 3.6). This proved to be extremely helpful, as very little time was dedicated to setting up the development environment – with only the notebook file needing to be created.

## **How to set up the dependencies and train my data:**

In order to be able to use the xgboost library you need to install it using the 
```
!pip install xgboost
```
Command.

In regards to other libraries they can all be imported normally see code below
```
import numpy as np
import pandas as pd
import os, sys
from sklearn.preprocessing import MinMaxScaler
from xgboost import XGBClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score
```

After you import all of the dependencies you need to download the **parkinsons.data** and **/telemonitoring/parkinsons_UPDRS.data** files from **https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons** Then upload these data sets to your azure project.


Next run all of the different lines and view the output to see that it matches what I wrote above
