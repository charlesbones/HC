# Arduino.h error in Matlab or simulink

Firstly, you will need to install  five Add-ons which are used in the Arduino engineering kit projects.
After installing the 5 Add-ons if you receive a **fatal error: Arduino.h: No such file or directory #include "Arduino.h" ^ compilation terminated** follow the instructions below.
## Instructions:
* Type arduinoio.PackageRoot on MATLAB Command Window, this will tell you the Arduino Support Package root location.
  Example – ```C:\ProgramData\MATLAB\SupportPackages\R2019a\3P.instrset\arduinoide.instrset\idepkgs ```.
* Uninstall both MATLAB and Simulink support package for Arduino by selecting Add-Ons from the MATLAB Toolstrip as shown in the image below and click on manage Add-Ons.
  ![Add-ons](/assets/img/education/Arduino.h_1.jpg) 
 
* Next go to this location and ensure no more files are left, and feel free to delete any left over.
* Then close MATLAB and right click on MATLAB icon and select ‘Run as administrator’
* Later, reinstall both support packages.
