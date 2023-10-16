# ExpressionLBPkNN
kNN for Facial Expression Detection using LBP

![sER 2013 example]()

The idea behind this project is to detect human facial emotions using AI. The employed model is a k-Nearest Neighbors (kNN) model. kNN is a classification model that utilizes parameters to form a space. To predict the class of a point, the point is placed in the space and the majority class of the k nearest neighbors is observed. Training this model involves placing points with known classes in the space. We trained this model using the [FER 2013 dataset](https://www.kaggle.com/datasets/msambare/fer2013). The parameters used to characterize these images are determined using the Local Binary Patterns (LBP) method. This method involves considering a pixel and comparing its value with its neighbors within a certain radius, assigning a binary code to each of these neighbors, which constitutes a local pattern for the pixel. Subsequently, a histogram is constructed to represent the distribution of patterns in the image.

The parameters that can be adjusted to improve the model's performance are the radius of neighboring pixels in the LBP method and the number k of neighbors in the kNN.

The highest accuracy we managed to achieve is 0.3 for the following parameters:
Radius = 10, k=100
This is a relatively low accuracy, which can be attributed to the limited effectiveness of the LBP method in characterizing images.
