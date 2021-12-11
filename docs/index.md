# Central Server Based Smart Camera System

This project discovered the feasibility and potential for a central server based smart camera system. The smart camera module alone is able to perform light weight tasks including motion detection and simple person detection using a neural network. The central server running on a PC or Raspberry Pi is able to handle heavy duty tasks such as more advanced and accurate person detection and semantic segmentation, as well as render the GUI. Tasks inside the  smart camera are scheduled to use FreeRTOS, this ensures that the central server will have stable image input while the smart camera performs person detection. The motion detection and person detection result calculated in edge AI devices is transferred to the central server, those results act as a guidance for camera priority. Central serval will first process the camera data with higher priority. This design ensures that the central server will be optimally efficient when multiple cameras connect to it. The system is tested on a 16 mins video and achieve 91% precision on person with the help of the central server. 
![hardware](media/hardware.png)


# Team

* Name of team member \# Deyu Yang


# Required Submissions

* [Proposal](https://github.com/RX-0-95/ecem202a_project/blob/main/docs/proposal.md)
* [Midterm Checkpoint Presentation Slides](https://drive.google.com/file/d/13vPOdrWIEbdKkYJzp15Q4d7FP_68Vn4n/view?usp=sharing)
* [Final Presentation Slides](https://docs.google.com/presentation/d/1pgtKPLpFbrri3FStLB12uFwTmaA0Dbs1Rm_6Q1KEPNU/edit?usp=sharing)
* [Final Report](report)
