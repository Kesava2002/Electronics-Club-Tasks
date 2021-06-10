# Analysis of the project:
## Problem Statement
To create and cheap, portable, foldable display with limited uses like scorecards, timers that can be configured using an Android Application.

![image](https://user-images.githubusercontent.com/84671311/121397933-71585080-c972-11eb-8b35-146960d79330.png)

## Ideation
This display can be created by using WS2812B strips connected to a ESP8266 microcontroller with Bluetooth and Wifi features. The microcontroller would be controlled from an Android application.  
Basics connection of a WS2812B strip:  
![Screenshot from 2021-06-10 09-50-33](https://user-images.githubusercontent.com/84671311/121464487-93cd8680-c9d1-11eb-843f-916e832d2361.png)

For configuring the LEDS, we can use FastLED library.
'''  
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
'''

 
