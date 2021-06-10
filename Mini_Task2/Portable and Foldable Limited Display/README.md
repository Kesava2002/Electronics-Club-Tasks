# Analysis of the project:
## Problem Statement
To create and cheap, portable, foldable display with limited uses like scorecards, timers that can be configured using an Android Application.

![image](https://user-images.githubusercontent.com/84671311/121397933-71585080-c972-11eb-8b35-146960d79330.png)

## Ideation
This display can be created by using WS2812B strips connected to a ESP8266 microcontroller with Bluetooth and Wifi features. The microcontroller would be controlled from an Android application.  
Basics connection of a WS2812B strip:  
![Screenshot from 2021-06-10 09-50-33](https://user-images.githubusercontent.com/84671311/121464487-93cd8680-c9d1-11eb-843f-916e832d2361.png)

### Configuring the LEDS

For configuring the LEDS, we can use FastLED library. This is an example code snippet for a WS2812B with 20 LEDS connected an Arduino at pin 7.  
```
#include <FastLED.h>  

#define LED_PIN     7 
#define NUM_LEDS    20  

CRGB leds[NUM_LEDS];  

void setup() {  

  FastLED.addLeds<WS2812, LED_PIN, GRB>(leds, NUM_LEDS);  
  
}  

void loop() {  
  
  leds[0] = CRGB(255, 0, 0);  
  FastLED.show();  
  delay(500);    
  leds[1] = CRGB(0, 255, 0);  
  FastLED.show();  
  delay(500);  
  leds[2] = CRGB(0, 0, 255);  
  FastLED.show();  
  delay(500);  
  leds[5] = CRGB(150, 0, 255);  
  FastLED.show();  
  delay(500);
  leds[9] = CRGB(255, 200, 20);
  FastLED.show();
  delay(500);
  leds[14] = CRGB(85, 60, 180);
  FastLED.show();
  delay(500);
  leds[19] = CRGB(50, 255, 20);
  FastLED.show();
  delay(500);
}
```  

Here we can control each LED in the strip seperately!  
We can now configure many number of strips and turn them on/off to our convenience.  

### Receiving data via Bluetooth

We need to establish an serial communication between the bluetooth segment and the microcontrollers. Then we have to configure the mobile application to send data to the bluetooth segment via the bluetooth connection.

## Planning

### Parts of Pipeline
|Part                                                        | Feasibility                                     | Means to improve                         |
|------------------------------------------------------------|-------------------------------------------------|------------------------------------------|
| Configuring WS2812B LED strips                             | Simple                                          | Cost Reduction is possible               |        | Establishing Bluetooth serial communication channel        | Medium Difficulty                               | Better range/quality modules             |        | Designing an Android application with user interface       | Difficult                                       | -                                        | 
| Controlling the microcontrolller using the Android app     | Difficult                                       | Cost reduction, implementing             | 
     
## Prototyping Phase

Application designing and establishing proper connection between the microcontroller and the application, will be the major "headaches" during this phase. Working of LED strips can easily be checked. If any one LED isn't properly functional, it can be easily removed and the other parts can be combined.  




 
