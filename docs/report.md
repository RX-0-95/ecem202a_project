# Table of Contents
* Abstract
* [Introduction](#1-introduction)
* [Related Work](#2-related-work)
* [Technical Approach](#3-technical-approach)
* [Evaluation and Results](#4-evaluation-and-results)
* [Discussion and Conclusions](#5-discussion-and-conclusions)
* [References](#6-references)

# Abstract

Provide a brief overview of the project objhectives, approach, and results.

# 1. Introduction
With the fast development of machine learning model compression and edge device AI framework, it is practical to deploy machine learning programmes to edge devices, more and more electronic devices are able to become smart devices. One of the most important areas is smart cameras. Smart cameras can be widely used in personal home security, warehouse security or factory assembly line monitoring. Currently, most of the smart cameras in the market use their onboard chip for AI computation. Although those smart cameras have fast WIFI connection and are able to connect to smartphones or computers, their entire computation is limited by their on board microcontroller.  Such design leads to several potential problems. First, most of those cameras can only run simple person detection neural networks due to the limited computational power and ram. Most of the high performance neural network requires hundreds of MB’s to store the model and fast GPU to inference the model which is unlikely to be available on smart camera due to the cost and physical size of the camera.  Second, it’s impractical to update such a smart camera because most of the time the camera module is good enough for many years, but new machine learning algorithms update fast, and would require more computational power in general. Updating such a smart camera for new AI performance would require replacing the entire module. 

Despite those problems, I do believe that the edge device AI has it’s irreplaceable role in smart devices. With the large bandwidth provided by 5G and WIFI, it is easy to transfer data from the edge device to a central hub or server for large computation. But that does not mean the edge device is only transmitting dataout, in fact, their computation ability can work tightly with the central server to reduce the pressure of the server. Furthermore, in a central server based smart camera system, the edge AI can provide baseline functions to prevent sudden shutdown of the server, especially when using a cloud central server. 

The goal of this project is to design a central server based camera system but meanwhile maximize the usage of the edge device AI computation resource. The project includes two modules, the smart camera module and the central server module. The smart camera transfers the captured image to the central server and meanwhile processes the image to detect if there is motion and person in the captured image. The central serval has a GUI to display the captured video to the user. Due to the limit of microcontrollers inside the smart camera module, the person detection accuracy and  robustness are limited. Thus the central server will run an advanced neural network for person detection. A Dynamic priority system is implemented to integrate edge AI I and the central server. The motion and person detection computed inside the smart camera model will be sent to central serval. Central serval will change the priority of the camera based on those results, the purpose of the system is to use edge AI to increase the efficiency of the central server, reduce the cost on those servers, especially when multiple cameras are connected to the server. 

Challenges of this project include design pipeline for the smart camera system, taks schedule inside the embedded system. How to make the camera transfer image to the central server while performing neural network inference and how to make the smart camera work tightly with the central server are important tasks in this project.The main hardware of this project includes two Raspberry Pi Pico, one is used for the smart camera system and another one is used as a programmer to program and debug the other Pico. One Arducam used to capture images and one MacBook and Raspberry Pi 3B+ used as a central server connected to Raspberry Pi Pico serial port via TTL USB adapter. One the software side, the entire program uses C and C++ with the GNU compiler.  The software build system is CMake, and uses FreeRTOS as the real time operating system. The program also uses neural networks in both the camera module and the central server. In the Pico, the neural network is implemented  using Tensorflow lite, in the central server, the neural network is implemented based on Pytorch. 





This section should cover the following items:

* Motivation & Objective: What are you trying to do and why? (plain English without jargon)
* State of the Art & Its Limitations: How is it done today, and what are the limits of current practice?
* Novelty & Rationale: What is new in your approach and why do you think it will be successful?
* Potential Impact: If the project is successful, what difference will it make, both technically and broadly?
* Challenges: What are the challenges and risks?
* Requirements for Success: What skills and resources are necessary to perform the project?
* Metrics of Success: What are metrics by which you would check for success?

# 2. Related Work

# 3. Technical Approach

# 4. Evaluation and Results

# 5. Discussion and Conclusions

# 6. References
