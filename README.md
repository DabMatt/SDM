# SDM

This file descirbes the global architecture of the code that we published.

The file "Preprocessing.ipynb" corresponds to the pre-treatments we applied to the images, to be able to use them as a dataset.
The file "HOG and creation of dataframes.ipynb" contains:
  - the definition of our function computing the Histogram of Oriented Gradients for each image
  - a treatment applied to our images to build training and test datasets in the form of csv files
			(we can not send these produced datasets as they are too heavy)

The "Saved" folder contains elements that were computed one time and re-used, especially during the presentation.
We find here "SVM_b" which is the first version of the SVM, and "SVM_b_2.0" which is the second version, as described in the report.
We can also find the file "Homography_matrix" which contains the homography matrix used for our video.

The "Pedestrians" folder contains input images and videos on which we tested our algorithms.
The "Results" folder contains results of these tests.

The "SocialDistanceMonitoring.ipynb" file contains the main parts of the code, and the code used for the tests mentioned previously.
It exploits the files

The Datasets (both csv files and images used) are available on GitHub at the url: 
https://github.com/DabMatt/SDM

The folders of the same name in GitHub contains those images and csv files, and use the below described architecture.

The purpose of the "DataToPreProcess" folder, which empty here, is to contain raw images that have been preprocessed before using them
 in our dataset. It contains subfolders "Train" and "Test" which themselves contain subfolders "Pos" and "Neg" corresponding to samples 
respectively belonging and not belonging to the class "human", for our training set and our test set.

The purpose of the "Datasets" folder, which is empty here, is first to contain the preprocessed images that are fit to be used for 
building the dataset, and its architecture is the same (using "Train", "Test", "Pos" and "Neg" subfolders).

Its second purpose is to contain three csv files representing our datasets. One is called "test_data_b.csv", corresponds to the
test set, and is located in the "Test" folder, outside "Pos" and "Neg" subfolders.
In a similar way, in the "Train" folder we find two csv files "train_data_b.csv" and "train_data_b2.csv".
"train_data_b.csv" has been used to train the first version of the SVM described in the report.
"train_data_b2.csv" has been used to train the second version.