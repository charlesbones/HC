# Arduino.h error in Matlab or simulink

Firstly, you will need to install  five Add-ons which are used in the Arduino engineering kit projects.
After installing the 5 Add-ons if you receive a **fatal error:0 `Arduino.h: No such file or directory #include "Arduino.h" ^ compilation terminated`** follow the instructions below.
## Instructions:
1. Type `arduinoio.PackageRoot` on MATLAB Command Window, this will tell you the Arduino Support Package root location.

  For example – `C:\ProgramData\MATLAB\SupportPackages\R2019a\3P.instrset\arduinoide.instrset\idepkgs `.
2. Uninstall both MATLAB and Simulink support packages for Arduino by selecting Add-Ons from the MATLAB Toolstrip as shown in the image below and click on manage Add-Ons.
  ![Add-ons](/assets/img/education/AEK_ArduinohError1.jpg)

3. Next go to this location and ensure no more files are left, and feel free to delete any left over.
4. Then close MATLAB and right click on MATLAB icon and select ‘Run as administrator’
5. Reinstall both support packages.
