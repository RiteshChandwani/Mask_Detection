# Mask_Detection
Face Mask Detection using Python, Keras, OpenCV

Link to Dataset

https://www.kaggle.com/prithwirajmitra/covid-face-mask-detection-dataset

Import Statements -
Sequential is a prebuild Keras model where you can add layers.
Conv2D layer is used to extract the features from the image. Convolution helps with the sharpening face detection and other operation that can help the machine to learn specific characteristics of an image.
Max Pooling 2D layers helps to reduce the size of the data or we can say it reduces image dimensionality without importing features or patterns.
Dropout layer is to to reduce overfitting.
Flatten layer it transforms two dimensional matrix of features into a vector that can be fed into fully connected to neural network classifier. So that means converting data into one dimensional array for inputting into next layer. So we flatten the output of convolution layer to create a single long feature.
Dense layer is a classic fully connected neural network layer where each input node is connected to each output node.
To compile the model we will need an optimizer, so we had used 'adam' optimizer.
The image data generator class is used for augmentation purpose. So augmentation is one useful technique in building CNN that can increase the size of training set without acquiring new images. So the idea over here is very simple, just duplicate images with some kind of variation so model can learn from more examples.Overview Structure of 

Directories -
The New Masks Dataset contains 4 directories out of which 3 are from the original dataset on Kaggle, the 4th directory Static Images was created later which contains 2 images randomly downloaded from the Internet to check if our model can accurately make the right prediction or not.

The three folders inlude -

Train
Validation
Test
Each of these three folders have sub-folders - Mask and Non Mask.
