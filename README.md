# Using GMM for target detection with remote sensing

Iterating through different GMM variations with rigorous evaluation for each, testing if the BIC-selected model is best or if another model is better.

Using Multiple Gaussian Distributions approach on 
- Cooke City image (compare to other people's work)
- Baccharis image.

Python package for modeling an image with multiple mixtures:
https://scikit-learn.org/1.5/modules/mixture.html

Example:
https://scikit-learn.org/1.5/auto_examples/mixture/plot_gmm.html#sphx-glr-auto-examples-mixture-plot-gmm-py

Methods for 'best' model selection using BIC score (best meaning selecting the number of Guassians to use and the type of covariance to use) (BIC = Bayesian Information Criterion, a way to evaluate a model with low error and low complexity):
https://scikit-learn.org/1.5/auto_examples/mixture/plot_gmm_selection.html#sphx-glr-auto-examples-mixture-plot-gmm-selection-py