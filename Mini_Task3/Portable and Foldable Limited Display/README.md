# Debugging Tutorial for the project

## LED strips
WS2812B contains easily addressable LEDs. This makes it easier to control a specific LED without disturbing others. This strip also has LED driver ICs embedded along the the LED. This helps in removing, extending the strip easier.  

| Type of Error                                                  | Fix                                                                                             | 
|----------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| LED strip doesn't light up at all                              | Check if supply voltage and current are suitable for the LED strip, and confirm if the power supply is working. Then test the strip after removing any accesories like dimmers, controllers etc. Check for any loose connections or visible short circuits. Short circuit can be easily detected by the rapid heating of the LEDs and connecting wires. Check the resisitance between positive and negative terminals of a LED. If is is finite, it may imply a short circuit. If problems still exist, try removing LEDs at the edges and trying again |
| Change in colour at the end of the strip                       | This occurs due to loss in voltage across the LEDs. Suggested fix is to connect a wire at the end of the LED strip that acts like a feedback, regulating the drop in the voltage. This is known as power injection |
| LEDs are loosing brightness over time                          | This might possibly due to the drop in input voltage. If the problem is still there, this suggests that the LEDs are defective by design |
| Few LEDS don't light up                                        | This can be fixed by reconnecting the LED segment to the adjacent LEDs                          |

## Bluetooth Connection
Give test signals and print them on the serial monitor. Make sure that variable names and baud rates are properly given. Make sure the TX and RX connections are properly made. If it is working only for short time, then there's improper supply to the bluetooth module. We need to give supply voltage from external source to the arduino. 

## Microcontroller Code
Make sure that proper delays are added inbetween to avoid any congestion. Make sure that you unplug RX and TX connections when you burn the code onto the device.
If the device is hot and you can't burn any code, it means that the microcontroller is damaged. You might have to change devices.


