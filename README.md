# Description

Recognize the spam email using Machine Learning by `sklearn` and `pandas`.

This project implements a simple email filter, which recognize the spam and ham emails.

The modes uses `Multinomial Navie Bayes` to classify the emails.

# Details about train and test

At the beginning, I clean the dataset by removing the `Email No.` column that’s not taken account into the prediction model. Then we can start to build the model.

First, it uses `train_test_split` to split the `train_emails` as `train` and `test` by the ratio 8:2.

Then, it use `MultinomialNB` to train the model.

After that, it uses `test` to calculate the `mean accuracy`, `ROC AUC`, `confusion matrix`, `precision` and `recall` scores to determine how accurate the model really is.

Moreover, I also use another email dataset to check the accuracy, which is a little lower than that of the `test` data aparted from the `train_emails`, but is still accurate to filter the spam and ham emails.

# How to use

You can see the result in https://github.com/KyanChen/Spam-Email-Recognization/blob/master/spam-recognization.ipynb

Alternatively, you can see it using Microsoft Azure Notebooks by https://notebooks.azure.com/cche7346/projects/spam-recognization

If you want to run the Jupyter Notebook on your own machine, you can clone files and run it. But note that I run it by `python 3.8.2`, `pandas 1.0.1` and `sklearn 0.23.0` on `MacOS 10.15.4`. I didn’t test it on other versions.

# Acknowledge

The `train_emails.csv` is from https://www.kaggle.com/balaka18/email-spam-classification-dataset-csv

The `test_emails.csv` is from https://www.kaggle.com/venky73/spam-mails-dataset.

