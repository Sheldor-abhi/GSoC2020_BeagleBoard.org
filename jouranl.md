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
  
<!-- ## Week 11

- Aug 10:
  - Not able to make the compatibility code to work on v5.4x-ti-overlay branch.
- Aug 11:
  - Tried merging compatibility code uisng meld but things didn't work out well.
  - rcn-ee's creating 4.19x-ti-overlays and that will solve the issue hopefully.
- Aug 12:
  - Compatibility layer got merged into v4.19.x-ti-overlays branch.
- Aug 13:
  - Submitted [UART console](https://github.com/beagleboard/cloud9-examples/pull/46) example to cloud9-examples.
- Aug 14:
  - updted blinkR30 examples [PR](https://github.com/beagleboard/cloud9-examples/pull/45#issuecomment-674055684).
- Aug 15:
  - Independence Day break 🤩
- Aug 16:
  - added McASP nodes and labels for BBBWL, BBB and BBAI.

## Week 12

- Aug 17:
  - added eCAP pinmux nodes.
  - started working on eQEP.
- Aug 18:
  - Completed McASP, eCAP, ADC, and eQEP DT nodes.
- Aug 19:
  - [compatibility_update1](https://github.com/beagleboard/BeagleBoard-DeviceTrees/pull/20) has been merged.
- Aug 20:
  - Started working on compatibility_update2.
- Aug 21:
  - Worked in compatibility_update2.
- Aug 22:
  - Created new nodes and cleaned up things for compatibility_update2.
- Aug 23:
  - Completed compatibility_update2 coding.
  - Started Testing i.e. Loading each overlays on boards.

## Week 13

- Aug 24:
  - Compatibility update got [merged](https://github.com/beagleboard/BeagleBoard-DeviceTrees/pull/21).
- Aug 25:
  - looking into TI SDK for LCD solution.
- Aug 26:
  - Started Working on this site, updated page handling.
  - New Table of content file `/_data/toc.yaml` for finer control.
- Aug 27:
  - Created new collapsable item for `site.description`, press 📌to see the message.
  - Updated Blog page for better pagination.
  - LCD4 is working with BBAI now! 
    - [BBAI-4D4C-00A1.dts](https://github.com/lorforlinux/BeagleBoard-DeviceTrees/blob/compatibility_Update3/src/arm/overlays/BBAI-4D4C-00A1.dts)
- Aug 28:
  - Finalized [cape interface spec](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec) page.
- Aug 29:
  - Updated this site, ready to submit GSoC final report.
- Aug 30:
  - Submitted Final evaluation.
- Aug 31:
  - End of my GSoC2020 journey!
  - Will continue to work on this site! -->
