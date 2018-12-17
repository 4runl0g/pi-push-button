# pi-push-button
Installing the RPi.GPIO Library
In order to read the tactile pushbutton switch status, the RPi.GPIO library needs to be installed on the Raspberry Pi. The RPi.GPIO  is a software module that conveniently allows the Raspberry Pi GPIO pins to be manipulated for electronic controls applications. To install the RPi.GPIO library onto the Raspberry Pi, open the LXTerminal and type the following Linux installation command after the prompt:

pi@raspberrypi ~ $ sudo apt-get install python-dev python-rpi.gpio

After the Linux installation command is entered, you will see a series of RPi.GPIO build-installation file sequences being displayed on the monitor as shown below.

Once the build is complete, the RPi is ready for reading the status of a tactile pushbutton switch.

Wiring the Tactile Pushbutton Switch to the RPi
Attaching a tactile pushbutton switch to the RPi is quite easy to do. An important item to remember is the RPi's GPIO pins are +3.3VDC compliant. Applying voltages greater than +3.3VDC will damage the RPi. The electrical wiring diagram for attaching the tactile pushbutton switch is shown next.

As an additional project build material, I included an equivalent circuit schematic diagram for reference below.

Although, the circuit wiring to the RPi is quite simple, recheck the wiring before programming the RPi. This important verification step will assure you project execution success when the python code is installed and running on the RPi. 

The Programmable Switch Python Script
The next phase of the project build is to provide a python script for reading a tactile pushbutton switch wired to an RPi GPIO pin. The python script for reading a tactile pushbutton switch is shown next.

You can enter this script using either the LXTerminal's nano editor or with the Python's IDLE (Integrated Development Environment). Save the script as pbbutton.py in the home/pi directory of the RPi. Next, type the following Linux command to run the script on the RPi into the LXTerminal as shown next.

pi@raspberrypi ~ $ sudo python pbbutton.py

Next, press the tactile pushbutton switch. If the script was typed correctly, you will see the message "button press" displayed on the monitor's screen. Congratulations on building a programmable pushbutton switch!

For additional build reference, check out the video clip below.

The tactile pushbutton switch can easily be programmed to provide a variety of output messages and switching responses. Try changing the "Button Press" message to display your name or a whimsical word when activating the switch. Record your results in a laboratory notebook. In the next project article, you will learn how to code the RPi to toggle a LED on and off using your programmable pushbutton switch.
