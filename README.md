# Arduino Nano33 BLE Applied Emotion Classification Based on the Playing Motion of Musical Instruments  
## Yuanlong Chen  
### ECE_M202A_project (UCLA ECE FALL 2022)
## Abstract  
## Instructions:  

Hardware: Arduino Nano33 BLE  
  
Software: Edge Impulse  
  
Before Running:  
1. For Mac：Add ‘arduino-cli’ into your path by following the instruction from https://osxdaily.com/2014/08/14/add-new-path-to-path-command-line/  
2. For Mac: To connect to your Nano33 BLE, following the instruction from https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense, then check that whether the Nano33 BLE board has been detected in the serial port.  
3. Attach the Nano33 BLE board onto the player's wrist.  

How to run on Nano33 BLE board: (For Mac)  
1. Choose a folder in software (for example: clarinet_lefthand-nano-33-ble-sense-v2), double click the flash_mac.command file to flash the firmware of trained model into the connected Nano33 BLE board.  
2. Open a new terminal, and type in the command: edge-impulse-run-impulse
3. Then the modal would run automatically with refreshing detection of emotion each five seconde.  
4. Now it is time for the player to play, and keep checking the feedback of emotion in ratio (for example: happy 0.54, angry 0.33, sad 0.13)  

### Use the folders as follows:

* [docs](docs) for the website contents (report, media).
* software/ for files used for deploying the model on Nano33 BLE board or Arduino Library.
* data/ for the collected motion data from music instruments of Piano, Violin, Drum, and Clarinet.

### Links:  
Demo Video:  
https://drive.google.com/file/d/1UJw4sF4zUcUYsoU1NJBmmMxS5ZUQhkQN/view?usp=sharing  

Slide:  
https://docs.google.com/presentation/d/1xzd-4Lvj697t_955xlcXllmiTQB8dc0Xl4lTnfAXUJA/edit#slide=id.p1  

Website:  
https://jaychen9909.github.io/eceM202A_project/

