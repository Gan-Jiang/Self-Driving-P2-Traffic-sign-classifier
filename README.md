## Project: Build a Traffic Sign Recognition Program
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Overview
---
In this project, I use convolutional neural networks to classify traffic signs in the [German Traffic Sign Dataset](http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset). After the model is trained, I try out the model on some images of traffic signs that I find on the web. This is the second project of udacity self-driving car engineer nanodegree. The codes are in Traffic_Sign_Classifier.ipynb. 

### What I did 
---
The steps of this project are the following:
* Load the data set. The data are preprocessed into training data and test data. There are 39209 training examples and 12630 testing examples. 
* Explore and visualize the data set. I conduct a histgram of the labels in the training set and test set. I find that the distributions in the training set and test set are not the same. 
* Preprocess the data so that it has zero mean and the same variance.  Then, I do train-validation split, and generate additional data by rotate the images in the training dataset by [-15, 15] degrees. The size of the training dataset is trippled. 
* Implement a 5 layer neural network with first 2 layer convolutional layers. 
* Use the model to make predictions on 5 new images online. 

### Dependencies
This lab requires:

* [CarND Term1 Starter Kit](https://github.com/udacity/CarND-Term1-Starter-Kit)

The lab environment can be created with CarND Term1 Starter Kit. Click [here](https://github.com/udacity/CarND-Term1-Starter-Kit/blob/master/README.md) for the details.

### Dataset and Repository

1. Download the data set. The classroom has a link to the data set in the "Project Instructions" content. This is a pickled dataset in which we've already resized the images to 32x32. It contains a training, validation and test set.
2. Clone the project, which contains the Ipython notebook and the writeup template.
```sh
git clone https://github.com/udacity/CarND-Traffic-Sign-Classifier-Project
cd CarND-Traffic-Sign-Classifier-Project
jupyter notebook Traffic_Sign_Classifier.ipynb
```
