# Mask-Detection
# Abstract
The requirements of the final project of the course requires us to build a model capable of classifying a dataset of images
with and without masks.The initial model used Principal Component Analysis and fully connected Convolutional neural network.
Since the data is in the form of images, the input features for any of these models will be too huge for these models to handle.
Hence we used a pretrained model for extracting facial features using. For this we used he concept of HuMoments and Haralick
Texture. By using these concepts we were able to get an feature vector as an output which we later used these extracted features
to train various Machine Learning Models and classify the images.

# Problem Statement
We are given a dataset in which we need to classify whether the person is wearing a mask or not. We used a fully fledged Convolutional Neural Network and MobileNet version 2 as a base classifier in our second method of analysis for detection of images with masks and without masks

# Feature Extraction

The facial features have been extracted using 3 main components :
 
 **Understanding HuMoments**
In computer vision and image processing, image moments are often used to characterize the shape of an object in an image.These moments capture basic information such as the area of the object, the centroid (i.e. the center (x, y)-coordinates of theobject), the orientation, and other desirable properties. Hu Moments are an image descriptor utilized to characterize the shapeof an object in an image. The Hu Moments descriptor returns a real-valued feature vector of 7 values. These 7 values captureand quantify the shape of the object in an image. We can then compare our shape feature vector to other feature vectors todetermine how “similar” two shapes are.
 
 **Understanding Haralick Texture**
Haralick texture features are used to describe the “texture” of an image. Haralick features are derived from the Gray Level Co-occurrence Matrix (GLCM). This matrix records how many times two gray-level pixels adjacent to each other appear in an image. Then based on this matrix, Haralick proposes 13 values that can be extracted from the GLCM to quantify texture. An additional 14 values can be computed; however, they are not often used due to computational instability.

**Understanding cv2.calcHist**
A histogram represents the distribution of pixel intensities (whether color or grayscale) in an image. It can be visualized as a graph (or plot) that gives a high-level intuition of the intensity (pixel value) distribution. We are going to assume a RGB color space in this example, so these pixel values will be in the range of 0 to 255. When plotting the histogram, the x-axis serves as our “bins.” If we construct a histogram with 256 bins, then we are
effectively counting the number of times each pixel value occurs.

**Model Used**

Different models used and their accuracies

Model    | Accuracies  |          
-------------- | ------------- 
Logistic Regression    |  0.8596
Gaussian Naive Bayes    |  0.9074
Random Forest Classifier    | 0.8956
SVM(Linear)    |  0.8922
SVM(RBF)   |  0.8532
Decision Tree Classifier   |  0.8599

The accuracies got increased after applying Neural Network on above models and we were able to reach accuracies near 97%.WOW

# REFERENCES
https://cvexplained.wordpress.com/2020/07/21/10-4-hu-moments/

https://cvexplained.wordpress.com/2020/07/22/10-6-haralick-texture/

https://www.pyimagesearch.com/2021/04/28/opencv-image-histograms-cv2-calchist/

