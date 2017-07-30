# DNN-Study

Repository for Research Project in NN.
### Giulio Isacchini
# Learning Through Invariants
## Understanding Deep Convolutional Neural Networks
![alt text](https://raw.githubusercontent.com/giulioisac/DNN-Study/ScatteringTransform.png)

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
- By taking insides from [here](https://07306847857070430948.googlegroups.com/attach/19204cc059e291/gabor_vs_scattering_fortexture_classif.html?part=0.1&view=1&vt=ANaJVrGrgRkwAqsNBqU4f7GRBwVrRCpnTDm__VktUJEF5o_1NaHtr5yUxGBB9M6UVrIav8m5MKMW-e7rUzb02aDy7kaBQKJ0Ev-Dfl_PlBUy8bndD1wbI9k) I tried to build the Scattering transform, the code can be seen in the [notebook](ScatteringTransformMNIST.ipynb). It is not working well at all. Some implementations can be found [here](https://github.com/edouardoyallon/pyscatwave) or [here](https://github.com/joanbruna/scattorch), but I am not really able to decode what is going on in there. 
- build a CNN by taking insides from the [tutorial of Tensorflow](https://www.tensorflow.org/get_started/mnist/pros): the notebook can be found [here](DNN-MNIST.ipynb)

