# Callisto: Entropy based test case generation and data quality detection for Machine Learning Systems

### Dependencies
* Python 3
* Keras
* Tensorflow==1.15.0
* Random
* Pickle
* Math
* Matplotlib
* OpenCV
* h5py
* ipython
* numpy

In case of any unforseen dependencies, a detailed ```pip freeze``` of the system used to develop Callisto can be found 
[here](https://docs.google.com/document/d/1Cbcfiv3Y7Fz3jKcwv-h2EWLBY37orPuwbflp_C8P2ok/edit?usp=sharing) 


### Organisation 
Each folder in Callisto represents a dataset under test. We have four datasets under test namely:
* MNIST-Digit
* Fashion MNIST
* CIFAR-10
* SVHN

### Test Generation
For each dataset there are four transformations we experiment on. These are Panning, 2D Rotation, Affine and Perspective. 
The python notebook can be found under Test Generation under each dataset folder. 

Please change 'MINI_DATASET_TEST' to False if you want to run the full datasets. Once it is set to true, the test generation framework will only run for a subset images in the interest of time.


### Data Quality

### Auxillary Files
  For the SVHN dataset, the dataset *needs* to be downloaded. It can be found [here](https://drive.google.com/file/d/1Zxz1QC5ZD6eREwLfjv1NVdUaZxV0hp4U/view). Please make a folder 'data' under SVHN. 
