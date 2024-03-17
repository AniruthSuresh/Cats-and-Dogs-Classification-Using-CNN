# Cats-and-Dogs-Classification-Using-CNN

- **Objective**:
  - The objective here is to effectively classify images of dogs and cats.

- **Dataset**:
  - We utilized the very famous Kaggle-Microsoft dataset of dogs and cats.
  - All images were scaled to the size of 60 x 60 pixels.
  - The dataset was shuffled to prevent the model from memorizing and encourage understanding.

- **Model Selection**:
  - Due to the dataset's size and the aim for maximum accuracy, **Convolutional Neural Networks (CNNs)** were chosen over Artificial Neural Networks (ANNs).
  - Various models were trained, considering different configurations of dense layers, layer sizes, and convolutional layers.
  - Dense layer options: [0, 1, 2]
  - Layer sizes options: [32, 64, 128]
  - Convolutional layer options: [1, 2, 3]
  - 27 models were tested, and their performance was evaluated using **Tensorboard**.

- **Best Model**:
  - The model with **0 dense layers, a layer size of 64, and 3 convolutional layers** emerged as the best fit for our dataset.

- **Convolutional Network**:
  1. We constructed a sequential model with the following components:
     - Convolutional layer with a kernel size of (3,3) and 64 filters.
     - Max pooling layer to improve feature mapping and reduce data size.
  2. No dense layers were added, as the model performed best with 0 dense layers.
  3. The output layer utilized a **sigmoid** activation function with 1 unit for binary classification.

- **Performance**:
  - The model achieved the following metrics:
    - Accuracy: 0.7960
    - Loss: 0.4365
    - Validation Accuracy: 0.7820
    - Validation Loss: 0.4660

This implementation demonstrates effective classification of cats and dogs using Convolutional Neural Networks.
