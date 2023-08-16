# Malaria Detection using Deep Learning

## Objective

Develop an automate malaria detection system using Deep Learning algorithms and thus able to support the health sector by reducing the time taken, cost, the effort put in to detect malaria at present and hence, an easily adoptable solution.

## Skills/Tools Used

1. Python Programming Language
2. Deep learning

## Project Overview

**1. Data Collection :**  In this level, the required image files for the project are taken from Kaggle. The images are converted to csv files.

  - Size of the dataset : ~14000 images for healthy and infected images. 

**2. Data Preprocessing :** 

  - Greyscaling images to reduce complexity of models and elimate noise, making them faster to train and requiring less memory.

  - Resizing images to ensure uniform input size, save memory, speed up training, apply data augmentation, and match pretrained model requirements.

**3. Model Training :**

  - Used InceptionV3 Model as the Base Inception of my CNN model
  - Then added a Global Average Pooling Layer to reduce the size of the input neurons
  - Added two more Dense layers with 512 neurons and leaky_relu activation function.
  - Added a dropout layer to avoid overfitting(Dropout Regularization)
  - Finally, a prediction dense layer with sigmoid activation function.
  - Used Adam Optimizer and binary_crossentropy loss function.

**4. Model Testing :**

  - Utilised early stopping method to decide number of epochs to be used
  - Tested two kinds of activation functions: RELU, Leaky RELU
  - Achieved an accuracy of ~ 97% 
