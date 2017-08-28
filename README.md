[//]: # (Image References)


[image1]: ./grafo.png "Output"

## Project Overview

In this project we implement, thorugh the routines offered by TensorFlow, the new algorithm contained in [1]. 
It is well known that global minimization of the loss energy related to a Neural Network is a hard task, because
of the several local minima that characterize the energy landscape. Several techniques such as drop out and gradient momentum
have been introduced to mitigate the disadvantages due to gradient descent minimization.
In addition, gradient calculation of a Recurrent Neural Network is a very unstable numerical procedure that easily leads to 
numerical failures. Convoluting the loss function with the heat kernel, we obtain a one parameter family of relaxed energies
that converge to the original functional, for vanishing values of this parameter. These relaxed energies have a convex structure
that stabilizes the numerical minimization, without introduction of other spurious techniques. At each step, the minimization
process is reinitialized with the global minimum of the previous step, and eventually one should converge to the global minimum
of the original loss function.

![Output][image1]

## References

[1] Mobahi, Hossein. "Training Recurrent Neural Networks by Diffusion." arXiv preprint arXiv:1601.04114 (2016).
