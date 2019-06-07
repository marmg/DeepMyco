_____________________
# DeepMyco
## Deep Learning applied to micology
_____________________

Final degree project of Marcos Martinez Galindo.

### Abstract

One of the greatest enchanment of the county of Teruel is its micologycal diversity, which thousands of people take advantage of every year. But not everyone knows to distinguish the different species of mushrooms, something really difficult. Because of that, the idea of a mobile application that recognizes the specie just with a photo is very interesting.

The neural networks are gaining a lot of limelight in the industry given its great capacity to learn to recognize patterns in data. One of the areas where this kind of algorithms are used is in computer vision, area increasingly in use and in evolution. One of the main functions is object recognition in images, or image classification. With just the image, the neural network is able to recognize the objects in it, if it has been well trained. However, to train well a neural network to recognize objects is not an easy task.

This, attached to the difficulty of differentiate with a naked eye a mushroom, makes of mushroom recognition in images with neural networks a considerable challenge. In this project, it has been done an essay of the main data centers, of the functionality of this algorithms and the performance of some of the different pretrained algorithms of the market. With that, it has been developed a model with 82\% of accuracy, differentiating between 7 species of the county of Teruel, which has been embedded in a mobile application developed for that.

### Keywords
Neural networks, Deep Learning, Transfer Learning, Mushroom recognition, Mushroom, Micology.

# Preprocess data

Code to preprocess images. It contains:
- COCO Annotation reader
- DataFrame creation
- Getting images from directory
- Resize images
- Data Augmentation
- Creation of numpy arrays (X_train, X_test, y_train, y_test)

# Building a neural network

## Building a neural network from scratch

## Building a neural network model with Sklearn

## Building a neural network model with Keras

# Transfer Learning

## MobilenetV2

## ResNet50

## InceptionV3

## VGG19

__________________

# Mobile app
