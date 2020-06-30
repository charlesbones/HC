# How to connect the Arduino SAMD Boards to Arduino create

## Overview
This article provides you the details on how to connect SAMD boards to the Arduino cloud, it applies to the following boards:

* Nano 33 IoT
* MKR 1000
* MKR 1010

## Requirements:
* Arduino SAMD board
* Internet Connection
* USB cable
* Arduino Account

## Steps

1. Log in to your Arduino account connected with Maker Plan.
2. Go to your account's [Device Manager](https://create.arduino.cc/devices/).

3. Scroll down to `MY ARDUINO BOARDS` and click on `ADD NEW BOARD`.

  ![Device manager "Add new"](/assets/img/online/create/Devices_newArduinoBoard.png)

4. Under 'Setup an IoT Board' look for your board and click on it.

  ![](/assets/img/online/create/Devices_ChooseArduino.png)

5. The board configuration part will start once you click on the `START`.

    ![](/assets/img/online/create/Devices_SAMDStart.png)

    > In these images, you will see we use the Arduino Nano 33 IoT, but these same steps are the ones taken for any of the SAMD boards listed at the beginning.

6. Give a personalized name for the board for easy understanding.

  ![](/assets/img/online/create/Devices_SAMDNaming.png)

7. You will reach the Configuration page which will set up the board to connect to the Arduino cloud. Click on ‘Configure’.
  >  This will take a few minutes to complete.

 ![](/assets/img/online/create/Devices_MKRWANConfiguration.png)

8. After the configuration is done you will be taken to a sample sketch that can be uploaded to test out the connection with Arduino IoT Cloud. Click on `Enter WiFi Data`.

  ![](/assets/img/online/create/Devices_SAMDWiFiSketch.png)

9. Under the Secrets Tab, you will have to add your WiFi name and Password for your network connection. Click on `Upload`.  

  ![](/assets/img/online/create/Devices_SAMDWiFiCredentials.png)

10. After the code is uploaded you will be taken to the ‘Your Board is Connecting to Cloud’ step.
  > This may also take a few minutes to complete. If this part fails you have to enter the WiFi data and upload the sketch again.

  ![](/assets/img/online/create/Devices_SAMDWiFiCheck.png)

11. Once the Connection to the Arduino Cloud is established it will take you to an interactive page where you can control the LED on the board by sending ’ON’ and ‘OFF’ commands.

  > If the LED is not turning ON when you pass the command then that means the board is not connected to the Cloud, please chech both the WiFi credentials and the internet connection to said Wifi network.

  ![](/assets/img/online/create/Devices_SAMDPlay.png)

12. After testing you can click next which will take you to the confirmation of successful connection to Arduino IoT cloud.

  ![](/assets/img/online/create/Devices_SAMDReady.png)

13. Once you receive this message you can click and go to the device manager to view the board added to your Arduino boards section, ready to be used in your Arduino cloud-based projects.



**Author:** Joyal John

**Reviewed By:** Judit M. Villadangos - 30/June/2020
