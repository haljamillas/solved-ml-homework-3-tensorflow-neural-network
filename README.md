Download Link: https://assignmentchef.com/product/solved-ml-homework-3-tensorflow-neural-network
<br>
In this lab, we built three projects that study how Neural Network learn. Each project was built on the MNSIT’s Fashion Data Set. The first model we built was a simple Neural Network from scratch using python, the second model we built used Keras and Tensor flow to build multiple layer Neral Networks, and the last model we have to build a Convolutional  Nerual Network using the Keras module.

1  Introduction to Neural Networks

In this section I will spend time talking a basic idea of a Neural Network. Then show a picture of a simple  Neural Network and explain it’s components.

<strong>1.1</strong><strong>    What is a Neural Network?</strong>

A Neural Network is actually a function of many variables: It takes an input, makes computations and produces an output. We like to visualize it as neurons in different layers, with each neuron in a layer connected with all neurons in the previous and the next layer. All the computations take place inside those neurons and depend on the weights that connect the neurons with each other. So all we have to do is learn the right weights in order to get the desired output.

Their structure is generally very complex including a lot of layers and even more than a million neurons in order to be able to handle the large datasets of our era. However, in order to understand how large deep neural networks work one should start with the simplest ones.

<strong>1.2</strong><strong>  Example of a Simple Neural Network</strong>

Here’s an example of a Neural Network:

Neural networks can usually be read from left to right. Here, the first layer is the layer in which inputs are entered. There are 2 internals layers (called hidden layers) that do some math, and one last layer that contains all the possible outputs. Don’t bother with the “+1”s at the bottom of every columns. It is something called “bias” and we’ll talk about that later.

<h1>2   Performance of each Neural Network</h1>

This section will try to explain why different Neural Network might have different performance base on the activation functions and algorithm used.

3.1 One Hidden Layer Neural Network

This is the simplest form of a Neural Network. This is where we only have three layers. So we will have an input layer, a hidden layer and an output layer. Next, we need an activation function. The sigmoid function is a good choice for the last layer because it outputs values between 0 and 1 while tanh (hyperbolic tangent) was considered but the sigmoid had performed better for the hidden layer, but every other commonly used function will work (RELU etc.)

<h2>3.2 Mutli-Layer Model Neural Network</h2>

This is a larger version of the last Neural Network with multiple weights and hidden layers.

Since Keras is easier to use more complicated activation functions were used such as Hyperbolic Tangent and Softmax function. These were used to make the results more accurate. Here is a picture of a larger NN:

3.3 Convolution Neural Network

A Convolutional Neural Network (ConvNet/CNN) is a Deep Learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other. The preprocessing required in a ConvNet is much lower as compared to other classification algorithms. While in primitive methods filters are hand-engineered, with enough training, ConvNets have the ability to learn these filters/characteristics. The architecture of a ConvNet is analogous to that of the connectivity pattern of Neurons in the Human Brain and was inspired by the organization of the Visual Cortex. Individual neurons respond to stimuli only in a restricted region of the visual field known as the Receptive Field. A collection of such fields overlap to cover the entire visual area.

<h1>4 Result Comparison</h1>

<ol>

 <li><strong>One hidden layer Neural Network </strong></li>

</ol>

The Cost rapidly declines and then steadily declines after the 100<sup>th</sup> iteration.  However, our model isn’t quite precise:

<ol start="2">

 <li><strong>Nine Layer Model Neural Network </strong></li>

</ol>

<table>

 <tbody>

  <tr>

   <td width="220"></td>

  </tr>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>




This came out to be fairly accurate. 87% and was an overall good model.

<ol start="3">

 <li><strong>Convolutional Neural Network </strong></li>

</ol>

It faired up around the same as the MultiLayer Network

<h1>           CONCLUSION</h1>

The Convolution Neural Network are the most accurate out of the three, because it involves performing a convolution algorithm which essentially recognize the image and extract 119 abstract features from the image. It could achieve 90% accuracy when train well enough. The second model is the multiple layer Neural network which has 87% accuracy, it shows that the more layer we had, the better prediction outcome. The first layer has around 60% accuracy after train, this is due to not having a large number of iterations (due to time constraints)


