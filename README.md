# Image-Compression-with-K-Means
<br/>
The code is using the KMeans clustering algorithm from scikit-learn to compress an image. The original image is loaded using the matplotlib library, and the shape of the image is displayed as (1599, 899, 3), which indicates that it has 1599 rows, 899 columns, and 3 color channels (red, green, blue). The image is then normalized by dividing all values by 255, so that all values fall in the range of 0-1. The image is then reshaped into a 2D array with 1437501 rows and 3 columns, where each row represents a pixel in the image and the 3 columns represent the red, green, and blue values of that pixel.<br/><br/>

KMeans is then used to cluster the pixel values into 16 clusters, with the cluster centers being stored in the "kmeans.cluster_centers_" variable. The labels of the clusters each pixel belongs to is stored in the "kmeans.labels_" variable. The shape of kmeans.labels_ is (1437501,), which is the same as the number of pixels in the image.<br/><br/>

The image is then represented in terms of the indices of the cluster centers and the image is reshaped back to the original shape. The original image and the compressed image are then displayed using matplotlib's imshow function. The compressed image will be a version of the original image with fewer colors, and therefore a smaller file size.<br/>
