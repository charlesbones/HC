# How to connect the Arduino MKR WAN to Arduino create

## Overview
This article is about how you can connect the Arduino MKR WAN boards you have to the Arduino cloud, it applies to the following boards:

* MKR WAN 1300
* MKR WAN 1310

## Requirements:
* Arduino MKR WAN board
* Internet Connection
* USB cable
* Arduino Account

## Steps

1. Log in to your Arduino account connected with Maker Plan.
2. Go to your account's [Device Manager](https://create.arduino.cc/devices/).

3. Scroll down to `MY ARDUINO BOARDS` and click on `ADD NEW BOARD`.

  ![Device manager "Add new"](/assets/img/online/create/Devices_newArduinoBoard.png)

4. Under 'Setup an IoT Board' look for your MKR WAN board and click on it.

  ![](/assets/img/online/create/Devices_ChooseArduino.png)

5. The board configuration part will start once you click on the `START`.

    ![](/assets/img/online/create/Devices_MKRWANStart.png)

  > Make sure the board is connected to the computer you are using to add this board to your Create-Device manager configuration process. In these images, you will see we use the MKR WAN 1310, but these same steps are the ones taken for the MKR WAN 1300.

6. Give a personalized name for the board for easy understanding.

  ![](/assets/img/online/create/Devices_MKRWANNaming.png)

7. After clicking on the register button you will be taken to a page with a sketch where the only thing needed is to click on ‘Enter Connectivity Data’.

  ![](/assets/img/online/create/Devices_MKRWANDataSketch.png)
  [//]: # (SMALL IMAGE!)

8. You will be taken to the secret tab of the sketch which shows SECRET_APP_KEY and SECRET_APP_EUI.

  ![](/assets/img/online/create/Devices_MKRWANCredentials.png)

9. Click on upload and wait till you get the success message

  ![](/assets/img/online/create/Devices_AddDone.png)

10. Once you receive this message you can click on go to device manager to view the board added to your Arduino boards section.

  ![](/assets/img/online/create/Devices_MKRWANInBoards.png)

11. You have completed the setup of added MKR WAN board to the Arduino Create Device Manager.


**Author:** Joyal John

**Reviewed By:** Judit M. Villadangos - 29/June/2020
