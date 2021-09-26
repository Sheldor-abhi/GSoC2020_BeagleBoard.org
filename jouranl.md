---
layout: page
title: Journal
permalink: /journal/
---

---

## Week 1

- Went through courses on Neural Networks and Deep Learning and 
  Convolutional Neural Networks for understanding the basics.


## Week 2

- Finished a course on Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning
  
## Week 3

- Familiarized myself with OpenCV
  - Face detection using Haar Cascade Classfiers
  - Cropping and localization of faces

## Week 4

- Implemented OpenCV for face detection using Haar Cascade Classfiers.
- Flashed the Debian 10 image an SD card and booted the board
- Successfully SSHd into the board
- Started setting up my board with all the dependecies required(python,OpenCV,etc)
- Had to resize the SD card partition, as the board was only able to access 866MB of space from the 16GB SD card 

## Week 5

- Implemented a CNN for recognizing sad or happy from a small data set(80 images) with 3 convolutional layers
  and accuracy of 100% (as data set was too small)
  Now that I know how to build a CNN from scratch and have already made a face detector using OpenCV
  I will be starting to implement facial features extraction from next week.

## Week 6

- Read some papers and looked into some videos for implementing CNN.
- Finalized FER 2013 dataset for testing the CNN
- Trained a model on FER-2013 data set and ran into some issues.

## Week 7

- Trained a model on the FER-2013 data set, but the validation accuracy was not crossing 0.6 
- So I removed one of the emotion subset from the list as the data set was imbalanced with the no of images 
  of 'disgust' being low compared to the others, but even that didn't help much
- Will try changing the deep layers a bit or just use some other dataset


## Week 8

- Tried to find different ways to improve the model
- Looked into different prebuilt architectures like RESTNet101,GoogleNET,MobileNet 
- Will try to build on it through transfer learning as they are pretty good models


## Week 9

- Decided to implement transfer learning by building on the MobileNetV2 architecture
- Worked on bulding and improving the model

## Week 10

- Tried to use OpenCV over SSH
- As I was not able to use my laptop as a display for the board, implemented flask for streaming the OpenCV frames 
  from the board to a IP
- Tried installing Tensorflow lite on the board from source, but failed to do so.
- So overall, was able to implement face detection on the board,streaming the frames to an IP,
  and was able to depoly my Emotion Detection model on my laptop.
  

