# DNN-Study

Repository for Research Project in NN.
### Giulio Isacchini
# Learning Through Invariants
## Understanding Deep Convolutional Neural Networks
<div align="center">
 <img src="https://raw.githubusercontent.com/giulioisac/DNN-Study/master/ScatteringTransform.png" >
</div>

### The Mathematical Model

Scattering Convolution Transorm as mathematical model to interpret CNN

Papers:

- [Mallat: Understanding Deep Convolutional Networks](https://arxiv.org/pdf/1601.04920v1.pdf) ironically not much understandable
- [Bruna, Szlam and LeCun: Learning Stable Group Invariant Representations
with Convolutional Networks](https://arxiv.org/pdf/1301.3537v1.pdf) - shorter, easier

The mathematical model with  NO LEARNING is the scattering transform:
- [Bruna, Mallat: Invariant Scattering Convolution Networks](https://arxiv.org/pdf/1203.1513.pdf)

"Workflow":
- Build the Scattering Transform on MNIST- NO LEARNING
- Build a CNN on MNIST - SUPERVISED LEARNING
- Possibly Build a [GAN](https://arxiv.org/pdf/1511.06434.pdf) - UNSUPERVISED LEARNING
	- the "VECTOR ARITHMETIC ON FACE SAMPLES" section is really interesting as it express the linearization on the representation space

What I did so far:
- By taking insides from [here](https://07306847857070430948.googlegroups.com/attach/19204cc059e291/gabor_vs_scattering_fortexture_classif.html?part=0.1&view=1&vt=ANaJVrGrgRkwAqsNBqU4f7GRBwVrRCpnTDm__VktUJEF5o_1NaHtr5yUxGBB9M6UVrIav8m5MKMW-e7rUzb02aDy7kaBQKJ0Ev-Dfl_PlBUy8bndD1wbI9k) I tried to build the Scattering transform bymiself, the code can be seen in the [notebook](ScatteringTransformMNIST.ipynb). It is not working well at all. Then (after weeks of 0 improvements) I found another implementation well documented by one of the students of Mallat and reapplied on the previous example and obtained [this](ScatteringTransformMNIST-NEW.ipynb)
- build a CNN by taking insides from the [tutorial of Tensorflow](https://www.tensorflow.org/get_started/mnist/pros): the notebook can be found [here](DNN-MNIST.ipynb). My first layer filters do not really look like wavelets, however [these ones](https://www.cs.nyu.edu/%7Efergus/papers/zeilerECCV2014.pdf) do, I might choose a better dataset? Or is it worth to compute a wavelet-like first layer?
- Most of all: I spent a lot of time reading Papers and focusing on the theoretical side of the Problem, not much on the implementation, should I focus on that also when I write down the project?

