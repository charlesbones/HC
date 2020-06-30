# How to burn the bootloader between two Arduino Mega

This is a tutorial that explains how to burn the bootloader using 2 Arduino Mega. You can do this when the board suddenly stops working after using the board for a while and also as a last resort to see if the new board you got is a faulty board.

## Components required:

* Arduino Mega 2560 - 2
* Jumper wires - 6
* USB 2.0 cable - 1

## Steps to follow:

1. Choose the working board as your programmer.
2. Make the connections according to the below table

| Master (Pin number) 	| Slave(Pin number) 	|
|:-------------------:	|:-----------------:	|
| 50 - MISO           	| 50 - MISO         	|
| 51 - MOSI           	| 51- MOSI          	|
| 52 - SCK            	| 52 - SCK          	|
| **53 - SS**          | **RESET PIN** |

![Mega-To-Mega connection](/assets/img/hardware/boards/mega-to-mega_connection.png)

3. Open Arduino IDE
4. Click on *Files > Examples > Arduino ISP*
6. In the *ArduinoISP* example, make the following changes according to the pin connection.

![ArduinoISP example](/assets/img/hardware/boards/ArduinoISP_Example.png)
[Link to example](https://create.arduino.cc/example/builtin/11.ArduinoISP%5CArduinoISP/ArduinoISP/preview?embed&snippet=L68-L89&hidenumbers#L73,L85-L87)


After changes are made make sure the board selected is mega 2560 and port is selected.

* Upload the code.
* After uploading the code. Go to `Tools > Programmer > Arduino as ISP`.
* Go to tools again > press on 'Burn Bootloader'.  (Takes a few minutes to be done.)
