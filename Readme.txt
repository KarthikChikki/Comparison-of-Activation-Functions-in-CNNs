Comparison of Activation Functions in CNNs

Overview:
This project evaluates the performance of three activation functions—Sigmoid, Tanh, and ReLU—in a Convolutional Neural Network (CNN) for satellite image classification. The study aims to analyze how different activation functions affect model accuracy, convergence speed, and loss reduction.

Dataset:
The dataset is obtained from Kaggle and consists of four classes:
- Cloudy (1500 images)
- Desert (1131 images)
- Green Area (1500 images)
- Water (1500 images)

Images are resized to 75x75 pixels, normalized, and split into training and testing sets.

Model Architecture:
Three CNN models are implemented with identical architectures but different activation functions (Sigmoid, Tanh, and ReLU). Each model consists of:

- Three convolutional layers (32, 64, and 128 filters)
- Max pooling layers
- Dense layers with 128 neurons
- A final output layer with softmax activation

Results:
Tanh outperforms ReLU and Sigmoid, achieving the highest accuracy and lowest loss. ReLU performs well but has fluctuations due to dying neurons. Sigmoid struggles with vanishing gradients, leading to slower learning.

Usage:
Clone the repository and run the notebook to experiment with different activation functions.