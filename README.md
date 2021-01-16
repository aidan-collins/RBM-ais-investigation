# RBM-ais-investigation
This is a short exercise I put together to investigate the usage of Annealed Importance Sampling to evaluate the unsupervised training of RBMS.

I am interested in using density estimation to tuning good generative models for unintuitive data using quantitative metrics as the standard
for evaluation. 

Eventually I hope to apply this to the a dataset of recipes and ingredients.

The included notebook shows two brief hyperparameter sweeps over 1 variable (n epochs/model and hidden size/ model).

The results of the epoch-wise sweep were in line with expecations decreasing the negative log liklihood of the test set wrt to an ais test.

The results of the hidden-layer-wise sweep were slightly unexpected indicating the optimal hidden layer size of 600 units (500 expected) increasing
M Ais samples should fix this.

Please note the github links in the notebooks from which I sourced the implementations of RBM and AIS. Many thanks to these authors!
