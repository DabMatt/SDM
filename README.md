# SDM

This file descirbes the global architecture of the code that we published.

The "Saved" folder contains elements that were computed one time and re-used, especially during the presentation.
We find here "SVM_b" which is the first version of the SVM, and "SVM_b_2.0" which is the second version, as described in the report.
We can also find the file "Homography_matrix" which contains the homography matrix used for our video.

The file "Preprocessing.ipynb" corresponds to the pre-treatments we applied to the images, to be able to use them as a dataset.
The file "HOG and creation of dataframes.ipynb" contains:
  - the definition of our function computing the Histogram of Oriented Gradients for each image
  - a treatment applied to our images to build training and test datasets in the form of csv files
			(we can not send these produced datasets as they are too heavy)

The "SocialDistanceMonitoring.ipynb" file contains the main parts of the code, and the code used for the tests mentioned previously.
It exploits the files

The following folders with their content can be found on this GoogleDrive repository:
https://drive.google.com/drive/folders/1yHc6ppXA98T4zdSWuPmoEoexpBe5q9TY?usp=sharing

The "Pedestrians" folder has for purpose to contain input images and videos on which we tested our algorithms.
The "Results" folder has for purpose to contain the results of these tests.

The Datasets (both csv files and images used) are available on GitHub at the url: 
https://github.com/DabMatt/SDM

The purpose of the "DataToPreProcess" folder, found on GitHub, is to contain raw images that have been preprocessed before using them
 in our dataset. It contains subfolders "Train" and "Test" which themselves contain subfolders "Pos" and "Neg" corresponding to samples 
respectively belonging and not belonging to the class "human", for our respectively training set and our test set.

The first purpose of the "Datasets" folder, found on GitHub, is to contain the preprocessed images that are fit to be used for 
building the dataset, and its architecture is the same (using "Train", "Test", "Pos" and "Neg" subfolders).

Its second purpose is to contain three csv files representing our datasets. One is called "test_data_b.csv", corresponds to the
test set, and is located in the "Test" folder, outside "Pos" and "Neg" subfolders.
In a similar way, in the "Train" folder we find two csv files "train_data_b.csv" and "train_data_b2.csv".
"train_data_b.csv" has been used to train the first version of the SVM described in the report.
"train_data_b2.csv" has been used to train the second version.

When downloaded, all these folders (both from GitHub and GoogleDrive) should keep the same name, 
and be placed in the first folder (named "FinalCode") of the repository.

On GitHub, we can also find two more code files:

