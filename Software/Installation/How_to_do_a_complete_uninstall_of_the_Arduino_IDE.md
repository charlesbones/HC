# How to do a complete uninstall of the Arduino IDE

The Arduino IDE uses files in three locations on your computer:
* IDE installation folder
* Sketchbook folder, located in the Arduino IDE at *File > Preferences > Sketchbook location*
* Data folder
  * On Windows
    * Standard IDE:
     `C:\Users\{username}\AppData\Local\Arduino15`
    * Windows app:
      `C:\Users\{username}\Documents\ArduinoData\packages`
  * macOS: `/Users/{username}/Library/Arduino15`
  * Linux: `~/.arduino15`

When you use the uninstaller, **only the IDE installation folder** will be removed, so after reinstalling, the files left over in the other locations will still affect the new installation.

Deleting the data folder can often solve problems with the Arduino IDE not starting or failing compilation in unexpected ways.

1. Look for the data folder Arduino15 (depending on OS) which is usually hidden and delete it.
   In order to show the hidden folders, you can check the box in: *Start > File explorer > View > Show/hide advanced settings > check Hidden items*

2. Now, you can uninstall the Arduino IDE and no files will be left.
