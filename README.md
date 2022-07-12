# Forest Fire/Smoke Detection using RCNN

DELHI TECHNOLOGICAL UNIVERSITY


Faculty Supervisor:
Dr. Dinesh Kumar Vishwakarma

Submitted by:
Adarsh Jha (2K19/EE/018)
Manthan Garg (2K19/IT/076)
Mridul Chaturvedi (2K19/IT/079)
Index

Sno.
Topic
Pg No.



1
Introduction
3

2
Implementation Details
4

3
Code
5

4
Experimental Results
7

5
Discussion
8

6
References
10







1. Introduction

Object detection has been an increasing measure of attention in recent years due to its wide scope of applications and recent technological leaps. Deep learning is the state-of-art method to perform object detection. This task is under extensive investigation in both academics and real-world applications such as security monitoring, autonomous driving, transportation surveillance, drone scene analysis, robotic vision, etc. It is a computer technology related to computer vision and image processing that deals with detecting instances of semantic objects of a certain class (such as humans, buildings, or cars) in digital images or videos. It not only provides the classes of the objects in an image but also localizes them in that particular image. The location is given in the form of bounding boxes or centroids. Instance segmentation may be defined as the technique that gives fine inference separately for each object by predicting labels for every pixel of that object in the input image. Each pixel is labeled according to the object class within which it is enclosed. We deal with Mask Region-Based Convolutional Neural Network (Mask R-CNN) to implement instance segmentation and detection of fire in a video or an image which can be used in real-world such as automatic fire extinguisher and alert systems. The training was done using Mask R-CNN. With this, the proposed framework can detect fire using Mask Region-Based Convolutional Neural Network and can send an immediate alert to the user if the fire is detected.

 
2. Implementation Details
 
This project is about the development of smoke detection algorithms in the case of forest fires. Our main problem statement is applying classification and object detection to identify smoke/fire through images. I am using the Mask RCNN model for object detection in this case.
Step 1: Data gathering and collection: We have gathered data available online at the below location. https://sintecsys-omdena.s3.amazonaws.com/images3.zip Dataset has almost 16.5K images (~8k masked and ~8k original images).
Step 2: Exploration of data: Masked images have been already created. The model needs to be trained on existing masked images and start predicting. Size of images is 1920 X 1080   .
Step 3: Applying Image recognition and Object detection models.
Iteration 1: Simple image recognition model and tried to train with simple CNN model
Iteration 2: Mask RCNN model
Step 4: Demonstration of Mask RCNN model

5. Discussion/Conclusion



The model so constructed provides more than 75% precision, along with more than 85% recall rate, and detects fire from smoke coming out of the field.  
To make the whole system more user-friendly and accessible we have also made a web page using normal JS and HTML. On this page, the user just has to upload the png file and click submit. The model automatically takes the image uploaded and checks it for fire. If detected it is shown as the above image. And if it’s safe it’s displayed as the image below. 









6. References

Mask R-CNN Kaiming He, Georgia Gkioxari, Piotr Dollar, Ross Girshick; Proceedings of the IEEE International Conference on Computer Vision (ICCV), 2017, pp. 2961-2969

 
 
 
 
 
 
 
