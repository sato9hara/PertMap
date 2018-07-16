# PertMap
Sample codes for feature attribution (a.k.a. saliency map) based on data perturbation.


## About PertMap
PertMap (Perturbation-based Saliency Map) highlights pixels in the input image that are relevant to the classification result of machine learning models (mostly, DNN/CNNs).

PertMap uses the size of the allowable data perturbation as the masure of relevance. It seeks the maximally invariant data perturbation that does not change the classification result. The details of the algorithms can be found in the following papers.

* Linear programming, with linear approximation.
	* Satoshi Hara, Kouichi Ikeno, Tasuku Soma, Takanori Maehara. [Maximally Invariant Data Perturbation as Explanation](https://arxiv.org/abs/1806.07004). arXiv:1806.07004, 2018 [[slide]](https://www.slideshare.net/SatoshiHara3/maximally-invariant-data-perturbation-as-explanation).

* Stochastic optimization.
	* Kouichi Ikeno, Satoshi Hara. [Maximizing Invariant Data Perturbation with Stochastic Optimization](https://arxiv.org/abs/1807.05077). arXiv:1807.05077, 2018.

## Sample Codes

### [Linear programming](http://github.com/sato9hara/PertMap/blob/master/Sample_LPPertMap_VGG16.ipynb)

### [Stochastic optimization](http://github.com/sato9hara/PertMap/blob/master/Sample_StochasticPertMap_VGG16.ipynb)

#### Requirements

* Python3.x
* Numpy
* Matplotlib
* scikit-image
* Tensorflow
* CPLEX (only for linear programming)

The code also requires the VGG16 weight file in [this repository](https://github.com/machrisaa/tensorflow-vgg).
