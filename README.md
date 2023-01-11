# Deep-Learning-human-recognition-Video-Processor
For detailed report refer : Deep-Learning-human-recognition-Video-Processor/Extracting and Identifying individuals from media files using supervised 
and unsupervised learning methods (1).pdf

THE GOAL OF THE PROJECT ANALYSING VIDEOS OF SURVEILLANCE TO EXTRACT AND IDENTIFY HUMAN FACES PRESENT OR PARTICIPATED IN THE
VIDEO TO SAVE TIME FOR HUMANS INSPECTING THE VIDEO AND DISPLAY THE IDENTITIES OF THE KNOWN INDIVIDUALS AND PRESENT THE UNKNOWN INDIVIDUALS AS WELL.

The current development takes video files and employs the Intel Open-Source Computer Vision Library - CV2 Library methods to extract the image frames from the video.
Using different face recognition algorithms like HAAR Cascades and Convolutional Neural Networks we identify faces present in individual frames and deploy the 
optimal solution as per efficiency.The output of the current model will contain the faces present in the video frames. This output works as raw data for 
our identification model. Here we will employ the DLIB- ClustImage to cluster similar faces based on the feature extraction using different unsupervised learning 
methods like Principal Component Analysis (PCA),
Histogram Oriented Gradient (HOG), etc. The similar faces are clustered together giving us the unique individuals present in our media file.
This will be the Test data for our identification model which employs supervised classification to identify and name the individuals 
and mention those who are not present in our data.

The project goes under several phases of Data Analysis or steps as mentioned below for cleaning, transforming, processing, visualizing, and modelling data to 
get results:
1. Data Collection
2. Data Exploration
3. Data Pre-processing
4. Feature Extraction
5. Training Model
6. Testing Model
7. Embracing Failure
8. Evaluation

The plot represents the presence of the individuals in Actual Video File, Unsupervised Clusters and the classifier recognition.
The values with 2 are describe as they are present while the value 1 represents that they are absent in the following set. 
Here the numbers of individuals present in the original video file were 14. While the individuals correctly identified and are present in both clusters and classifier 
recognition are 6. 
Hence the prediction accuracy for the current dataset.

Required Libraries to be installed to run the project:
cv2
pandas
numpy
os, os.path
dlib
fnmatch
clustimage ->Clustimage
image
cv2

# from google.colab.patches import cv2_imshow
face_recognition
sklearn -> svm
