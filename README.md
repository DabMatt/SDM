# SDM

The file "Preprocessing.ipynb" corresponds to the pre-treatments we applied to the images, to be able to use them as a dataset.
The file "HOG and creation of dataframes.ipynb" contains:
  - the definition of our function computing the Histogram of Oriented Gradients for each image
  - a treatment applied to our images to build training and test datasets in the form of csv files
			(we can not send these produced datasets as they are too heavy)

The "Saved" folder contains elements that were computed one time and re-used, such as different versions of the trained SVM model
The "Pedestrians" folder contains input images and videos on which we tested our algorithms
The "Results" folder contains results of these tests

The "SocialDistanceMonitoring.ipynb" file contains the main parts of the code, and the code used for the tests mentioned previously