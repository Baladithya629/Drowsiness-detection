# Eye State Detection using Convolutional Neural Networks

This project focuses on detecting whether eyes are open or closed using Convolutional Neural Networks (CNNs). It utilizes the TensorFlow and Keras libraries for model development and training.

## Dataset

The dataset consists of images of eyes categorized into two classes: "Opened" and "Closed." Each image has a resolution of 256x256 pixels with RGB color channels. The dataset is split into training, validation, and testing sets as follows:

- Training: 70%
- Validation: 20%
- Testing: 10%

## Model Architecture

The CNN model architecture is designed as follows:

- Input Layer: Conv2D with ReLU activation (16 filters, 3x3 kernel size)
- MaxPooling2D Layer
- Conv2D with ReLU activation (32 filters, 3x3 kernel size)
- MaxPooling2D Layer
- Conv2D with ReLU activation (16 filters, 3x3 kernel size)
- MaxPooling2D Layer
- Flatten Layer
- Dense Layer with ReLU activation (256 units)
- Output Layer with Sigmoid activation (1 unit)

The model is compiled using the Adam optimizer and Binary Crossentropy loss function.

## Training

The model is trained for 10 epochs on the training data with validation performed on the validation set. Training progress is logged using TensorBoard for visualization.

## Evaluation

Evaluation metrics such as precision, recall, and accuracy are computed on the test data to assess model performance.

## Results

The model achieves the following performance metrics on the test data:

- Precision: 1.0
- Recall: 1.0
- Accuracy: 1.0

Additionally, sample predictions are provided for the first four images in the test batch, showcasing the model's ability to predict eye states.

## How to Use

To use this project:

1. Clone the repository.
2. Ensure you have TensorFlow and other dependencies installed.
3. Run the provided code scripts for training and evaluation.
4. Customize the model architecture or training parameters as needed for your application.
