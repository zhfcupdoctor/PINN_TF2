# PINN(s): Physics-Informed Neural Network(s) on TensorFlow 2

This repository includes [PINN(s)](https://doi.org/10.1016/j.jcp.2018.10.045) implementation on TensorFlow 2 to solve von Karman vortex streets (inverse problem, <code>01_von_Karman</code>), Burgers equation (forward problem, <code>02_Burgers</code>), and 2D wave equation (forward problem, <code>03_wave</code>). 

<br>
The power of [automatic differentiation](https://arxiv.org/abs/1502.05767), which is a generalization of [back-propagation](https://doi.org/10.1038/323533a0), is utilized to leverage the convenctional neural network architecture's expressive power. While [original work](https://github.com/maziarraissi/PINNs) is bulit on TensorFlow 1, this repository's codes implement on TensorFlow 2 for GPU-utilized acceleration

Further descriptions can be found in corresponding directories (usage, option, etc.). 

This is an implementation of   to solve Burgers equation (1D NS equation eliminating pressure gradient) under Dirichlet boundary condition without training data (data to fit initial & boundary conditions need to be provided). . Unlike <code>03_wave</code>, this repo utilizes keras packages for simple coding, and does not include [L-LAAF](https://doi.org/10.1098/rspa.2020.0334). 

## Environment
Tested on 
<br>
<code>
  python 3.8.10
</code>
<br>
with the following:

|Package                      |Version|
| :---: | :---: |
|numpy                        |1.22.1|
|scipy                        |1.7.3|
|tensorflow                   |2.8.0|

## Reference
[1] Raissi, M., Perdikaris, P., Karniadakis, G.E.: Physics-informed neural networks: A deep learning framework for solving forward and inverse problems involving nonlinear partial differential equations, *Journal of Computational Physics*, Vol. 378, pp. 686-707, 2019. 
<br>
[2] Baydin, A.G., Pearlmutter, B.A., Radul, A.A., Siskind, J.M.: Automatic Differentiation in Machine Learning: A Survey, *Journal of Machine Learning Research*, Vol. 18, No. 1, pp. 5595–5637, 2018. 
<br>
[3] Rumelhart, D., Hinton, G., Williams, R.: Learning representations by back-propagating errors, *Nature*, Vol. 323, pp. 533–536, 1986. 
<br>
[4] Jagtap, A.D., Kawaguchi, K., Karniadakis, GE.: Locally adaptive activation functions with slope recovery for deep and physics-informed neural networks, *Proceedings of Royal Society A*, pp. 4762020033420200334, 2020. 
