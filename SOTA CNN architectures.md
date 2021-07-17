# A Deep Dive into CNNs
***

### 1 | Getting Started

- To get a basic understanding what a Neural Network is, watch this excellent playlist by [3Blue1Brown](https://www.youtube.com/channel/UCYO_jab_esuFRV4b17AJtAw) - [Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi). 

- Now, to build your own Neural Network, try completing this short course by Andrew NG - [Neural Networks and Deep Learning](https://www.coursera.org/learn/neural-networks-deep-learning?specialization=deep-learning). You can opt for Financial aid, if you need to.

- It is sometimes overwhelming to visualise how a neural network improves its performance over time. This website will allow you to do just the same - [Neural Network Playground](https://playground.tensorflow.org/).   
P.S. - You might come across new terms here. Instead of just overlooking them, try finding out what they mean. You could google them or just visit our [Wiki](https://www.wncc-iitb.org/wiki/) page on [Deep Learning](https://www.wncc-iitb.org/wiki/index.php/Deep_Learning).

- Exhausted by all the math? Here's an article to get you motivativated - [Applications of CNNs](https://machinelearningmastery.com/applications-of-deep-learning-for-computer-vision/).


### 2 | Learning Pytorch

- Libraries like PyTorch and Tensorflow make implementing neural nets a bliss. PyTorch's [60 Minute Blitz](https://pytorch.org/tutorials/beginner/deep_learning_60min_blitz.html) will help you get started. It's recommended that you type your own code as well.

- Hopefully you would have got a clear understanding of what a neural network is. It is now time to tinker around with them to decrease training time, and improve accuracy. Do this course on [Hyperparameter Tuning](https://www.coursera.org/learn/deep-neural-network?specialization=deep-learning) to know more. You can skip the TensorFlow part if you wish to, since you already got an idea of PyTorch.

- You can now do further PyTorch [tutorials](https://pytorch.org/tutorials/beginner/pytorch_with_examples.html). The above course would help you understand these examples better. Make your own [Google Colab](https://colab.research.google.com/) notebooks and tinker around. It's important to try out various values of hyperparameters for better practical learning.


### 3 | Attempting a Kaggle Challenge

- [MNIST](http://yann.lecun.com/exdb/mnist/) dataset is a large database of handwritten digits. Pytorch has a [tutorial](https://pytorch.org/tutorials/beginner/nn_tutorial.html) to train your NN on the MNIST dataset. You can leave the [CNN](https://pytorch.org/tutorials/beginner/nn_tutorial.html#switch-to-cnn) part for now.

- Kaggle is a community of data scientists where you can find a vast variety of datasets and competitions to hone your skills. Try attempting this Kaggle Challenge to get started - [Digit Recognizer](https://www.kaggle.com/c/digit-recognizer).

### 4 | CNNs

- Convolutional Neural Networks have been considered revolutionary in processing images. Read either of these articles to get an understanding of how they work - 
	+ [CNN in PyTorch](https://adventuresinmachinelearning.com/convolutional-neural-networks-tutorial-in-pytorch/)
	+ [CNN in PyTorch (2)](https://algorithmia.com/blog/convolutional-neural-nets-in-pytorch)

- [CIFAR-10](http://www.cs.toronto.edu/~kriz/cifar.html) is an established computer-vision dataset. Attempt a related challenge on Kaggle - [Object Recognition](https://www.kaggle.com/c/cifar-10).

- Try implementing CNN models for classification problems on your own. This article will guide you as to how you can [Create your own dataset](https://towardsdatascience.com/how-to-create-your-own-image-dataset-for-deep-learning-b53f1c22c443).

### 5 | CNN Architectures

- We will now start with understanding the significance of CNN architecture. In case you have never read a research paper before, here is a guide to get you started - [How to Read a Research Paper](https://www.youtube.com/watch?v=SHTOI0KtZnU).

- It might be overwhelming to read a paper but it is strongly recommended that you do read at least one of them - 
 	1. [AlexNet](https://papers.nips.cc/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf)
 	2. [VGGNet](https://arxiv.org/pdf/1409.1556.pdf)
 	3. [ResNet](https://arxiv.org/pdf/1512.03385.pdf)
 	4. [GoogleNet](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43022.pdf)

- It is okay even if you do not understand all of it. These articles might come handy -
	+ [AlexNet: The Architecture that Challenged CNNs](https://towardsdatascience.com/alexnet-the-architecture-that-challenged-cnns-e406d5297951)
	+ [VGGNet Architecture Explained](https://medium.com/analytics-vidhya/vggnet-architecture-explained-e5c7318aa5b6)
	+ [Understanding and Implementing Architectures of ResNet](https://medium.com/@14prakash/understanding-and-implementing-architectures-of-resnet-and-resnext-for-state-of-the-art-image-cf51669e1624)
	+ [A Simple Guide to the Versions of the Inception Network](https://towardsdatascience.com/a-simple-guide-to-the-versions-of-the-inception-network-7fc52b863202)
	
- Read about comparison between these architectures to understand how their development happened and why they are considered as milestones in image processing -
	+ [Difference between AlexNet, VGGNet, ResNet, and Inception](https://towardsdatascience.com/the-w3h-of-alexnet-vggnet-resnet-and-inception-7baaaecccc96)
	+ [The pioneering CNN models in the ILSVRC through the years](https://medium.com/analytics-vidhya/cnns-architectures-lenet-alexnet-vgg-googlenet-resnet-and-more-666091488df5)

### 6 | Implementing Architectures

- Now that you are done with the reading part, lets get our hands hands dirty! For the purpose of getting familiar with coding CNNs, implement AlexNet and VGGNet from scratch. These references might come in handy -
	+ [Scratch to SOTA: Build Famous Classification Nets 2 (AlexNet/VGG)](https://medium.com/swlh/scratch-to-sota-build-famous-classification-nets-2-alexnet-vgg-50a4f55f7f56)
	+ [An awesome repository for tutorial and reference](https://github.com/bentrevett/pytorch-image-classification)
	(If you are feeling adventurous try implementing ResNet too!)
	
- Use an external dataset instead of the built-in ones in pytorch to understand more about dataset reading and data loader creation. Some reasonable size datasets for image classification are - [Caltech 101](https://www.kaggle.com/athota1/caltech101), [Caltech 256](https://www.kaggle.com/jessicali9530/caltech256), [Fashion MNIST](https://www.kaggle.com/zalando-research/fashionmnist), [Food-101](https://www.kaggle.com/kmader/food41?select=images), [Oxford-102-Flowers](https://www.robots.ox.ac.uk/~vgg/data/flowers/102/), [Oxford-IIIT-Pets](https://www.kaggle.com/tanlikesmath/the-oxfordiiit-pet-dataset), [Stanford-Cars](https://www.kaggle.com/jessicali9530/stanford-cars-dataset), [Stanford-Dogs](https://www.kaggle.com/jessicali9530/stanford-dogs-dataset), [Intel Scene](https://www.kaggle.com/puneet6060/intel-image-classification) etc.

### 7 | Transfer Learning

- Transfer learning is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem. Here is [a brief introduction](https://www.geeksforgeeks.org/ml-introduction-to-transfer-learning/) to get you familiar with the concept.
- It is time to use off the shelf models from torchvision, this [guide on using transfer learning for computer vision](https://towardsdatascience.com/transfer-learning-with-convolutional-neural-networks-in-pytorch-dd09190245ce) will help you get started with it. 
- Try experimenting aroung the different pretrained models, an article on [using pretained CNNs in pytorch](https://towardsdatascience.com/using-predefined-and-pretrained-cnns-in-pytorch-e3447cbe9e3c) gives good insights.
- Since this a broad topic to explore and helps you utilize the framework's power, try using more complex datasets and experiment with the new layers you add at the end of pre-trained layers. Here are some more references to help with transfer learning in PyTorch - 
	+ [Using Pre-trained models and their comparison](https://learnopencv.com/pytorch-for-beginners-image-classification-using-pre-trained-models/)
	+ [A vanilla tutorial on transfer learning for computer vision](https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html)
	+ [An edgy tutorial on transfer learning for computer vision](https://medium.com/walmartglobaltech/tackling-multi-class-image-classification-problem-with-transfer-learning-using-pytorch-50150b215fb6)


### 8 | Applications of CNNS
Some applications worth exploring are as follows - 
- [Image Classification With Localization](https://theaisummer.com/Localization_and_Object_Detection/)
- [Object Detection](https://machinelearningmastery.com/object-recognition-with-deep-learning/)
- [Object Segmentation](https://medium.com/visionwizard/object-segmentation-4fc67077a678)
- [Image Style Transfer](https://medium.com/data-science-group-iitr/artistic-style-transfer-with-convolutional-neural-network-7ce2476039fd)
- [Image Colorization](https://towardsdatascience.com/colorizing-black-white-images-with-u-net-and-conditional-gan-a-tutorial-81b2df111cd8)
- [Image Reconstruction](https://www.sciencedirect.com/science/article/pii/S2667102621000061)
- [Image Super-Resolution](https://towardsdatascience.com/an-evolution-in-single-image-super-resolution-using-deep-learning-66f0adfb2d6b)
- [Image Synthesis](https://machinelearningmastery.com/impressive-applications-of-generative-adversarial-networks/)


### 9 | Conclusion
We hope this plan helps you in getting a better understanding Convolutional neural networks which functioned as backbones for many computer vision tasks. If on your learning path you discover some more efficient resources, we would be more than happy to incorporate them here. Just [create a pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on this repository.

***

<p align="center">Created with :heart: by <a href="https://www.wncc-iitb.org/">WnCC</a></p>
