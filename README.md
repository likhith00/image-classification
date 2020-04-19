# image-classification
Image classification involves predicting the class of object/objects in image. There are different types of classification based on class and labels. I will try to upload the various type of classification models.

[cats_and_dogs_classification.ipynb](https://github.com/likhith00/image-classification/blob/master/cats_and_dogs_classification.ipynb) is the implementation of simple classification model. The dataset used in this repo is cats and dogs with 2000 training images and 600 validation images. I've trained the model with the help of google colab and I've accessed my dataset by mounting google colab with google drive. The model performance is average with considerable accuracy but fluctuating validation loss 

## Model Flowchart

The model consists of bunch of convolution layers,maxpooling layers, activation functions,Dense layers etc
these layers are present in keras.layers

<img src="https://github.com/likhith00/image-classification/blob/master/model.png?raw=true" width="500" height="1000" />

## Model Accuracy

The train accuracy and validation accuracy plots seems to be good but with some considerable fluctuations. Initially, the validation accuracy exceeded the training accuraccy becauce the model takes random values to train itself. Later, due to the backpropagation the model learns itself and the weights get updated hence training accuracy is more than validation accuracy 

![Accuracy](/accuracy.png)

## Model Loss

The train loss decreased constantly there are no big fluctuations but there are more fluctuations in validation loss. 

![Loss](/loss.png)


## Confusion Matrix

A confusion matrix is a summary of prediction results on a classification problem. The number of correct and incorrect predictions are summarized with count values and broken down by each class. This is the key to the confusion matrix. The confusion matrix shows the ways in which your classification model is confused when it makes predictions. It gives us insight not only into the errors being made by a classifier but more importantly the types of errors that are being made.

![confusion matrix](/confusion_matrix.png)

# Accuracy

The accuracy of this model is <b>80.0</b>

To improve the accuracy of the model by changing the hyperparameters such as learning rate,batchsize,epochs etc or we can use pretrained networks and finetune our model.


