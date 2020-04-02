# How to update the WiFi Nina firmware

This tutorial shows the step by step process on how to **Check the Firmware** and **Update the Firmware** of the WiFi Nina Module available on the board.

This are the boards that have a WiFi Nina module: 

* MKR WiFi 1010
* MKR Vidor 4000 (Add Vidor peripherals library)
* MKR 1000
* Nano 33 IoT
* Arduino UNO WiFi Rev2

## To check the version of the firmware.

1. Connect the board to the laptop or PC
2. Go to *Files > Example > WiFi Ninna > Tools > Select ‘CheckFirmware Version’*

![Example location](/assets/img/hardware/boards/ninaUpdate1.png)

3. Select the board and port number under tools.
4. Upload the sketch to the board.
5. After uploading the sketch, open the Serial Monitor to see the version.

![Serial monitor](/assets/img/hardware/boards/ninaUpdate2.png)

## To update the version of the firmware.

1. Click on *Tools > WiFi101/WiFiNinna Firmware updater*

![Example location](/assets/img/hardware/boards/ninaUpdate3.png)

2. The updater tool will open, select the board inside the box. If there are no listed boards with their port number, press ‘Refresh List’ button.

![Example location](/assets/img/hardware/boards/ninaUpdate4.png)

3. Once you select the board make sure you are updating to the latest version by checking under the drop-down option (this shows all the available version of firmware).
![Example location](/assets/img/hardware/boards/ninaUpdate5.png)

4. Click on *Open Updater Sketch*, then select the board and port under the Tools section. Upload the sketch.
(You can also open the Updater Sketch by following the steps *Files → Examples → WiFiNinna → Tools → FirmwareUpdater*)

![Example location](/assets/img/hardware/boards/ninaUpdate6.png)

5. After uploading the sketch to the board, press Update Firmware Button.

![Example location](/assets/img/hardware/boards/ninaUpdate7.png)

6. The Update will take about a minute to complete. Once the update is done you will get a message like shown below.

![Example location](/assets/img/hardware/boards/ninaUpdate8.png)

