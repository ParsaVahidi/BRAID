# Publication:
This repository provides implementation of BRAID (**Behavioraly relevant Analysis of Intrinsic Dynamics**)

*Input-driven nonlinear dynamical modeling of neural behavioral data*. ***Under revision*** (2024).

# Usage examples
The following notebook contains usage examples of BRAID for several use-cases:
[source/BRAID/example/BRAID_tutorial.ipynb]

A .py scripty version of the same notebook is also available in the same directory [source/BRAID/example/BRAID_tutorial.py]

# Usage examples
The following are the key classes that are used to implement BRAID formulation as explained in [source/BRAID/BRAIDModelDoc.md] (the code for these key classes is also available in the same directory):

- `BRAIDModel`(./source/BRAID/BRAIDModel.py): performs the full 2-stage modeling with the optional preprocessing stage. BRAID's main 2 stages are implemented in a separated class named MainModel in [source/BRAID/MainModel.py].

-  `RNNModel`(./source/BRAID/RNNModel.py): The custom RNN class, which implements the RNNs that are trained in stages 1, 2 (and the preprocessing stage if used). 

-  `RegressionModel`(./source/BRAID/RegressionModel.py): The class internally used by both `RNNModel` and `MainModel` to build the general multilayer feed-forward neural networks that are used to implement each model parameter. 
