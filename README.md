# Building multi-class-image-classification models using CNN in Keras

_Keywords_ - Convolutional Neural Networks, Multi-class image classification, precision, recall, accuracy, F-1 score, confusion matrix, cross-validation 

**Why is multi-class image classification important?**

1. Object Recognition - recognize and categorize objects within images, allowing systems to understand and respond to diverse visual content.
2. Medical Diagnosis - for diagnosing diseases or conditions based on visual data such as X-rays, MRIs, or pathology slides.
3. Retail and E-commerce - to categorize products, making it easier for users to search, browse, and find relevant items. It also enables automated product tagging and recommendation systems.
4. Human-Computer Interaction - enabling systems to understand and respond to gestures, facial expressions, or objects in images or video streams. 

## Flower Species Recognition
This project aims at testing two Convolutional Neural Networks (CNN) for recognizing different flower species based on images. <br>
The models are trained to classify images into specific flower categories. <br>

## Data 
This data has been taken from aiplane.com - https://aiplanet.com/challenges/61/data-sprint-25-flower-recognition-61/overview/about <br>
The dataset consists of images of 5 flower species, and the model aims to predict the correct flower category for a given image. <br>
The train, test and validation data could be found here - https://pitt-my.sharepoint.com/:f:/g/personal/yak39_pitt_edu/EotbgAlZtOpOkPUxuyLVcDUBmZnLiKGu3pr9zqBReZSbaw?e=rUGIkz <br>
Each folder contains 5 folders corresponding to each flower species. <br>

## Method 
We first build a simple Sequential CNN model with convolutional layers for feature extraction, max pooling layers for down-sampling, a flatten layer for reshaping, and fully connected layers for classification. The model is compiled with the Adam optimizer, categorical crossentropy loss, and accuracy as the evaluation metric. <br>
We then add complexity to this model by adding dense layers followed by dropout layers with a dropout rate of 0.5 for regularization and improved generalization. <br>

## Result 
1. Though our validation accuracy increased from 65% to 70%, inreasing complexity of the model does not always help in better learning. 
2. We tested various ranges of hyperparameters like number of epochs (5,10,15,20) and learning rate (0.1, 0.001, 0.0001) and went ahead with choices optimized for maximum accuracy and precision. 
3. Having more data would be useful here (not always the case) as our train set, test set and validation set has only 2193, 277 and 276 images, repsectively. 


