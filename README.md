# Using Deep Learning to classify images of dogs vs cats

## Context
The goal of this project is to use deep learning to classify images of dogs vs cats. The dataset used is the Dogs vs Cats dataset from Kaggle. The dataset contains 25,000 images of dogs and cats. The dataset is split into 12,500 training images and 12,500 testing images. The dataset is available at https://www.kaggle.com/c/dogs-vs-cats/data.

## Content
Each image contains a dog or a cat.

## Work done
First, in file `01-fully_connected_layer.ipynb`, the images are loaded by calling an iterator on the dataset. Then, a fully connected layer is proposed in order to train and test the model during 30 epochs. However, after the 15th epoch, it is already clear that a fully connected layer will not suit my purposes. Hence,  I will next have to try a convolutional network, or even use an already existing model with transfer learning.

Then, in file `02_CNN_with_transfer_learning_CPU.ipynb`, I will use a pre-trained network based on ImageNet in order to make the same predictions. I will use the DenseNet121 model, which is a convolutional neural network that is 121 layers deep. I will use the pre-trained weights on ImageNet. I will then add a fully connected layer on top of the pre-trained network, and train the model on the Dogs vs Cats dataset. I will then test the model on the test set, and evaluate the performance of the model. However, since this is based on the use of my local CPU, training will take a really long time. Hence, I will next have to use Google Colab in order to speed up the training process.

Finally, in file `03_CNN_with_transfer_learning_GPU.ipynb`, I will use the same model as in the previous file, but this time I will use the GPUs available on Google Colab in order to speed up the training process. I will then test the model on the test set, and evaluate the performance of the model.