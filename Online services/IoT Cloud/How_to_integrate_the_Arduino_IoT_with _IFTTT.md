# How to integrate the Arduino IoT with IFTTT

## Overview:

This article is to show how to connect your Arduino IoT device cloud and get the data you want to collect from the cloud to your personal mail.

### Hardware Requirements:

* Mkr Wifi 1010
* Mkr ENV shield
* USB cable 2.0

### Software Requirements:

* Arduino Create account.
* IFTTT - [If This Then That](https://ifttt.com/)

## Steps

### 1 - IoT CLOUD setup:

1. Mount **MKR ENV Shield** onto an **MKR WIFI 1010** board.
2. Connect it to your computer using a USB cable.
3. Add your MKR 1010 board to the create Device Manager
4. Go to the **Arduino IOT cloud** in [Arduino Create](https://create.arduino.cc/).
5. Select the option **New Thing**.
6. Then, provide a name for your new thing and inside select the board drop-down menu, choose to **configure a new device**.
7. Later, the page redirects you to setup and configure a new device into the IoT cloud.
8. Once the board configuration is done, we should set up the new thing.
9. Select the **ADD Properties** option on the right side of the page.
10. Inside the properties page, add all the properties required for the project and save it.

    ![](/assets/img/online/iot/ifttt_1.png)

11. Click on the Edit sketch option on the top right side corner.
12. In order to activate the ENV shield, you must add the below code inside the Void setup.
    ```
    while (!Serial);
       if (!ENV.begin()) {
        Serial.println("Failed to initialize MKR ENV shield!");
        while (1);
      }
     ```
13. In the Secret tab, provide the **SSID** and **Password**.

    ![Secret tab](/assets/img/online/iot/ifttt_2.png)

14. Now, **upload** and **run** the sketch.       
15. Open the serial monitor and check if it is connected to the internet and also if the values are changing to the given variables.
16. Once the process is done, click on the IoT cloud tab and go to the dashboard to see the property values.

    ![Property dashboard](/assets/img/online/iot/ifttt_3.png)

### 2 - IFTTT setup:
1. Go to the link create IFTTT page [here](https://ifttt.com/create) and create a new applet.
2. Select the option **if +this** and choose webhooks

   ![IFTTT "+This" option](/assets/img/online/iot/ifttt_4.png)

3. Add a trigger inside your webhooks.
4. Select ‘**receive a web request**´ option and give your event name which should be the same name given to thing in IoT Cloud.
5. And then create the trigger.
6. Now, click on **+that**, choose email, enter the details

   ![IFTTT "+That" option](/assets/img/online/iot/ifttt_5.png)

7. Enter the received pin and select connect.
8. In the ‘**complete action field**’ press save creating an applet
9. Go to my services page, click on **Documentation** on upper right

   ![Event trigger information](/assets/img/online/iot/ifttt_6.png)

  >**Note**: Inside complete action field ‘eventname’ refers to the thing name to be triggered from IoT, val1 refers to the variable name, val2 refers to the reading or value and val3 refers to the timestamp. And you don’t have to fill it up.

10. Copy the link until ‘**event**’ copies it on the webhooks section of the IoT cloud and put the name of the thing to be published over IFTTT.
11. Copy the rest of the link from the Documentation page.
12. Click on **test it**.
13. You should start receiving emails.

## Checkpoint!

1. If you don't start receiving emails, we recommend you to check the following instructions:
2. Check the link provided in the webhooks section (step 10 in IFTTT steps).
3. Make sure you have assigned the correct event name (event name should be the same as the thing name inside the trigger).
4. Check the mail Id you have provided  (step 6 in IFTTT steps).
