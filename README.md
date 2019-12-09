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
Each folder below represents the dataset under test. We have four datasets under test namely:
* MNIST-Digit
* Fashion MNIST
* CIFAR-10
* SVHN

We also have a ``User Study`` folder which has the user study data in .csv format and accompanying scripts to analyze the
same.

### Test Generation
For each dataset there are four transformations we experiment on. These are Panning, 2D Rotation, Affine and Perspective. 
The python notebook can be found under Test Generation under each dataset folder. 

Please change 'MINI_DATASET_TEST' to False if you want to run the full datasets. Once it is set to true, the test generation framework will only run for a subset images in the interest of time.


### Data Quality
For each dataset we try to find low entropy (this means that the model is fairly certain of the prediction), but the prediction 
for these images is incorrect. Intuitively, this may mean that the data may be mislabelled [1]. 

We also highlight some prominent examples of low data quality in each notebook 

### Auxillary Files
  For the SVHN dataset, the dataset *needs* to be downloaded. It can be found [here](https://drive.google.com/file/d/1Zxz1QC5ZD6eREwLfjv1NVdUaZxV0hp4U/view). Please make a folder 'data' under SVHN.
  
#### Auxilarry Data

Consolidated test generation + Test data - https://docs.google.com/spreadsheets/d/1FIYf7CeOIuPmZBWR9B1YZi02qso9plWzGSUu6olZSFA/edit#gid=1182530912

User Study Survey (a Google Account is needed to see the survey) - https://forms.gle/Fprk2pQ9Bk58vi7t9
It is important to note that we present the results from only the first three questions from Section 1 to 4. 

User Study Survey Data - https://docs.google.com/spreadsheets/d/1-5JouWM8o_i64jli8VkmLqo-EHxKcKCSjUIU757bMII/edit?usp=sharing


 
 #### References
 
[1] Jiangwen Sun, Feng-ying Zhao, Chong-Jun Wang, and Shifu Chen. Identifying and correcting mislabeled training instances. In Future Generation Communication and Networking, FGCN 2007, Ramada Plaza Jeju, Jeju-Island, Korea, December 6-8, 2007, Proceedings, pages 244 250, 2007. URL: https://doi.org/10.1109/FG

 #### Contact
 Please contact sakshi_udeshi@mymail.sutd.edu.sg for any queries/clarifications

