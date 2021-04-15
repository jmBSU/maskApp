

# Mask Data Terminal

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

This is the companion app for the MASK project code found [here](https://github.com/jmBSU/maskTest).

---
## Requirements
* Android only
* Android 4.3+
* BLE 4.0+ compatible
---
## Original App

This app is a repurposed version of SimpleBluetoothLETerminal: [Github](https://github.com/kai-morich/SimpleBluetoothLeTerminal)

---
## Major changes
* Cosmetic
    * Terminal page no longer shows a terminal
    * Changed terminal to multicolored display page
* Data representation
    * App no longer displays all serial data
    * Data is parsed from the data sent from the MASK project code
    * Only the numeric values is kept and displayed.
    
---
## Incoming Data Format
This is the C/C++ code from the MASK project code: 

    sprintf(strToPrint, "Temp: %d \n HR: %d \n SPO2: %d \n", tempTemperature, tempheartRate, tempspo2);

where the format is:

    Temp: %d \n HR: %d \n SPO2: %d \n

and each %d corresponds to the data value that precedes.

