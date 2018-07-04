# PertMap
Sample code for feature scoring (a.k.a. feature attribution, saliency map) based on data perturbation.


## About PertMap
PertMap (Perturbation-based Saliency Map) highlights pixels in the input image that are relevant to the classification result of machine learning models (mostly, DNN/CNNs).

PertMap uses the size of the allowable data perturbation as the masure of relevance. It seeks the maximally invariant data perturbation that does not change the classification result. The detail of the algorithm can be found in the following paper.

* Satoshi Hara, Kouichi Ikeno, Tasuku Soma, Takanori Maehara. [Maximally Invariant Data Perturbation as Explanation](https://arxiv.org/abs/1806.07004). arXiv:1806.07004, 2018.

## [Sample Code](http://github.com/sato9hara/PertMap/blob/master/Sample_PertMap_VGG16.ipynb)
### Requirements

* Python3.x
* Numpy
* Matplotlib
* scikit-image
* Tensorflow
* CPLEX

The code also requires the VGG16 weight file in [this repository](https://github.com/machrisaa/tensorflow-vgg).
