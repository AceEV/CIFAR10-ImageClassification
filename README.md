# CIFAR-10 Dataset Image Classification

Dataset available [here](https://www.cs.toronto.edu/~kriz/cifar.html). Unpacked the dataset using the information provided on the page. After reading them once, I preprocessed the data and saved the dataset into .npy files, so that it can be read easily in the future.



### Models created

#### 1. Custom Architecture

- Achieved a training accuracy of 96% and validation accuracy of ~87% in 20 epochs
- Used Adam Optimizer

#### 2. LeNet5 Architecture

- Achieved a training accuracy and validation accuracy of ~60% in 20 epochs.
- Tried a custom version of LeNet with Dropout to slightly improve the model.
- The shallowness of the model is a bottleneck for the process.

#### 3. ResNet 34 - Transfer Learning.

- Got model architecture and weights from `qubvel`'s repository : [Classification models Zoo - Keras (and TensorFlow Keras)](https://github.com/qubvel/classification_models)

- Added a Dense layer of 10 neurons to the top of the ResNet Architecture.
- To train, 
  - Started with Adam Optimizer till the validation accuracy plateaued. 
  - Then, reduced batch size and learning rate for some further improvement.
  - Finally switched to SGD Momentum for the best results
- Got a training accuracy of 98% and validation accuracy of 87% in the best model version.





###### Note : As the .h5 weights and models files are too big to upload onR Github, they are not in the repo.
