## Image-Clustering

### Overview and Objectives:
- Implement the K-Means Algorithm.
- Deal with Image data (processed and stored in vector format).
- Think about Best Metrics for Evaluating Clustering Solutions

### Detailed Description:
There are 2 parts in this Project:
Writing and testing your own implementation of k-means on a simple data (IRIS)
Using your implementation on a more complex data (MNIST)
Only our results for the MNIST data requires a submission to the leaderboard.
assignment. IRIS is an easier dataset where K-Means can be tested quickly.
For this assignment, you are required to implement the K-Means algorithm. Please
do not use libraries for this assignment except for pre-processing and measuring
performance.

#### Part I: IRIS Data
You can access the data either by:
Using the sklearn library directly with sklearn.datasets.load_iris. It will return X,
y, where X are the features and y the label
Download it from here. The first four columns are the features and the last the labels
The dataset has 150 instances and 4 features:
sepal length in cm
sepal width in cm
petal length in cm
petal width in cm

With this simple data:
Test your k-mean implementation
Implement and test the effect of different initialization strategies (random,
kmeans-++ style)
Compute the silhouette values and coefficients (e.g. using sklearn silhouette
samples and score) for different number of clusters and identify an optimal value.
Familiarize yourself with the V-score (e.g. sklearn.metrics.v_measure _score): this
is a measure of external validity that estimates how the clustering aligns with the
labels. The measure is between 0 and 1, 1 stands for a perfectly complete labeling.

#### Part II: MNIST data
The MIST data is provided under Test and consists of 10,000 images of handwritten
digits (0-9). The images were scanned and scaled into 28x28 pixels. For every digit, each
pixel can be represented as an integer in the range [0, 255] where 0 corresponds to the
pixel being completely white, and 255 corresponds to the pixel being completely black.
This gives us a 28x28 matrix of integers for each digit. We can then flatten each matrix
into a 1x784 vector. No labels are provided.
Format of the input data: Each row is a record (image), which contains 784 comma-
delimited integers.

With this data, you will:
Use your algorithm from Part 1 to assign each of the instances in the input data to
K clusters identified from 1 to K
Show the effect of the number of clusters on the silhouette score when varying the
number of clusters from 2 to 20 by step of 2
Set the number of clusters to 10 and submit the resulting assignment in the
leaderboard.
The format file shows an example file containing 10,000 rows with random class
assignments from 1 to 10
