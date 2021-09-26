---
layout: default
title: Home
---

<!-- <div class="text-center">
    <a href="https://elinux.org/BeagleBoard/GSoC/2020_Projects/Cape_Compatibility" target="_blank">
        <img src="public/projectBanner.png" class="border border-danger rounded img-fluid" alt="banner">
    </a>
</div> -->

<p class="text-center message border border-warning bg-dark text-warning">
    The idea of this project was to implement Facial Emotion Recogition on the BeagleBone Black,
    using OpenCV for face detection and a Tensorflow model for the emotion detection. 
</p>

<a href="https://beagleboard.org/latest-images" 
    class="btn btn-warning btn-block text-dark" 
    role="button" aria-pressed="true" target="_blank">
    Download BeagleBoard.org Latest Firmware Images
</a>


<div class="card">
  <div class="card-header bg-dark text-light text-center">
    Installing required libraries and dependencies
  </div>
  <div class="card-body">
    <!-- Section A -->
    <h2 class="card-title">1. Update and Upgrade your system</h2>
    <!-- Step 1 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="sudo apt update -y" id="A1" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('A1')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Step 2 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="sudo apt upgrade -y" id="A2" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('A2')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Step 3 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="sudo reboot" id="A3" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('A3')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Section B -->
    <h2 class="card-title">2. Python installation</h2>
    <!-- Step 1 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="sudo apt-get install python3" id="B1" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('B1')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Step 2 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="sudo apt install python3-pip" id="B2" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('B2')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Section C -->
    <h2 class="card-title">3. Installing dependencies</h2>
    <!-- Step 1 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="pip3 install opencv-python" id="C1" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('C1')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
    <!-- Step 2 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="pip3 install --user --upgrade tensorflow" id="C2" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('C2')"><span class="fa fa-copy"></span></button>
        </div>
        This command cannot be directly used for the beaglebone black, you need to build tensorflow lite from scratch
        Follow<a href="https://github.com/samjabrahams/tensorflow-on-raspberry-pi/blob/master/GUIDE.md">this</a>
    </div>
    <!-- Step 3 -->
    <div class="input-group mb-3">
        <div class="input-group-prepend">
            <span class="input-group-text" id="inputGroup-sizing-sm">&#36;</span>
        </div>
        <input type="text" class="bg-light form-control" value="pip3 install flask" id="C3" disabled>
        <div class="input-group-append">
            <button class="btn btn-outline-secondary copy" type="button" onclick="copy2Clipboard('C3')"><span class="fa fa-copy"></span></button>
        </div>
    </div>
  </div>
</div>

---

# {% octicon shield-check height:24 %} Achieved Milestones

<div class="message">
    These are my major milestones. 
    <!-- <a href="https://elinux.org/BeagleBoard/GSoC/2020_Projects#Milestones">here</a>. -->
</div>

<div class="text-center text-dark border border-warning bg-dark">
    <a href="https://github.com/Sheldor-abhi/Facial-Emotion-Detection" style="color:#ffc107; fill:#ffc107">
        After successfully installing all the dependencies and training my model, I tried deploying the code on the board.
        But due to some issues tensorflow/tensorflowlite could not be directly installed on the board.
        Even after trying some different <a href="https://github.com/samjabrahams/tensorflow-on-raspberry-pi/blob/master/GUIDE.md">methods</a>, I was not able to do it.
        So the model was deployed on my laptop.
    </a>
</div>

| 1. [OpenCV](https://github.com/Sheldor-abhi/Facial-Emotion-Detection/tree/main/OpenCV) 
| 2. [OpenCV+Tensorflow](https://github.com/Sheldor-abhi/Facial-Emotion-Detection/tree/main/OpenCV%2BTensorflow) 

<!-- | 3. [SPI](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#SPI) | 10. [eMMC](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#eMMC) |
| 4. [UART](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#UART) | 11. [LCD](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#LCD) |
| 5. [CAN](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#CAN) | 12. [eQEP](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#eQEP) |
| 6. [ADC](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#ADC) | 13. [McASP](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#McASP) |
| 7. [PWM](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#PWM) | 14. [PRU](https://elinux.org/Beagleboard:BeagleBone_cape_interface_spec#PRU) | -->





---





