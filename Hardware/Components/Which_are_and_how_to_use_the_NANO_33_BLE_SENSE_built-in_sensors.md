# Which are and how can I use the NANO 33 BLE SENSE built-in sensors

### IMU (Inertial Measurement Unit)  
The IMU is a [LSM9DS1](https://www.st.com/resource/en/datasheet/lsm9ds1.pdf) chip that comes integrated in the board. It features a 3-axis accelerometer, 3-axis gyroscope and 3-axis magnetometer. This chip, made by ST Microelectronics, is a standard component supported by our library [ArduinoLSM9DS1](https://www.arduino.cc/en/Reference/ArduinoLSM9DS1) which contains example sketches to use the sensor.

### Digital microphone 
The digital microphone is a [MP34DT05](https://www.st.com/resource/en/datasheet/mp34dt05-a.pdf), this chip, made by ST Microelectronics, is an ultra-compact, low-power, omnidirectional, digital MEMS microphone built with a capacitive sensing element and an IC interface; it produces an output coded in [PDM](https://en.wikipedia.org/wiki/Pulse-density_modulation). The PDM format is supported by our [PDM library](https://www.arduino.cc/en/Reference/PDM) that can be used also with our [ArduinoSound](https://www.arduino.cc/en/Reference/ArduinoSound) which contains example sketches to use the sensor.

### Gesture sensor
The Gesture sensor is a [APDS9960](https://docs.broadcom.com/docs/AV02-4191EN), it senses gesture, color, ambience illumination and proximity. This chip, made by Broadcom is supported by our [ArduinoAPDS9960](https://www.arduino.cc/en/Reference/ArduinoAPDS9960) which includes example sketches to use the sensor for gestures, color and proximity.

### Pressure
The barometer sensor is a [LPS22HB](https://www.st.com/resource/en/datasheet/lps22hb.pdf), is an ultra-compact sensor which functions as a digital output barometer. This chip, made by ST is supported by our [ArduinoLPS22HB](https://www.arduino.cc/en/Reference/ArduinoLPS22HB) library which includes example sketches to measure the atmospheric pressure.

### Relative humidity and temperature
The relative humidity and temperature sensor is a [HTS221](https://www.st.com/resource/en/datasheet/HTS221.pdf), is an ultra-compact sensor that uses a polymer dielectric planar capacitor structure capable of detecting relative humidity variations and temperature, returned as digital output on a serial interface. This chip, made by ST is supported by our library [ArduinoHTS221](https://www.arduino.cc/en/Reference/ArduinoHTS221).
The library contains, as usual, the example sketch to use the sensor to measure the [relative humidity](https://en.wikipedia.org/wiki/Relative_humidity).
