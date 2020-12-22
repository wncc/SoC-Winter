# Neural Style Transfer for Stylising Images
***

Neural style transfer is an optimization technique used to take two images—a content image and a style reference image (such as an artwork by a famous painter)—and blend them together so the output image looks like the content image, but “painted” in the style of the style reference image.
Remember those pictures where AI apparently used to create art? Neural Style Transfer is one way of achieving this by allowing your AI to create paintings of objects inspired by a particular style!

## Prequisites
- ### Python
  Python is the default choice for fast prototyping and deployment of AI models right now and we will use the same for this approach of Neural Style Transfer. If you are enthusiastic you can attempt this in Julia or R or even C++! (Anything that supports TensorFlow is a good bet!)
  However if you are a complete beginner we recomend Python. You can learn to code in Python [here](https://www.wncc-iitb.org/wiki/index.php/Python_for_Beginners).

- ### Basics of Deep Learning
  This is an intermediate project that assumes you are familar with deep learning! If you have no clue, we recommend our [course](https://github.com/wncc/learners-space/tree/master/Machine%20Learning) on Machine Learning. The content from Week 4 onwards is really important and required for this project!
  
## The Idea

The principle of neural style transfer is to define two distance functions, one that describes how different the content of two images are, called the content distance, and one that describes the difference between the two images in terms of their style, the style distance. Then, given three images, a desired style image, a desired content image, and the input image (initialized with the content image), we try to transform the input image to minimize the content distance with the content image and its style distance with the style image.

How will this be achieved? Gradient Descent! In essence you want to optimise the output image with respect to two distances. If we choose a proper metric all we have to do is descend down the hill and minimise both the content and the style image!

It is best to read the original paper [here](https://arxiv.org/pdf/1508.06576.pdf) to get an undersatnding of the motivation and approach used by the authors (including their choice of metric).

## The Procedure

In principle, one could just optimise with respect to the original image. But this would be too time consuming since the number of parameters would be huge. Instead we could use an image classification network (like VGG16 or VGG19) and use their intermediate activations as a representation of the image (encoding!). We will use this representation to compute both the style and the content distance!

There are a lot of articles on the internet that explain step by step how to achieve this. If you are looking for a challenge, implementing from the original paper seems to be the best way!
However for the less daring, the following two articles serve as a good resource:
1. [TensorFlow Tutorial on Neural Style Transfer](https://www.tensorflow.org/tutorials/generative/style_transfer)
2. [Neural Style Transfer on TensforFlow 2](https://www.datacamp.com/community/tutorials/implementing-neural-style-transfer-using-tensorflow)

Note that it is recommended to use Colab for this SoC since GPU resources are scarce. If you have a good CUDA powered GPU feel free to implement yourself! Try to achieve a low distance cost by tweaking parameters appropriately.

## Make it more useable!

These are bonus tasks that you can do when you are done:
1. Add a frontend: Flask would be the best way to do this, simply add a frontend to link it with the backend process. You can create an API too!
2. Deploy it to Mobile: There are two ways to do this, one is to use a server side API based in Python and call it with Kotlin/Java. The other would be TensorFlow Lite on Android. I am not sure how good the second approach will be so try!
3. There have been extensions on the above paper, including a real time [variant](https://arxiv.org/abs/1705.06830). TensorFlow Hub has an implementation of this, try to see how this can be used and deployed to mobile (real time makes the most sense here!)

Have fun creating awesome artwork with deep learning!
