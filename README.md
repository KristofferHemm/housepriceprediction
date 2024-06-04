# Housepriceprediction

## Project description
This project consists of a classification task.\
The task is to predict which of 3 price classes a property in the city belongs to.

The dataset for this project consists of property data from Melbourne.\
The features are a mix of continuous and categorical variables.\
The target feature is unbalanced, so using macro f1 score as the training metric is the natural choice.


## Results
After training multiple classification models on the dataset, both with outliers removed and on with outliers left in the dataset, our best performing model was random forest classifier trained on the dataset with outliers removed. \
This generally produced poor results, so we will try to upsample the minority classes in the dataset using SMOTE, and train the random forest classifier again. \
Using the random forest classifier on the upsampled dataset produced the best results, with a macro f1 score of 0.91.
