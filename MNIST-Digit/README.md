### Test Generation
For each dataset there are four transformations we experiment on. These are Panning, 2D Rotation, Affine and Perspective. 
The python notebook can be found under Test Generation under each dataset folder. 

Please change 'MINI_DATASET_TEST' to False if you want to run the full datasets. Once it is set to true, the test generation framework will only run for a subset images in the interest of time.


### Data Quality
For each dataset we try to find low entropy (this means that the model is fairly certain of the prediction), but the prediction 
for these images is incorrect. Intuitively, this may mean that the data may be mislabelled [1]. 

We also highlight some prominent examples of low data quality in each notebook 
