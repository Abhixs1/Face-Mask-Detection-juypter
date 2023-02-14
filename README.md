# Face-Mask-Detection


![image](https://user-images.githubusercontent.com/100253637/218631063-139687f0-0411-4aa1-a59c-6d2e2c5e16a4.png)

Face Mask Detection System built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.

![image](https://user-images.githubusercontent.com/100253637/218634800-cddb019a-8d28-490e-a381-db7c63ec0a57.png)

# Abstract

Face mask detection had seen significant progress in the domains of Image processing and Computer
vision, since the rise of the Covid-19 pandemic. Many face detection models have been created using
several algorithms and techniques. The proposed approach in this paper uses deep learning, TensorFlow,
Keras, and OpenCV to detect face masks. This model can be used for safety purposes since it is very
resource efficient to deploy. The SSDMNV2 approach uses Single Shot Multibox Detector as a face
detector and MobilenetV2 architecture as a framework for the classifier, which is very lightweight and
can even be used in embedded devices (like NVIDIA Jetson Nano, Raspberry pi) to perform real-time
mask detection. The technique deployed in this paper gives us an accuracy score of 0.9264 and an F1
score of 0.93. The dataset provided in this paper, was collected from various sources, can be used by
other researchers for further advanced models such as those of face recognition, facial landmarks, and
facial part detection process.

# Objective of the project:

To identify the person on an image/video stream wearing a face mask with the help of computer vision and
deep learning algorithm with opencv, keras,tensorflow. The mask detector that is built in this project could
potentially be used to help in ensuring your safety of others.

# Methodology:

To predict whether a person has worn a mask correctly, the initial stage would be to train the model using
a proper dataset. Details about the Dataset have been discussed. After training the classifier, an accurate
face detection model is required to detect faces, so that the SSDMNV2 model can classify whether the
person is wearing a mask or not. The task in this paper is to raise the accuracy of mask detection without
being too resource-heavy. For doing this task, the DNN module was used from OpenCV, which contains a
‘Single Shot Multibox Detector’ (SSD) ( Liu et al., 2016 ) object detection model with ResNet-10

(Anisimov & Khanova, 2017 ) as its backbone architecture. This approach helps in detecting faces in real-
time, even on embedded devices like Raspberry Pi. The following classifier uses a pre-trained model

MobileNetV2 ( Sandler, Howard, Zhu, Zhmoginov, & Chen, 2018 ) to predict whether the person is
wearing a mask or not.

# Block Diagram

![image](https://user-images.githubusercontent.com/100253637/218635692-22820db8-d7af-4a5c-b11e-ae367f29a567.png)

# Working of block diagram:

Training: Here we’ll focus on loading our face mask detection dataset from disk, training a model
(using Keras/TensorFlow) on this dataset, and then serializing the face mask detector to disk
Deployment: Once the face mask detector is trained, we can then move on to loading the mask detector,
performing face detection, and then classifying each face as with_mask or without_mask

# Features

Our face mask detector doesn't use any morphed masked images dataset and the model is accurate. Owing to the use of MobileNetV2 architecture, it is computationally efficient, thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

This system can therefore be used in real-time applications which require face-mask detection for safety purposes due to the outbreak of Covid-19. This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed

# Result

![image](https://user-images.githubusercontent.com/100253637/218635190-af22bfc7-aebd-476b-b020-636272517be7.png)
