# DROWSINESS DETECTOR<br>
### Sub Project of:- `Driver Drowsiness Detection System`

In this Python project, we will be using OpenCV for gathering the images from webcam and feed them into a Deep Learning model which will classify whether the person’s eyes are ‘Open’ or ‘Closed’. The approach we will be using for this Python project is as follows :<br>
Step 1 – Take image as input from webcam.<br>
Step 2 – Detect the face in the image and create a Region of Interest (ROI).<br>
Step 3 – Detect the eyes from ROI and feed it to the classifier.<br>
Step 4 – Classifier will categorize whether eyes are open or closed.<br>
Step 5 – Calculate score to check whether the person is drowsy.<br>

## The Dataset
The dataset used for this model is created by us. To create the dataset, we wrote a script that captures eyes from a camera and stores in our local disk. We separated them into their respective labels ‘Open’ or ‘Closed’. The data was manually cleaned by removing the unwanted images which were not necessary for building the model. The data comprises around 7000 images of people’s eyes under different lighting conditions. After training the model on our dataset, we have attached the final weights and model architecture file `models/cnnCat2.h5`.<br>
Now, you can use this model to classify if a person’s eye is open or closed.

## The Model Architecture

The model we used is built with Keras using **Convolutional Neural Networks (CNN)**. A convolutional neural network is a special type of deep neural network which performs extremely well for image classification purposes. A CNN basically consists of an input layer, an output layer and a hidden layer which can have multiple numbers of layers. A convolution operation is performed on these layers using a filter that performs 2D matrix multiplication on the layer and filter.
The CNN model architecture consists of the following layers:<br>
•	Convolutional layer; 32 nodes, kernel size 3<br>
•	Convolutional layer; 32 nodes, kernel size 3<br>
•	Convolutional layer; 64 nodes, kernel size 3<br>
•	Fully connected layer; 128 nodes<br>

## Prerequisites
The requirement for this Python project is a webcam through which we will capture images. You need to have Python (3.6 version recommended) installed on your system, then using pip, you can install the necessary packages.<br>
1.	OpenCV – pip install opencv-python (face and eye detection).<br>
2.	TensorFlow – pip install tensorflow (keras uses TensorFlow as backend).<br>
3.	Keras – pip install keras (to build our classification model).<br>
4.	Pygame – pip install pygame (to play alarm sound).<br>
