# Sign-Language-Recognition_CNN
Building a classification model using CNN to classify the sign language into alphabet and Detecting the hand gesture using OpenCV. Also, Making real time prediction using the classification model and Convert it into text for further use.
# Dataset
The dataset is created by using opencv The data set is a collection of images of alphabets from the American Sign Language, separated in 26 folders which represent the various classes. The training data set contains 2371 images which are 300x300 pixels. There are 26 classes of alphabets.
# Preprocessing
The first task is to preprocess the image. In order to do so first a background of dark is pasted around all the images are converted to ‘RGB’ format to make the image channels similar. Next, we apply our gaussian blur filter to our image which helps us extracting various features of our image. Finally,  the images are transformed to similar dimension 300x300.At the end images are saved but while saving the images extension of images are changed and changed to .jpeg to .png.
# Interfernce
This step is to make the interface that will interpret the sign language and will convert to text. This will be made using OpenCV library of python. The image will be captured and will be made ready so that it can be fade to the CNN model and the output of the model will be displayed in the screen.
# Training and Testing
We apply adaptive threshold to extract our hand from the background and resize our images to 64*64 and then We feed the input images after preprocessing to our CNN model for training and testing. The prediction layer estimates how likely the image will fall under one of the classes. So, the output is normalized between 0 and 1 and such that the sum of each value in each class sums to 1. We have achieved this using SoftMax function.



