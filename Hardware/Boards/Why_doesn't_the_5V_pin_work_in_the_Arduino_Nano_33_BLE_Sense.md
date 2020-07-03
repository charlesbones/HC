# Why doesn't the 5V pin work in the Arduino Nano 33 BLE Sense

The 5V pin comes disconnected by default on your NANO 33 BLE SENSE. It has been developed this way as a precaution, since previous Arduino boards use 5V I/O signals. This way users will not accidentally damage the board by powering their circuits with 5V instead of 3.3V.

5V on that pin is available only when two conditions are met:

1. You make a solder bridge on the two pads marked as VUSB (image below)

  ![Example location](/assets/img/hardware/boards/Nano5V1.png)

2. You power the NANO 33 BLE Sense through the **USB port**.
   If you power the board from the VIN pin, you won’t get any regulated 5V and therefore even if you do the solder bridge, nothing will come out of the 5V pin.

Therefore, if your design requires 5V and you plan on powering it using the Arduino board, it won’t work until  the VUSB pads at the back of the board are connected.
