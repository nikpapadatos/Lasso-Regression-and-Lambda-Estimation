# Project: Lasso Regression and Lambda Estimation

## Overview

This project focuses on implementing Lasso and post-Lasso methods for estimating lambda (the regularization parameter) in regression models, with a specific emphasis on instrumental variables (IV) regression. The methodology follows the theoretical framework established in A. Belloni, D. Chen, V. Chernozhukov, C. Hansen (BCCH) paper, which presents a robust technique for high-dimensional settings where the number of instruments (p) exceeds the sample size (n).

### Motivation

The Lasso method is widely used for regularization and variable selection, but its optimal performance depends on accurately selecting the penalty parameter (lambda). In this project, I implement a data-driven approach for estimating lambda, building on the innovations outlined in the referenced paper. These methods allow for efficient model selection and produce reliable first-stage predictions in IV models, even in the presence of heteroscedastic or non-Gaussian errors.

### Key Features

- **Lambda Estimation**: The project introduces a modified version of Lasso designed to handle heteroscedastic disturbances by using a data-weighted ℓ1-penalty.
- **IV Regression**: The Lasso-based IV estimator is applied to empirical examples, demonstrating its performance compared to traditional IV estimation techniques.
- **Applications**: The code can be applied across various datasets, particularly in contexts where the number of instruments is large and unknown a priori.

### Methodology

The Lasso-based IV estimator is asymptotically normal and efficient under the assumption of approximately sparse models, where only a subset of instruments contribute significantly to the first-stage predictions. The project explores this methodology through simulations and real-world applications, showcasing how Lasso and post-Lasso techniques can improve inference in complex, high-dimensional environments.
