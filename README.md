# OHTS-Jet-Drone
## Explanation
Jet Drone is a project started and overseen by Mr David Langevin from the Oxford Hills Technical School.
The goal is to produce a working control unit for the base of a wheelchair with single and dual motor control.
Involved are members of both the Pre-Engineering Year 2 class and Computer Technology Year 2 and Year 3 classes.

Above and below are our links/sources to documentation on code, command, and design. Included are the schematics and all code involved (HTML, CSS, JS, Python, and C++)

## Code Usage
*HTML* - HTML was chosen for the web design used to control the drone, included with HTML was some basic CSS and JavaScript for web use.

*CSS/JS* - Additions of the afformentioned HTML for use only in the basic control website.

*Python* - Python was solely chosen for it's simplicity and usage. It is used in the website for communication to the Raspberry Pi/Arduios and for back-end work. It is also used in a simple UI to control the drone from close range using bluetooth or wifi, not including video.

*C++* - C++ is used for most every major component of this project. The Arduino's controlling the motors, the communication between arduino and raspberry pi, and any other background processes required.

## Required Modules
__Python__ - Tkinter, RPi.GPIO, Serial, time, and Flask.

*Tkinter* - ```pip install tkinter```  
*RPi.GPIO* - ```pip install RPi.GPIO```  
*Serial* - ```pip install PySerial```  
*time* - ```pip install time```  
*Flask* - ```pip install Flask```  

## How it works

The Arduino Mega will be connected to the internet via a wifi hat and will have a static IP address configured by the team. Once done a secondary program will be written to connect to the Arduino giving vital control capability. Once that has been done it will be tethered to the web server via internet connection to Raspbery Pi. The Raspberry Pi will be taking secondary inputs from the Arduino via a 4 bit connection. If control becomes impossible via tethered internet connection the Raspberry Pi will assume control sending a full stop command to the Arduino until the error has been assessed and the Raspberry Pi has prepped the Arduino and additional hardware/sensors for it's control. Web based control will then be reconnected VIA internet connection to the Raspberry Pi HOST1.


*Officially licensed under GNU GPLv3 and OHTS-JD License V1**
