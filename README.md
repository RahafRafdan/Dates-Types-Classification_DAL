# Dates-Types-Classification using ConvNeXt-Tiny (DAL competetion)

This notebook implements a solution for classifying different types of dates (Ajwa, Medjool, Meneifi, Nabtat Ali, Shaishe, Sokari, and Sugaey) using the ConvNeXt-Tiny model. The model is trained on a dataset from a Kaggle competition, and includes techniques to handle class imbalance and prevent overfitting.

Overview

The notebook consists of two main parts:

1. Initial Model Training
The first part of the code focuses on loading the data, preprocessing and augmenting it, and training the ConvNeXt-Tiny model. However, the model overfitted.
2. Enhancement to Prevent Overfitting
After observing the model’s tendency to overfit, adjustments were made to prevent this:
MixUp augmentation was added as a regularization technique.
A Dropout layer was introduced to the model architecture to improve generalization.
Class imbalance handling was implemented using weighted sampling.
Early stopping and learning rate scheduling were applied to monitor the training and prevent overfitting to the test data.
The final output includes model evaluation on the test set and saving predictions in the required submission format for the competition.
