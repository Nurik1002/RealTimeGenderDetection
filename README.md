# Real-Time Gender Detection

Real-Time Gender Detection is a project that uses computer vision techniques to detect the gender of a person in real-time. The project uses a Convolutional Neural Network (CNN) to detect gender with an accuracy of 0.9520.

# Features

Real-time detection of gender in video streams or from a webcam 

Built using OpenCV, Keras, and TensorFlow

Easy to use and integrate with other projects

CNN model architecture for gender detection

# Model Architecture
The model architecture used for gender detection is a CNN that consists of the following layers:

- Conv2D layer with 4 filters of size 3x3, padding "same", and ReLU activation
- BatchNormalization layer
- MaxPool2D layer with pool size of 2x2
- Dropout layer with 0.2 probability
- Conv2D layer with 8 filters of size 3x3, padding "same", and ReLU activation
- BatchNormalization layer
- MaxPool2D layer with pool size of 2x2
- Dropout layer with 0.2 probability
- Conv2D layer with 16 filters of size 3x3, padding "same", and ReLU activation
- BatchNormalization layer
- MaxPool2D layer with pool size of 2x2
- Dropout layer with 0.2 probability
- Conv2D layer with 32 filters of size 3x3, padding "same", and ReLU activation
- BatchNormalization layer
- MaxPool2D layer with pool size of 2x2
- Dropout layer with 0.2 probability
- Conv2D layer with 64 filters of size 3x3, padding "same", and ReLU activation
- BatchNormalization layer
- MaxPool2D layer with pool size of 2x2
- Dropout layer with 0.2 probability
- Flatten layer
- Dense layer with 128 units and ReLU activation
- BatchNormalization layer
- Dropout layer with 0.2 probability
- Dense layer with 10 units and ReLU activation
- BatchNormalization layer
- Dropout layer with 0.2 probability
- Dense layer with 2 units and sigmoid activation for binary classification (male vs. female)
# Installation
Clone the repository:  `git clone https://github.com/Nurik1002/RealTimeGenderDetection.git`

Navigate to the project directory: `cd RealTimeGenderDetection`

Install the dependencies: `pip install -r requirements.txt`

# Usage
To detect gender in real-time from a webcam:

`python detect_gender_video.py`

To detect gender in real-time from a video stream:

`python detect_gender_video.py --stream <stream_url>`

In the template above, be sure to replace <stream_url> with the actual URL of the video stream you want to use.
