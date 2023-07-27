# Digit Recognition in Real-Time from Canvas

This application is for real-time digit recognition using neural networks in Python. It allows you to draw a digit on a canvas using your mouse and see the predictions made by two different models in real-time: one is a neural network trained from scratch using Keras, and the other is a Convolutional Neural Network (CNN) trained using PyTorch. Both was trained using MNIST dataset.

## Prerequisites

Before running the application, make sure you have the following installed:

- Python (version 3.x)
- Pygame library (pygame)
- Keras library (keras)
- NumPy library (numpy)
- OpenCV library (cv2)
- Matplotlib library (matplotlib)
- PyTorch library (torch)

You can install these dependencies using `pip`:

```bash
pip install pygame keras numpy opencv-python matplotlib torch
```

## Getting Started

To use the digit recognition application, follow these steps:

1. Clone the repository to your local machine.

```bash
git clone https://github.com/RayaneKimo/Real_time_digits_recognition.git
```

2. Change directory to the project folder.

```bash
cd Real_time_digits_recognition
```

3. Run the `CNN_NN_digits_recognition.py` script to start the application.

```bash
python CNN_NN_digits_recognition.py
```

## Usage

Once the application is running, a window will open with a canvas on the left side and prediction results on the right side. You can draw a digit on the canvas using the left mouse button, and the models will make real-time predictions.
![image](https://user-images.githubusercontent.com/85368764/200424334-c53a445f-2b48-4f41-b4aa-88aea39aa309.png)


### Drawing

- Left mouse button: Draw in white color (represents the digit).
- Right mouse button: Draw in black color (eraser).

### Keyboard Shortcuts

- Press 'r': Clear the canvas to start drawing a new digit.

### Prediction

- The predictions for each model will be displayed on the right side of the window:
  - "NN": Prediction result from the neural network (Model 1).
  - "CNN": Prediction result from the Convolutional Neural Network (Model 2).

## Models

Both models, Model 1 (neural network) and Model 2 (CNN), are pretrained and loaded during the initialization of the application.

### Model 1 (Neural Network)

The neural network model used in this application was trained and loaded using Keras. You can load yours. Just respect the input data as images of a flat shape (784).

### Model 2 (Convolutional Neural Network - CNN)

Model 2 is a Convolutional Neural Network (CNN) trained using PyTorch. The weights of Model 2 are loaded from the file "mnist_classifier_model.pth". If you want to know more about the training process or the architecture of Model 2, please refer to the code provided in this repository.

## Customization

If you want to experiment with different models, you can replace the pretrained models with your own models. Ensure that the models have the appropriate architecture for digit recognition.

## Contributions

Feel free to open an issue or submit a pull request. Contributions are welcome!


