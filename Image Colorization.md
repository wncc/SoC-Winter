# Deploying an Image Colourization model
***

Image colorization is the process of taking an input grayscale (black and white) image and then producing an output colorized image that represents the semantic colors 
and tones of the input. The approach we are going to use here relies on deep learning. 

## Prequisites
- ### Python
  You'd be better off not doing this project if you don't know about Python Programming. But since you're enthusiastic, you can learn to code in Python [here](https://www.wncc-iitb.org/wiki/index.php/Python_for_Beginners).

- ### Deep Learning Library (PyTorch/Tensorflow) 
  Not sure what PyTorch is? Do [this](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html) tutorial on their website, to get to know the basics. But you need to know about Nerual Networks first. Oh here's where you can learn about NNs, just do [Week 1](https://github.com/wncc/learn-gan#week-1--getting-started) and you're good to go. Also, you need to know what Convolutional Neural Networks are, read and implement [this](https://adventuresinmachinelearning.com/convolutional-neural-networks-tutorial-in-pytorch/) to get an understanding
  
## Key Concept

Here, we will be using LAB color space, but you can try using YCbCr space also. Similar to the RGB color space, the Lab color space has three channels. But unlike the 
RGB color space, Lab encodes color information differently:
* The L channel encodes lightness intensity only
* The a channel encodes green-red.
* And the b channel encodes blue-yellow

For more information, you can refer to [This Wikipedia article](https://en.wikipedia.org/wiki/CIELAB_color_space).

Since the L channel encodes only the intensity, we can use the L channel as our grayscale input to the network.

From there the network must learn to predict the a and b channels. Given the input L channel and the predicted ab channels we can then form our final output image.

The entire (simplified) process can be summarized as:

1. Convert all training images from the RGB color space to the Lab color space.
2. Use the L channel as the input to the network and train the network to predict the ab channels.
3. Combine the input L channel with the predicted ab channels.
4. Convert the Lab image back to RGB.

## A pathway for Recolorization using Autoencoders

A very simple model can also be implemented as -

* **Download and Read 2000 Classic Painting's Dataset** - Visit [this link](https://www.kaggle.com/thedownhill/art-images-drawings-painting-sculpture-engraving) to download it from website or type the following command on terminal
```kaggle datasets download -d thedownhill/art-images-drawings-painting-sculpture-engraving```
* **Train/Test split** - Get a sample of 20 images to test the model when it is done
* **Create inception embedding of training data** - Load weights of InceptionResNetV2 and generate embedding of grayscaled image using the network
* **Create the Model** - The model can be a combination of an autoencoder and resnet classifier. The best an autoencoder can do by itself is just shade everything in a brownish tone. We can create a model which uses an resnet classifier to give the neural network an *idea* of what things should be colored

    **Encoder** - Add successive blocks of 2D convolutions with RELU activation function followed by max pooling to reduce the input
    
    **Fusion** - Concatenate encoder output with the image embedding from InceptionResNetV2 (repeated and resized) and add a 2D convolution block with RELU activation function
    
    **Decoder** - Add successive blocks of 2D convolutions with RELU activation function followed by upsampling layers to generate an image of original size
    Use **Adam** optimizer and **mean squared error** loss function for the model
* **Train the model** - Use batch size of 20 and train for atleast 25 epochs with suitable learning rate 
* **Generate results** - The output of model are the a and b channels, concatenate this with thhe L channel from original image to generate a recolorized image

Here's a [reference link](https://www.kaggle.com/abhishekbhole/image-coloring-using-autoencoders) in case you get stuck in implementing the above

### An Alternative Pathway 

You could code and train your own model quite by following [this article](https://tinyclouds.org/colorize/) on Automatic Colorization but it is bit more time taking. Implementation wise it has similar encoder network with residual connections except that it uses VGG-16 for generating embeddings and works in YUV color space.
Here's a [reference of implementation](https://github.com/pavelgonchar/colornet)

## Take a shortcut

If you want to focus on deploying the model, refer to 
[this article](https://medium.com/datadriveninvestor/coloring-black-white-images-using-deep-learning-984e6f4ddf14) to get a quick model up and running for 
image recolourization and move onto the next section. For more detailed information, please refer to original paper by [Zhang et al.](http://richzhang.github.io/colorization/).

## Deploying

Deploying your machine learning model is a key aspect of every ML project. We will now lean on the resourcefulness of Flask to help us deploy our own machine learning model

Flask is a web application framework written in Python. It has multiple modules that make it easier for a web developer to write applications without having to worry about the details like protocol management, thread management, etc.

Flask gives is a variety of choices for developing web applications and it gives us the necessary tools and libraries that allow us to build a web application.

**Install Flask** - Here, I am assuming you already have Python 3 and pip installed. To install Flask, you need to run the following command:
``` sudo apt-get install python3-flask ```

Here are some reference links so as to how to deploy an ML model on Flas which uses image as input - 
* [reference - 1](https://towardsdatascience.com/deploying-models-to-flask-fb62155ca2c4) 
* [reference - 4](https://medium.com/@jasonsalas_89883/deploying-your-machine-learning-model-and-porting-a-cool-example-a91ead6c3a7d)
* [reference - 2](https://www.analyticsvidhya.com/blog/2020/07/deploy-an-image-classification-model-using-flask/)
* [reference - 3](https://towardsdatascience.com/how-to-easily-deploy-machine-learning-models-using-flask-b95af8fe34d4)


That's it! You have implemented and deployed your own image recolorization model!
