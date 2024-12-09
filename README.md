# Data Generation-based Operator Learning for Solving Partial Differential Equations on Unbounded Domains
The code repository for the paper https://doi.org/10.48550/arXiv.2309.02446.
[https://github.com/JihongWang/DGOL](Code)

## Abstract
Wave propagation problems are typically formulated as partial differential equations (PDEs) on unbounded domains to be solved.
    The classical approach to solving such problems involves truncating them to problems on bounded domains by designing the artificial boundary conditions or perfectly matched layers, which typically require significant effort, and the presence of nonlinearity in the equation makes such designs even more challenging. 
    Emerging deep learning-based methods for solving PDEs, with the physics-informed neural networks (PINNs) method as a representative, still face significant challenges when directly used to solve PDEs on unbounded domains. Calculations performed in a bounded domain of interest without imposing boundary constraints can lead to a lack of unique solutions thus causing the failure of PINNs.
    In light of this, this paper proposes a novel and effective data generation-based operator learning method for solving PDEs on unbounded domains. 
    The key idea behind this method is to generate high-quality training data.
    Specifically, we construct a family of approximate analytical solutions to the target PDE based on its initial condition and source term.
    Then, using these constructed data comprising exact solutions, initial conditions, and source terms, we train an operator learning model called MIONet, which is capable of handling multiple inputs, to learn the mapping from the initial condition and source term to the PDE solution on a bounded domain of interest. 
    Finally, we utilize the generalization ability of this model to predict the solution of the target PDE.
    The effectiveness of this method is exemplified by solving the wave equation and the Schr\"odinger equation defined on unbounded domains. 
    More importantly, the proposed method can deal with nonlinear problems, which has been demonstrated by solving Burgers' equation and Korteweg-de Vries (KdV) equation.
