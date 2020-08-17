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


# Transfer Learning
Transfer Learning based on different pre-trained nets will be done. All of them will be used with the ImageNet pre-trained weights and the same classifier will be added to be able to comapre them. 

The classifier will have one Dense layer of 256 neurons and "tanh" as activation. One Flatten Layer if needed and 3 Dense Layer with 100 neurons each and "tanh" as activation. Finally, one Dense with 7 neurones and softmax to classify. It will use "adam" as optimizer and "categorical_crossentropy" as loss function.

Only the final classifier will be trained due to the lack of resources and time (Intel i7-5500U 2-Core @3.00GHz). All of them will be trained since 5 epochs.

Results (radius of circle = size of model file):

![](images/comparision.png?raw=true)

## MobilenetV2
***Notebook: Notebooks/TransferLearningMobilenetV2.ipynb***

[Link to notebook](./Notebooks/TransferLearningMobilenetV2.ipynb)

Confussion Matrix:

![](images/matriz-mobilenet.png?raw=true)

## ResNet50
***Notebook: Notebooks/TransferLearningResNet50.ipynb***

[Link to notebook](./Notebooks/TransferLearningResNet.ipynb)

Confussion Matrix:

![](images/matriz-resnet.png?raw=true)

## InceptionV3
***Notebook: Notebooks/TransferLearningInceptionV3.ipynb***

[Link to notebook](./Notebooks/TransferLearningInceptionV3.ipynb)

Confussion Matrix:

![](images/matriz-inception.png?raw=true)

## VGG19
***Notebook: Notebooks/TransferLearningVGG19.ipynb***

[Link to notebook](./Notebooks/TransferLearningVGG19.ipynb)

Confussion Matrix:

![](images/matriz-vgg.png?raw=true)

__________________

# Mobile app
