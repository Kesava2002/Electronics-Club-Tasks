# Analysis of Project:
## Problem Statement
To design a mirror that displays details like time, climate etc and can identify a person using a collection of photos tagged with faces of the person.  
Extra Addition: We can design an option for the user to take sufficient pictures of themself using the mirror and set it as the baseline for future identification.  
## Ideation
The idea of Smart Mirror arised from the use of two-way acrylic mirror.  

![Mirror](https://user-images.githubusercontent.com/84671311/121374740-c63d9c00-c95d-11eb-9885-79f27ad6f3ed.gif)  

Covering the backside with a black sheet gives a mirror. But instead of that, we can partially cover the backside and add a black display of suitable size. The display will be connected to a Raspberry Pi. A camera will also be added to the exterior of the mirror. Face recognition can implemented by OpenCV which uses machine learning algorithms to identify faces from a photo. Then we can implement machine learning again to compare it with photos already in database added by the user. 

Extra Addition: We can also add a voice input/output to the system to implement voice commands.

## Planning
Pipeline for this project can be divided into two subsections:

### Hardware
Here we can figure out dimensions of mirror, display and exterior design. Camera placement must also be determined.  

*Determining dimensions of the mirror-->Finding a suitably sized two-way acrylic mirror-->Finding suitable display--> Forming a rough structure for placement of display, camera and Raspberry pi along with the proper wiring*

### Software
Here there are two parts:

#### User interface
We need to write a python program to implement the functions of the smart mirror.       
Note: The background screen colour while the program is running should be adjusted so that the mirror looks uniform.  

#### Face Recognition
For the face regnition part, we can use the OpenCV library to identify the face part of the picture. Then we need to create neural network to identify the face from the given set of baseline-photos. The user can provide theses photos using an USB storage device with proper organisation of photos. This program must provide the user-interface program with a name or it should give an error message.

Extra Addition: We need to implement an Android/iOS application for the user to add photos and to transfer them to Raspberry Pi device using Bluetooth connection.  

### Parts of Pipleine
| Part                                                       | Feasibility                                     | Means to improve                         |
|------------------------------------------------------------|-------------------------------------------------|------------------------------------------|
| Python program for user-interface                          | Simple                                          | -                                        | 
| Python program for face recognition and identification     | Hard to implement                               | Nothing I could find for the moment      |       
| Setting up Raspberry Pi, camera, display                   | Simple                                          | Cost reduction analysis can be done here | 
| Designing mirror                                           | Simple                                          | Cost reduction, implementing             |     

## Prototyping phase
We can start by obtaining camera, Raspberry Pi device and the display and work on setting up the connections. Once proper functioning is ensured, we can start installing all necessary libraries for proper working of the programs. Then start running the program in Raspberry Pi. Then mirror structure can be constructed and all components can be added.  


