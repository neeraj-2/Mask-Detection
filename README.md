# Mask-Detection
# Abstract
The requirements of the final project of the course requires us to build a model capable of classifying a dataset of images
with and without masks.The initial model used Principal Component Analysis and fully connected Convolutional neural network.
Since the data is in the form of images, the input features for any of these models will be too huge for these models to handle.
Hence we used a pretrained model for extracting facial features using. For this we used he concept of HuMoments and Haralick
Texture. By using these concepts we were able to get an feature vector as an output which we later used these extracted features
to train various Machine Learning Models and classify the images.


 REFERENCES
[1] https://cvexplained.wordpress.com/2020/07/21/10-4-hu-moments/
[2] https://cvexplained.wordpress.com/2020/07/22/10-6-haralick-texture/
[3] https://www.pyimagesearch.com/2021/04/28/opencv-image-histograms-cv2-calchist/
[4] https://www.researchgate.net/publication/341798630C lassif icationoftomatoleafdiseasesusingMobileNetv2/fulltext/5ed54425299bf1c67d325075/Classif ication−
of − tomato − leaf − diseases − using − MobileNet − v2.pdf