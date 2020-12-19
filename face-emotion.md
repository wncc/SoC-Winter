# Facial Emotion Detection
In this project, you will implement a CNN model from scratch using a Deep Learning library like PyTorch/Tensorflow. The model will be trained to detect facial emotions of humans via live camera feed. 

If you don't have much experience with OpenCV or CNNs, don't worry about it, we have shared links to learn some basics about them as well.

## Prequisites
- ### Python
  You'd be better off not doing this project if you don't know about Python Programming. But since you're enthusiastic, you can learn to code in Python [here](https://www.wncc-iitb.org/wiki/index.php/Python_for_Beginners).
- ### OpenCV
  Only the basics of OpenCV would be required for this project. You can learn them [here](https://www.pyimagesearch.com/2018/07/19/opencv-tutorial-a-guide-to-learn-opencv/)
- ### Deep Learning Library (PyTorch/Tensorflow) 
  Not sure what PyTorch is? Do [this](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html) tutorial on their website, to get to know the basics. But you need to know about Nerual Networks first. Oh here's where you can learn about NNs, just do [Week 1](https://github.com/wncc/learn-gan#week-1--getting-started) and you're good to go. Also, you need to know what Convolutional Neural Networks are, read and implement [this](https://adventuresinmachinelearning.com/convolutional-neural-networks-tutorial-in-pytorch/) to get an understanding
  
## Pathway
- First we need a dataset. Download it from [here](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data?select=fer2013.tar.gz). You can use also type this in your CLI instead    
`kaggle competitions download -c challenges-in-representation-learning-facial-expression-recognition-challenge` 
- Split the data into *training* and *validation* sets, this is can be done in a ratio of about 10:1 or less
- Now augment the image data using Pytorch. Learn it [here](https://pytorch.org/docs/stable/torchvision/transforms.html)
- Now, code a CNN model, based on what you learnt from the link in prerequisites. A block would contain a Conv2D layer, Activation layer, BatchNorm, MaxPool, Dropout(optional). Create several such blocks (with successive blocks having double filters in Conv2D layer). Finally include a Flatten Layer, Dense layer, Activation layer. This, of course, is just a blueprint to give you direction. We'd encourage to try out different parameters and tinker around with the model to get some more practical knowledge. 
- Now come the standard training, testing, and hyperparameter training. After this, you can save the model to be used to create the emotion detector.
- Now we'll detect faces using OpenCV. It's pretty simple actually. Read up on Haar Cascade classifier [here](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html), it's based on the famous Viola-Jones algorithm. You can use this directly in OpenCV to detect faces in livestream.
- Select the RoI and use your model to classify the expression. You can make a bounding box and put text on it as well.
- Done!
