# Problem Statement
To design a mirror that displays details like time, climate etc and can identify a person using a collection of photos tagged with faces of the person.  
Extra Addition: We can design an option for the user to take sufficient pictures of themself using the mirror and set it as the baseline for future identification.  
# Ideation
The idea of Smart Mirror arised from the use of two-way acrylic mirror.  
![Mirror](https://user-images.githubusercontent.com/84671311/121374740-c63d9c00-c95d-11eb-9885-79f27ad6f3ed.gif)  
Covering the backside with a black sheet gives a mirror. But instead of that, we can partially cover the backside and add a black display of suitable size. The display will be connected to a Raspberry Pi. A camera will also be added to the exterior of the mirror. Face recognition can implemented by OpenCV which uses machine learning algorithms to identify faces from a photo. Then we can implement machine learning again to compare it with photos already in database added by the user.
Extra Addition: We can also add a voice input/output to the system to implement voice commands.

# Planning
Pipeline for this project can be divided into two subsections:
## Hardware
Here we can figure out dimensions of mirror, display and exterior design. Camera placement must also be determined.  

*Determining dimensions of the mirror-->Finding a suitably sized two-way acrylic mirror-->Finding suitable display--> Forming a rough structure for placement of display, camera and Raspberry pi along with the proper wiring*

## Software
Here there are two parts:
### User interface
We need to write a python program to implement the functions of the smart mirror.  
_Note the background screen colour while the program is running should be adjusted so that the mirror looks uniform_
