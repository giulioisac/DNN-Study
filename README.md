# DNN-Study

Repository for Research Project in NN.
# Giulio Isacchini
### Learning Through Invariants
## Understanding Deep Convolutional Neural Networks

The Structure I want to follow is the following
#The Mathematical Model
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
	 the "VECTOR ARITHMETIC ON FACE SAMPLES" section is really interesting as it express the linearization on the representation space
