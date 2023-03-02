# Using Deep Learning to classify images of dogs vs cats

## Context
The goal of this project is to use deep learning to classify images of dogs vs cats. The dataset used is the Dogs vs Cats dataset from Kaggle. The dataset contains 25,000 images of dogs and cats. The dataset is split into 12,500 training images and 12,500 testing images. The dataset is available at https://www.kaggle.com/c/dogs-vs-cats/data.

## Content
Each image contains a dog or a cat.

## Work done
First, in file `fully_connected_layer.ipynb`, the images are loaded by calling an iterator on the dataset. Then, a fully connected layer is proposed in order to train and test the model during 30 epochs. However, after the 15th epoch, it is already clear that a fully connected layer will not suit my purposes. Hence,  I will next have to try a convolutional network, or even use an already existing model with transfer learning.