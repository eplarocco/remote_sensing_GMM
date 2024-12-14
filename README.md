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

Thoughts:
- Should probably take target spectra out of background image  - can either use with spectra library or in addition or not but might mess up multiple guassian distribution if one group is the target distribution
- For baccharis - resample spectra (library has like 900 but we only need about 100)
- Cosine Similarity
- Discuss pros and cons of new proposed method
- If you use pixels from image as opposed to library spectra, gives you more robust results (can find that vegetation in other areas that aren’t that specific plant - just that plant type)
- Use ground truth to score, not to train
- Do I need to use PCA or normalize before clustering? Would k-means work better?

