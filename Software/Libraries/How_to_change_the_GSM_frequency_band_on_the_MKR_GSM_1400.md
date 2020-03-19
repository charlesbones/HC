# How to change the GSM frequency band on the MKR GSM 1400

## Overview

It is possible to change the frequencies that our GSM 1400 board uses to connect to the mobile network.
Different options are available to configure the frequency bands on which the MKR GSM 1400 can operate.
This tutorial will show all different possibilities to choose frequency band and how to change this setting.

### What you’ll learn

* How to check and change the operating frequency band/s on our MKR GSM 1400

### What you’ll need

* Arduino IDE
* MKR GSM 1400
* USB data cable

## Steps

### Step 0: Check that you have the basics.

* Make sure you have latest SAMD core. If you don’t, go to Arduino ```IDE > Tools > Board > Boards Manager: search for ‘Arduino SAMD Boards’ > Update/Install ```
* Make sure you have the latest update of the MKRGSM’ library: Go to Arduino ```IDE > Tools > Library Manager: search for ‘MKRGSM’ > Update/Install```

### Step 1: Upload the Band Manager sketch.

Go to ```Arduino IDE > File > Examples > MKRGSM > Tools: ‘BandManagement’ ``` and upload it.

![BandManagement Sketch location](/assets/img/software/libraries/change-GSM-1.png)

### Step 2: Manage the board's band frequency

This sketch, for the MKR GSM 1400 board, checks the band currently configured in the modem and 
allows you to change it. Make sure you take note of the current option, you might need to configure
it back to this one. Just open the serial monitor, the current configuration will show after “Current band”.
Following, the list of possible options:

1. E-GSM(900)
2. DCS(1800)
3. PCS(1900)
4. E-GSM(900)+DCS(1800) ex: Europe");
5. GSM(850)+PCS(1900) Ex: USA, South Am.
6. GSM800(800)+GSM(850)+E-GSM(900)+PCS(1900)
7. UMTS(2100)
8. GSM(850)+E-GSM(900)+PCS(1900)+UMTS(2100)

![Band options](/assets/img/software/libraries/change-GSM-2.png)

If you wish to change the band just enter the corresponding number to the option desired 
in the input box and press ‘Send’. Success message will be printed right after (the process 
can take up to 3 minutes).

![Band options](/assets/img/software/libraries/change-GSM-3.png)

You can check [http://www.worldtimezone.com/gsm.html](http://www.worldtimezone.com/gsm.html) to check which band each zone works with.

Usual configurations:
* Europe, Africa, Middle East: E-GSM(900)+DCS(1800)
* USA, Canada, South America: GSM(850)+PCS(1900)
* Mexico: PCS(1900)
* Brazil: GSM(850)+E-GSM(900)+DCS(1800)+PCS(1900)


### Next Steps

Now you have configured the band, get ready and visit [Arduino Project Hub](https://create.arduino.cc/projecthub/search?q=gsm) for inspiration. There are lots of existing projects developed with this board and GSM communication!

