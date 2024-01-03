# K-Means-Clustering-for-Image-Segmentation
K-Means Image Segmentation using Superpixels

  Background
Clustering is a process that groups data with respect to data similarity so that similar data take part
same cluster. In image domain clustering is used for various types of problem e.g. image quantization,
image segmentation. A good clustering algorithm must group data to homogeneous subsets as possibble.
Similarity is most critical step in a clustering algorithm that determine how the clustering algorithm
groups data. K-means clustering is one of the most popular clustering algorithm that groups data to k
dissimilar clusters. It is an unsupervised learning algorithm for clustering problem and the main idea is
to define k centroids one of each cluster. These centroids is randomly assigned to data space for first
iteration. In the next steps, for each data point, distance to these centroids is calculated and data points
are assigned to nearest centoids as cluster elements. Then for each cluster, new k centroids are calculated
from k clusters. This steps go on until clusters centroids unchange.

  Overview
In this assignment, you will use k-means clustering algorithm for image segmentation by using superpixel
representation of an input image. For this purpose you must carry out the following steps:
  • Extracts Superpixels
You will use SLIC Superpixel work to extract superpixel labels. You can use skimage.slic
  • Feature Representation of Each Superpixel
You will define a feature vector to represent eachs superpixel. This feature vector may contain
various type of features such as color,intensity, location or 1st order statistics of these features in
superpixels e.g. means of intensities. You will build up your own feature representation.
  • K-Means Clustering of Superpixels
You can use python built-in function for k-means clustering. You will give feature points obtained
from each superpixel and cluster number to k-means algorithm so that k-means algorithm will
produce cluster labels for each superpixel.

  Details
Your program will take an color or gray level image and cluster number as input and produce
segmentation result like in Figure 1-c,1-d.
