# RealTimeGenderDetection

This is a real-time gender detection program built with Python and OpenCV. It uses a convolutional neural network (CNN) to classify the gender of a person as male or female in real-time video streams.

## Model Architecture

The model architecture is as follows:

Conv2D(filters=4, kernel_size=(3,3), padding="same", activation="relu"), # 4 224 224
BatchNormalization(),
MaxPool2D((2,2)), # 4 112 112
Dropout(0.2),

Conv2D(filters=8, kernel_size=(3,3), padding="same", activation="relu"), # 8 112 112
BatchNormalization(),
MaxPool2D((2,2)), # 18 56 56
Dropout(0.2),

Conv2D(filters=16, kernel_size=(3,3), padding="same", activation="relu"), # 16 56 56
BatchNormalization(),
MaxPool2D((2,2)), # 16 28 28
Dropout(0.2),

Conv2D(filters=32, kernel_size=(3,3), padding="same", activation="relu"), # 32 56 56
BatchNormalization(),
MaxPool2D((2,2)), # 132 28 28
Dropout(0.2),

Conv2D(filters=64, kernel_size=(3,3), padding="same", activation="relu"), # 64 56 56
BatchNormalization(),
MaxPool2D((2,2)), # 64 28 28
Dropout(0.2),

Flatten(),

Dense(128, activation="relu"),
BatchNormalization(),
Dropout(0.2),

Dense(10, activation="relu"),
BatchNormalization(),
Dropout(0.2),

Dense(2, activation="sigmoid")


## Accuracy

The model achieved an accuracy of 95.20%.

## Dependencies

This program requires the following dependencies:

* OpenCV
* TensorFlow
* NumPy

## How to Use

To use this program, first clone this repository to your local machine. Then, install the dependencies listed above.

To run the program, execute the following command:

`
