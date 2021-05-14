# Melanoma-CNN-Logistic-Regression-Models

Melanoma is a highly aggressive cancer that develops in melanocytes, the cells that produce melanin. It can also form in the eyes and, rarely, inside openings of the body such as the nose or throat. It can be detected via irregular lesion shape, size, changes over time and color. Melanoma can be harmless or lead to cancer. It is much less common than some other types of skin cancers but is more dangerous due to its potential to spread to other parts of the body if not caught and treated early. Being able to identify early-onset melanoma is crucial to dermatologists and their patients and can save thousands of lives.

The purpose of these models is to classify skin lesions as benign or cancerous.

The dataset contains 33,126 dermoscopic training images of unique benign and malignant skin lesions from over 2,000 patients. Each image is associated with one of these individuals using a unique patient identifier. All malignant diagnoses have been confirmed via histopathology, and benign diagnoses have been confirmed using either expert agreement, longitudinal follow-up, or histopathology. A thorough publication describing all features of this dataset is available in the form of a pre-print that has not yet undergone peer review. The public training dataset contains a split of 32,542 benign skin lesions and 584 malignant skin lesions. The testing set for this dataset is available on Kaggle without any labels. Due to the size of the dataset and lack of computational resources, we used 2526 images for training and 510 for testing. All malignant class images were used. The images were resized to be 100x100 using MATLAB. However, we transformed the data to be flipped both horizontally and vertically to provide enough images for the models to train later. Therefore we had a total of 7578 images for training and 1530 images for testing. Both models were run via Google Colab’s GPU.

A logistic regression was hand written, and then compared to the SciKit Learn package's LogisticRegression function.

The CNN was constructed using PyTorch and consists of two convolutional layers, followed by 4 dense layers with one layer of dropout.


## This project was completed May 2021 as a part of UNC-CH's COMP 562 Intro to Machine Learning.

## All work done by Blaine Hill, Sam Friedman, Eric Ashton, and Mattheus Bezerra
