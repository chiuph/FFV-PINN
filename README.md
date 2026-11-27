# FFV-PINN

Code and example datasets for **FFV-PINN: A Fast Physics-Informed Neural Network with Simplified Finite Volume Discretization and Residual Correction**.
[![python >3.8](https://img.shields.io/badge/python-3.8-brightgreen)](https://www.python.org/) 

## **FFV-PINN: A Fast Physics-Informed Neural Network with Simplified Finite Volume Discretization and Residual Correction**

__Chang Wei, Yuchen Fan, Chin Chun Ooi, Jian Cheng Wong, Heyang Wang, Pao-Hsiung Chiu__


_With the growing application of deep learning techniques in computational physics, physics-informed neural networks (PINNs) have emerged as a major research focus. However, today’s PINNs encounter several limitations. Firstly, during the construction of the loss function using automatic differentiation, PINNs often neglect information from neighboring points, which hinders their ability to enforce physical constraints and diminishes their accuracy. Furthermore, issues such as instability and poor convergence persist during PINN training, limiting their applicability to complex fluid dynamics problems. To address these challenges, this paper proposes a fast physics-informed neural network framework that integrates a simplified finite volume method (FVM) and residual correction loss term, referred to as Fast Finite Volume PINN (FFV-PINN). FFV-PINN utilizes a simplified FVM discretization for the convection term, which is one of the main sources of instability, with an accompanying improvement in the dispersion and dissipation behavior. Unlike traditional FVM, which requires careful selection of an appropriate discretization scheme based on the specific physics of the problem such as the sign of the convection term and relative magnitudes of convection and diffusion, the FFV-PINN outputs can be simply and directly harnessed to approximate values on control surfaces, thereby simplifying the discretization process. Moreover, a residual correction loss term is introduced in this study that significantly accelerates convergence and improves training efficiency. To validate the performance of FFV-PINN, we solve a series of challenging problems - including flow in the two-dimensional steady and unsteady lid-driven cavity, three-dimensional steady lid-driven cavity, backward-facing step scenarios, and natural convection at previously unsurpassed Reynolds (Re) number and Rayleigh (Ra) number, respectively — that are typically difficult for PINNs. Notably, the FFV-PINN can achieve data-free solutions for the lid-driven cavity flow at Re = 10000 and natural convection at Ra = 1E8 for the first time in PINN literature, even while requiring only 680s and 231s respectively. These results further highlight the effectiveness of FFV-PINN in improving both speed and accuracy, marking another step forward in the progression of PINNs as competitive neural PDE solvers._

# Install
[![jax-0.4.33](https://img.shields.io/badge/jax-0.4.33-yellowgreen)](https://github.com/google/jax) [![evojax-0.2.17](https://img.shields.io/badge/evojax-0.2.17-orange)](https://github.com/google/evojax) [![evosax-0.1.6](https://img.shields.io/badge/evosax-0.1.6-red)](https://github.com/RobertTLange/evosax) [![flax-0.9.0](https://img.shields.io/badge/flax-0.9.0-lightgrey)](https://github.com/google/flax) [![optax-0.2.3](https://img.shields.io/badge/optax-0.2.3-blue)](https://github.com/google-deepmind/optax) [![numpy-2.1.1](https://img.shields.io/badge/numpy-2.1.1-green)](https://github.com/numpy/numpy) [![pandas-2.2.3](https://img.shields.io/badge/pandas-2.2.3-yellow)](https://github.com/pandas-dev/pandas) [![matplotlib-3.9.2](https://img.shields.io/badge/matplotl


# Usage
You can download this repo and run the demo tasks on your computing machine.

# Time cost
Typical install time should be under 30min for all the above packages. Expected time required for training in the provided scripts should be under 15 minutes on a workstation with Intel Xeon W-2275 CPU and Nvidia Gefore RTX 3090 GPU.

# Citation

Chang Wei, Yuchen Fan, Chin Chun Ooi, Jian Cheng Wong, Heyang Wang, Pao-Hsiung Chiu, "Bridging Computational Fluid Dynamics Algorithm and Physics-Informed Learning: SIMPLE-PINN for Incompressible Navier-Stokes Equations".[Computer Methods in Applied Mechanics and Engineering, 444 (2025), 118139](https://doi.org/10.1016/j.cma.2025.118139)
- **Preprint:** [arXiv:2603.24114](https://arxiv.org/abs/2603.24114) ([PDF](https://arxiv.org/pdf/2603.24114))

