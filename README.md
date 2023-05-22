Readme
This repository contains code for a handwritten digit classifier using the MNIST dataset. The classifier is built using the Support Vector Machine (SVM) algorithm from the scikit-learn library and is deployed with a graphical interface using Gradio.

Prerequisites
To run this code, you need the following dependencies:

Python 3.x
NumPy
scikit-learn
TensorFlow
Keras
Gradio
You can install the required dependencies by running the following command:

Copy code
pip install numpy scikit-learn tensorflow keras gradio
Dataset
The code uses the MNIST dataset, which is a collection of 60,000 training images and 10,000 testing images of handwritten digits (0-9). The dataset is automatically downloaded and loaded using the Keras library.

Training and Classification
The code preprocesses the data by reshaping the images into a flat vector of size 784 and normalizing the pixel values between 0 and 1. It then trains an SVM classifier using the training data.

After training, the code predicts the labels for the test images and calculates the accuracy of the classifier using the accuracy_score function from scikit-learn.

Classification Interface
The code provides a graphical interface using Gradio, allowing users to draw a digit on a sketchpad and classify it using the trained SVM classifier. The classify_digit function takes an image as input, reshapes and normalizes it, and returns the predicted digit as an integer.

To launch the interface, run the script and a browser window will open. You can draw a digit on the sketchpad and click "Submit" to classify it. For better accuracy, draw the digit in the center of the sketchpad.

Usage
To run the code, execute the following command:

Copy code
The interface will be launched in a browser window, and you can start drawing digits to classify.

