# Debugging Tutorial for the project

## Instuctions for Raspberry Pi:

Step 1: Download Raspberry Pi Imager on your PC. Insert an SD card and install Raspberry Pi OS(version/bit must be suitable with the Raspberry Pi model) onto the the inserted SD card.  
Step 2: Plug in the SD card into the slot in Raspberry Pi. Make sure it is plugged properly.  
Step 3: Plug in power supply and connect it to a display monitor( not the one for mirror) for testing.   
Step 4: Wait for a few minutes for it to boot up. After that if it still isn't loading then go back to Step 2 and check if all connections are proper.  
Step 5: Configure the Raspberry Pi. Install updates if available. Choose a common default password and set it.  
Step 6: Check if all the dependent libraries are installed, if not install them.  
Step 7: Check if the camera is fully functional. You must enable camera from Raspi-config file. If it doesn't work, try restarting.  
Step 8: Run the a test python script. If it doesn't work, go to step 5.  
Step 9: Run the actual final python scripts. Make sure the program is working properly.
Step 10: Configure the Raspberry Pi to enable the Pi to login automatically without requiring any user intervention. Then configure it to autorun a test python scripts and reboot to check if it works. Else try this again after reinstalling the OS. If it works then proceed to Step 8
Step 11: Configure the Raspberry Pi to autorun the main python scripts each time the Raspberry Pi is booted. This time make sure that the script is running all the time unless it is closed explicitly. Add "&" at the end of file name when adding it for autorun.

End of Instructions.
## Testing Display
Connect the display and turn on supply for the Raspberry Pi. If it doesn't work, then check all connections and try again. If it still persists, then check if its working for inputs from other devices

## Debugging in Python program for facial recognition
Seperate into modules and implement.  
Modules can be:  
Face Detection and seperating it out for further processing
Development of kNN algorthims
User Interface

