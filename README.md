# Central Server/Hub Based Smart Multi-Camera System
----------
UCLA ECE202A Final Project by Deyu Yang. 

## Table of Contenet
* TODO


## Abstract

## Background & Motivation
With the fast development of machine learning model compression and edge device AI framework, it is practical to deploy machine learning programmes to edge devices, more and more electronic devices are able to become smart devices. One of the most important areas is smart cameras. Smart cameras can be widely used in personal home security, warehouse security or factory assembly line monitoring. 

Currently, most of the smart cameras in the market use their onboard chip for AI computation. Although those smart cameras have fast WIFI connection and are able to connect to smartphones or computers, their entire computation is limited by their on board microcontroller.  Such design leads to several potential problems. First, most of those cameras can only run simple person detection neural networks due to the limited computational power and ram. Most of the high performance neural network requires hundreds of MB’s to store the model and fast GPU to inference the model which is unlikely to be available on smart camera due to the cost and physical size of the camera.  Second, it’s impractical to update such a smart camera because most of the time the camera module is good enough for many years, but new machine learning algorithms update fast, and would require more computational power in general. Updating such a smart camera for new AI performance would require replacing the entire module. 

Despite those problems, I do believe that the edge device AI has it’s irreplaceable role in smart devices. With the large bandwidth provided by 5G and WIFI, it is easy to transfer data from the edge device to a central hub or server for large computation. But that does not mean the edge device is only transmitting dataout, in fact, their computation ability can work tightly with the central server to reduce the pressure of the server. Furthermore, in a central server based smart camera system, the edge AI can provide baseline functions to prevent sudden shutdown of the server, especially when using a cloud central server. 


## Goal & Deliver



## Hardware

## Implementation

### Embedded Camera System

### Central Hub and Priorty Queue Scheduler

## Evaluation

### Weak Point

## Conclusion


## Time Line
----------------
# ecem202a_project
This is repository template for UCLA ECEM202A / CSM213A projects.

Use the folders as follows:

* doc/ for website content
* software/ for code used in your project
* data/ for data data used in your project

You may add additional folders as necessary.

Add your project's code to this folder.