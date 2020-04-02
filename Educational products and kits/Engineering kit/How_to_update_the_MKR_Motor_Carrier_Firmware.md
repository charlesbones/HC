# How to update the MKR Motor Carrier Firmware

If the red led besides the power led is 'ON' while uploading the Motor_test example(Arduino IDE>Files>Examples>Motor_test), it means that the firmware of the MkrMotor carrier has to be updated and in order to update the firmware on the MkrMotor carrier, we recommend you to follow the instructions below:

1. Mount the Mkr1000 on the Mkr motor carrier.
2. Connect the Dc encoder motor and the battery to the carrier.
3. Power the board using the USB cable.Below attached is the picture for references:

![enroll 1](/assets/img/education/AEK_UpdateMKREMotorCarrier1.png)

4. Now, slid the battery power switch to on status.
5. Upload the flasher example (Arduino IDE>Files>Examples>MkrMotor Carrier>Flasher).
6. Open the serial Monitor and check if the firmware is updated successfully.
7. Retry to upload the Motor_test (Arduino IDE>Files>Examples>Motor_test) and check if the Dc encoder motors connected to the carrier are working as expected.
