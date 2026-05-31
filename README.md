# imageclassifier
Dogs vs. Cats Image Classification using Support Vector Machine (SVM)
This repository contains a Google Colab notebook demonstrating a basic image classification task using a Support Vector Machine (SVM) to distinguish between images of dogs and cats. The dataset used is the popular Kaggle Dogs vs. Cats Redux: Kernels Edition dataset.

Project Overview

The goal of this project is to build and evaluate a simple SVM model for binary image classification. The process involves:

Dataset Acquisition: Downloading the Dogs vs. Cats dataset from Kaggle.
Image Preprocessing: Loading images, converting them to grayscale, resizing them to a uniform size (64x64 pixels), and flattening them into feature vectors.
Data Splitting: Dividing the preprocessed data into training and testing sets.
Model Training: Training a Linear Support Vector Classifier (SVC) on the training data.
Model Evaluation: Assessing the model's performance on the unseen test set using accuracy and a classification report.

Dataset
The dataset used is the "Dogs vs. Cats Redux: Kernels Edition" from Kaggle, available at https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition.
It consists of 25,000 training images (12,500 dogs and 12,500 cats) and 12,500 test images

How to Run the Notebook
To run this notebook in Google Colab:

Open in Colab: Click the "Open in Colab" badge (if available) or upload the .ipynb file to Google Colab.
Kaggle API Key: You will need a Kaggle API key (kaggle.json).
Go to your Kaggle account settings and click "Create New API Token" to download kaggle.json.
In the Colab environment, use the provided cells (eddafecf or a similar upload cell) to upload your kaggle.json file. The notebook will automatically move it to the correct location (~/.kaggle/) and set permissions.
Download Dataset: Run the cell that downloads and unzips the dogs-vs-cats dataset (23f03b5f or similar). This will create the necessary train and test1 directories.
Execute Cells: Run all the cells in sequence. The notebook will guide you through data loading, preprocessing, model training, and evaluation.

Results
After running all cells, the model evaluation will provide metrics such as accuracy, precision, recall, and F1-score on the test set. For example, with the current configuration (grayscale, 64x64 pixels, linear SVM), typical results might be:

Accuracy: 0.6000

Classification Report:
              precision    recall  f1-score   support

         cat       0.60      0.60      0.60      2500
         dog       0.60      0.60      0.60      2500

    accuracy                           0.60      5000
   macro avg       0.60      0.60      0.60      5000
weighted avg       0.60      0.60      0.60      5000
