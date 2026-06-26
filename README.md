Intel Image Classification using Convolutional Neural Network (CNN)

Project Overview


This project implements a Convolutional Neural Network (CNN) to classify natural scene images from the Intel Image Classification Dataset into six different categories. The model is trained using TensorFlow/Keras and evaluated on unseen test images to measure its performance.

Dataset

The Intel Image Classification dataset contains images belonging to the following six classes:

🏢 Buildings
🌲 Forest
❄️ Glacier
⛰️ Mountain
🌊 Sea
🛣️ Street

The images are resized before training and normalized for better model performance.

Project Objectives
Build a CNN model for image classification.
Train the model on the Intel Image Classification dataset.
Evaluate model performance using accuracy and loss.
Predict unseen images.
Visualize sample predictions with actual and predicted labels.
Technologies Used
Python
TensorFlow / Keras
NumPy
Matplotlib
OpenCV
Scikit-learn
Google Colab / Jupyter Notebook
CNN Architecture

The model consists of:

Convolutional Layers (Conv2D)
Max Pooling Layers
Flatten Layer
Dense (Fully Connected) Layers
Dropout Layer
Softmax Output Layer
Data Preprocessing
Image resizing
Image normalization (rescale = 1/255)
Data augmentation:
Rotation
Zoom
Width Shift
Height Shift
Horizontal Flip
Model Training

The model is trained using:

Optimizer: Adam
Loss Function: Categorical Crossentropy
Evaluation Metric: Accuracy
Epochs: (Specify your value, e.g., 20 or 25)
Batch Size: (Specify your value, e.g., 32)
Results

The trained CNN successfully classifies images into six scene categories.

Example prediction results:

Predicted	Actual
Sea	Sea ✅
Mountain	Mountain ✅
Glacier	Glacier ✅
Buildings	Buildings ✅
Sea	Mountain ❌
Sea	Street ❌
Buildings	Glacier ❌

The model correctly classified most test images while making a few misclassifications due to visual similarities between classes.
