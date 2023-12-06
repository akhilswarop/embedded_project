# Embedded Systems Project: Handwritten Characters Classifier

## Overview

Welcome to our embedded systems project! This project focuses on designing and implementing three classifiers for recognizing handwritten numbers, alphabets, and shapes. The embedded system utilizes a combination of hardware and software components to perform real-time classification.

## Classifiers

### 1. Handwritten Number Classifier

The handwritten number classifier is trained to recognize and classify numerical digits (0-9) written by hand. It uses a trained machine learning model (Linear SVC) to make predictions based on input images of handwritten numbers.

### 2. Alphabet Classifier

The alphabet classifier is designed to identify and categorize handwritten letters (A-Z). Similar to the number classifier, it employs a machine learning model trained on a dataset of handwritten alphabet images.

### 3. Shapes Classifier

The shapes classifier focuses on recognizing basic geometric shapes such as circles, squares, triangles, and rectangles. It utilizes image processing techniques and a custom-trained model to classify different shapes accurately.

## Hardware and Software Components

The embedded system is composed of the following key elements:

- **Microcontroller/Processor**: Raspberry Pi Pico

- **Sensor/Input Device**: Camera Module (OV7670)
- **Output Device**: 1.8 TFT 128*160 Display
- **Machine Learning Model**: 
A Linear Support Vector Classifier (Linear SVC) is a supervised machine learning model used for classification tasks. It belongs to the family of Support Vector Machines (SVMs) and is specifically designed for linearly separable datasets. The model aims to find a hyperplane that best separates different classes in the feature space.

- **Real-Time Processing**: The images are captured by the camera and are pre-processed in real time. They are converted to 12*12 resolution and converted to grayscale before feeding them to the model for fairly accurate yet, efficient predictions.

## Steps to run the project


1. Make connections between the components as shown below

| Display Pin Number | Display Pin Name | Pi Pico Pins |                          
| :------------------ | :---------------: | ------------: |
| 2                  | VCC               |            5V |
| 1                  | GND               |            GND |
| 10                 | CS                |          GP18 |
| 6                  | RESET             |          GP17 |
| 7                  | A0                |          GP16 |
| 8                  | SDA               |          GP11 |
| 9                  | SCL               |          GP10 |
| 15                 | LED               |         3.3V |


| OV7670 Pin Name | Pi Pico Pin Name                |
| :-------------- | :-----------------------------  |
| D0              | GP0                             |
| D1              | GP1                             |
| D2              | GP2                             |
| D3              | GP3                             |
| D4              | GP4                             |
| D5              | GP5                             |
| D6              | GP6                             |
| D7              | GP7                             |
| PCLK            | GP8                             |
| MCLK            | GP9                             |
| HS              | GP12                            |
| VS              | GP13                            |
| PDWN            | GP15                            |
| RESET           | GP14                            |
| SCL             | GP21 (via 4.7k external pull-up) |
| SDA             | GP20 (via 4.7k external pull-up) |


2. Install Mu Editor
3. Connect Raspberry Pi Pico to the computer, via a USB cable.
4.  Clone the repository:
    ```bash
    git clone https://github.com/akhilswarop/embedded_project 
   
5. Copy the files in the repository to the hardware.
   
6. The hardware will auto reboot and start its predictions.


## Youtube Link
[Embedded Project](https://youtu.be/zyvXpDkvRKw?si=4BKqQhl7FPQjjoI4)



  
