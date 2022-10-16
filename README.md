# DATASET 

AUTHOR: Julien de la Bruère-Terreault (drgfreeman@tuta.io)

LICENSE: CC-BY-SA 4.0

DESCRIPTION: This dataset contains images of hand gestures from the Rock-Paper-Scissors game. The images were captured as part of a hobby project where I developped a Rock-Paper-Scissors game using computer vision and machine learning on the Raspberry Pi (https://github.com/DrGFreeman/rps-cv)

CONTENTS: The dataset contains a total of 2188 images corresponding to the 'Rock' (726 images), 'Paper' (710 images) and 'Scissors' (752 images) hand gestures of the Rock-Paper-Scissors game. All image are taken on a green background with relatively consistent ligithing and white balance.

FORMAT: All images are RGB images of 300 pixels wide by 200 pixels high in .png format. The images are separated in three sub-folders named 'rock', 'paper' and 'scissors' according to their respective class.

# CODE

AUTHOR: Regina Aprilia Roberto

PURPOSE: trial in studying machine learning for beginner

FORMAT: .ipynb

DESCRIPTION: machine that can predict uploaded image based on dataset, non-binary, categorical which contain 'rock', 'paper' and 'scissor' as a data train and val for prediction.

SUGGESTIONS: 
- for file zipping: 
!unzip “path dataset” atau !unzip file_location.zip
- for data augmentation: 
use data test augmentation instead of validation data with validation_datagen = ImageDataGenerator(rescale=1./255)
- for callback and val accuracy: 
use more higher treshold for example if(logs.get('accuracy')>0.98 and logs.get('val_accuracy')>0.98)
- use dropout to avoid overfitting
- add more variable data image with variative background or use pretrained model and 'Transfer Learning' or 'Remove Image Background'
- use confusion matrix and classification report to evaluate model
- to improve accuracy and validation accuracy, try Transfer Learning with 'VGG16', 'RestNet', 'AlexNet'.
- use Handle Imbalance when facing imbalance dataset
- learn the model that have been created by trying to analyze is it goodfit, overfit or underfit.

REFERENCES:
- https://keras.io/api/callbacks/
- https://learnopencv.com/playing-rock-paper-scissors-with-ai/
- https://machinelearningknowledge.ai/image-segmentation-in-python-opencv/
- https://machinelearningmastery.com/dropout-regularization-deep-learning-models-keras/
- https://machinelearningmastery.com/padding-and-stride-for-convolutional-neural-networks/
