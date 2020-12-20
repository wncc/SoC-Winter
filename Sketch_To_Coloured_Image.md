# Sketch to Coloured Image using Conditional Adversarial Network

![Sketch to Coloured Image](https://miro.medium.com/max/2400/1*sOHB4IYP-a1T2qBcZCoPow.jpeg)

<hr>

## Prerequisites

### Python 

Python programming language is necessary for this project. If you have a grip over any other programming language, it wouldnt take much time to learn Python. You can follow this [tutorial](https://github.com/wncc/learners-space/tree/master/Python) .

###  Tensorflow

It is preferred that you have used a deep learning framework in the past especially tensorflow. We will write the code for the project in Tensorflow but this is not a hard prerequisite. Follow this [official documentation](https://www.tensorflow.org/api_docs/python/tf/all_symbols) of tensorflow as a reference throughout the project.

### Deep Learning

It is preferred that you are familiar with deep learning concepts such as Neural networks, Loss functions, Optimizers, Backpropogation, etc but not hard prerequisites. Follow these articles to understand some key concepts that you will need for the project.

Convolutional Neural Networks - [article 1](https://medium.com/@RaghavPrabhu/understanding-of-convolutional-neural-network-cnn-deep-learning-99760835f148) [article 2](https://adeshpande3.github.io/adeshpande3.github.io/A-Beginner's-Guide-To-Understanding-Convolutional-Neural-Networks/) [article 3](https://medium.com/datadriveninvestor/convolutional-neural-network-cnn-simplified-ecafd4ee52c5)

More on CNN - [article](https://stanford.edu/~shervine/teaching/cs-230/cheatsheet-convolutional-neural-networks)

Loss Functions - [article](https://towardsdatascience.com/understanding-different-loss-functions-for-neural-networks-dd1ed0274718)

Backpropogation - [article](https://medium.com/@pavisj/convolutions-and-backpropagations-46026a8f5d2c)

Normalization - [article](https://medium.com/techspace-usict/normalization-techniques-in-deep-neural-networks-9121bf100d8)

Generative Adversarial Networks - [paper](https://arxiv.org/pdf/1406.2661.pdf) [article](https://machinelearningmastery.com/what-are-generative-adversarial-networks-gans/)


<hr>

## Procedure

- Go through all the articles mentioned in the prerequisites (3 days)

- Read and understand this [paper](https://arxiv.org/pdf/1611.07004.pdf) completely since the project is based on implementation of this paper (2 days)

- Set up Microsoft Azure ML Workspace and start using Notebooks. Sign up/in using LDAP ID and start using your free credits for this project. Make a new ML workspace and start a new notebook. You have to use Tesla K80 (GPU) for compute. You will have to upload the kaggle dataset either by using API or manual download and upload.( 1 day)

- Implement the model as per this [article](https://towardsdatascience.com/generative-adversarial-networks-gans-89ef35a60b69). Follow each step carefully and understand the concepts while you write the code. You may change the size of dataset and number of epochs since GANs take alot of time for training (2 days)

- Train the model. You can try your own variations for lambda value and beta values in loss functions and optimizers. You can also change batch size or number of epochs, maybe manipulate the architecture a bit and compare the results. (4 days)

- That's it. Test the model and get some amazing outputs.

<hr>

## Some General Points

- Understand the paper and the algorithm involved before implementing the model by code.
- Refer the Tensorflow documentation extensively for importing dataset, pre-processing, and model training.
- Use Google and Stackoverflow extensively for all the little errors you get during coding. If you are not able to get a solution, ask your mentor.
- Try to have stable internet connection throughout the project from importing the dataset to training and testing. Save the checkpoints while training (most important). Procedure for this is mentioned in the article shared.

<hr>

<h3 align="center"> Happy Coding !</h3>
