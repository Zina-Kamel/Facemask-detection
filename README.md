# Facemask detection

With the current pandemic and the essential need to constantly wear a mask in public, this project is built to help detect, in real-time, people who are not wearing a mask.

# What I used:

* Mobilenet V2 Model 
* OpenCV
* Haarcascade face classifier

The model is built using transfer learning with MobileNet V2 pretrained model and is then loaded into OpenCV and with the help of haarcascade face classifier to detect the input face images, the model detects whether the person is wearing a facemask or not

# More about the model

MobileNet V2 is a CNN that has 53 layers and an input image size of 224-by-224. I loaded the network and removed the classification layers at the top, for feature extraction inorder to then add my custom dense layers which have 2 output classes. 

# The dataset

![Dataset](https://drive.google.com/uc?export=view&id=1MA_oPKL7yU-lrgXiV4UDK-7q04jO0JZY)

The dataset contains 1376 images belonging to 2 classes. The images also include augmented ones to expand the size of the data, providing variety to reduce the risk of overfitting. 


