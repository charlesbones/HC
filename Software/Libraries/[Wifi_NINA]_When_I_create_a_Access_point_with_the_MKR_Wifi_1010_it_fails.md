
# [Wifi NINA] When I create an access point, it fails
AP_SimpleWebServer is a simple web server to manage a LED with AP features. The boards which support the WiFi Nina library are MKR 1010, UNO WiFi rev2, Nano 33 IoT, and MKR VIDOR 4000.  After Uploading of the  AP_SimpleWebServer sketch under the WiFiNina library(IDE>File>Examples>WiFINina>AP_SimpleWebServer), if the serial monitor shows an error of “Create access point failed”, then follow the guidelines below:

![](/assets/img/software/libraries/nina_1.png)

 
**Initialize the Parameters as below:**
 
**ssid:** the SSID (Service Set Identifier) of the created Access Point.
**passphrase:** optional, the WPA password of the created Access Point.
 
**Note:** The ssid and passphrase “Must be 8 or more characters.” Otherwise the serial monitor will display an error “Creating an Access Point failed”. 
 
* Upload the Ap_SimpleWebServer sketch again under the WiFi Nina library.  
![](/assets/img/software/libraries/nina_2.png)

* Now, the board needs to connect to the WiFi named with SSID: “abcdefgh” in your WiFi networks.
* Once, the board is connected over WiFi. Open the web browser and enter the IP address.
![](/assets/img/software/libraries/nina_3.png)
* Finally, the LED of the board can be controlled over the WiFi network. 
 
 

