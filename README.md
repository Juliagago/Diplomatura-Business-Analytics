## Read Me

I conducted this project in the Business Analytics Diploma at Universidad del Aconcagua.

**The goal of this project is to predict the purchase of potential customers, which is crucial to carry out retargeting campaigns that increase the organization's profits and optimize marketing spending.**


**Description of dataset**

Administrative: Number of administrative pages that the user has visited.

Administrative_Duration: Amount of time the user has spent on these types of pages.

Informational: Number of informational pages that the user has visited.

Informational_Duration: Amount of time the user has spent on this type of pages.

ProductRelated: Number of product pages that the user has visited.

ProductRelated_Duration: Amount of time the user has spent on these types of pages.

BounceRates: Percentage of visitors who enter the website through the page they landed on.

ExitRates: Percentage of page views that end on the page they landed on.

PageValues: Internal evaluation of the page.

SpecialDay: Proximity in time to a holiday.

Month: Month.

OperatingSystems: Operating system.

Browser: Browser.

Region: Region.

TrafficType: Traffic type.

VisitorType: Visitor type (New or returning).

Weekend: True/False if is weekend.

Revenue: True/False if the customer has made a purchase.

To achieve this, the following upgrades were executed:

pip install --upgrade pip

pip install --upgrade pycaret


**The data is already separated into Train and Test, so there was no need to split the data:**

**Links dataset:**

train = "https://raw.githubusercontent.com/LucaAPiattelli/Diplomatura_Business_Analytics_UDA/main/Datasets/Clientes_train.csv"

test = "https://raw.githubusercontent.com/LucaAPiattelli/Diplomatura_Business_Analytics_UDA/main/Datasets/Clientes_test.csv"


**The following libraries were imported:**

import pandas as pd

import numpy as np

from pycaret.classification import *

from pycaret.utils.generic import check_metric

import logging, sys
logging.disable(sys.maxsize)

**DEVELOPMENT**

A general analysis of the data was performed.

No null values were found.

In the training data, the "Revenue" variable was replaced with 1 (True) and 0 (False).

The best classification models were compared to apply to the data, and it was concluded that the data should be predicted according to the "Gradient Boosting Classifier" or "GBC" model.

tune_model() was used to optimize the model.

The ROC curve obtained a very good score higher than 0.93.

The confusion matrix had 2201 correct predictions and made errors in 287 cases, which means it had a 10% error in predicting the data.

**CONCLUTION**

In conclusion, this project aimed to predict the purchase of potential customers to enable retargeting campaigns that increase the organization's profits and optimize marketing spending. By analyzing the data and using the "Gradient Boosting Classifier" or "GBC" model, we were able to achieve a very good score on the ROC curve and a 10% error rate in predicting the data. Overall, this project provides a useful framework for predicting customer purchases and can be used as a basis for further research and development in the field of data science.


```python

```
