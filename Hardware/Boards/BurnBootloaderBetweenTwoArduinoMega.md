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
| **53 - SS**          | **53 - RESET PIN** |

![Mega-To-Mega](/assets/img/Hardware/boards/BurnBootloaderBetweenTwoArduinoMega/1.png)

3. Open Arduino IDE
4. Click on *Files > Examples > Arduino ISP*
5. ArduinoISP program will open.
6. Make the following changes according to the pin connection.

```C++
#define RESET 53
#define PIN_MOSI 51
#define PIN_MISO 50
#define PIN_SCK 52
```
![code snipet](/assets/img/BurnBootloaderBetweenTwoArduinoMega/1.png)

After changes are made make sure the board selected is mega 2560 and port is selected.

* Upload the code.
* After uploading the code. Go to tools > Programmer > 'Arduino as ISP'.
* Go to tools again > press on 'Burn Bootloader'.  (Takes a few minutes to be done.)



