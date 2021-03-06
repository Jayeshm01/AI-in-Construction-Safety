### 1. Installations
Python 3.7
Tensorflow 1.15
LabelImg


### 2. Project Motivation
There are endless applications of AI, My thought process was to apply AI in Construction Industry in a way that could help improve construction workers' safety. This application of the model to CCTV Video can add as a safeguard to ensuring the safety of workers in the field. 

### 3. How it works?
I collected about 2K images from Google and labeled these images using 'LabelImg'. labelImg is a tool in python that has a straightforward interface to label our classes. In this case, 'Helmet_on' and 'Helmet_missing'. These images are then converted to a TensorFlow record for training. We are using the Tensorflow Object detection API here. 

Since I cannot train a model from scratch with limited images, I will apply Transfer learning here and use Faster-r-CNN-resnet pre-trained model weights as my starting point and modify it to detect classes for this specific use case.

The model is trained until loss < 0.05 

### 4. Results

![Test1](https://github.com/Jayeshm01/AI-in-Construction-Safety/blob/master/PHOTO-2020-03-17-17-46-32%202.jpg)
![Test2](https://github.com/Jayeshm01/AI-in-Construction-Safety/blob/master/PHOTO-2020-03-17-17-46-32%203.jpg)
![Test3](https://github.com/Jayeshm01/AI-in-Construction-Safety/blob/master/PHOTO-2020-03-17-17-46-32%204.jpg)
![Test4](https://github.com/Jayeshm01/AI-in-Construction-Safety/blob/master/PHOTO-2020-03-17-17-46-32.jpg)
![Test5](https://github.com/Jayeshm01/AI-in-Construction-Safety/blob/master/PHOTO-2020-03-17-18-18-45.jpg)


### Refrences

https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html

