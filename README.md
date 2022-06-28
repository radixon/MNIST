# MNIST
The MNIST database of handwritten digits, has a training set of 60,000 examples, and a test set of 10,000 examples.  Which is a subset of a larger set available from NIST.  The digits have been size-normalized and centered in a fixed-size image.<br /> <br />

The MNIST dataset is a preprocessed and cleaned dataset.  The dataset used was made available by PyTorch.  This can be found here: https://pytorch.org/vision/main/generated/torchvision.datasets.MNIST.html <br /> <br />

## Convolutional Neural Network
The goal is to accurately identify handwritten digits.  Due to the grid-like topology of the images, the CNN was the algorithm chosen for optimal results. <br /> <br />

Five Epochs were used to attain ~95% accuracy on the training set, which resulted in ~94% accuracy on the test set. <br />

## Choices Made
### Training Parameters
..* Batch size is the number of samples processed before the model is updated.
..* dropout_p will be used in the torch.nn.Dropout2d() module. p is the probability of an element to be zero-ed.[6]
..* color_scale is used as an input channel for the first convolutional layer. The images are gray scale, so the value is 1. If the images were RGB, then the value would be 3.

### Build & Initialize Model
..* kernel_size sets the size of the filter. A kernel_size of 5 sets the filter to 25x25

# Chapter Nine of Deep Learning by Ian Goodfellow and Yoshua Bengio and Aaron Courville was used as a reference to develop the model.

# PyTorch documentation was used to properly build the model using PyTorch
