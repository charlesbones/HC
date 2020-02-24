# Import Your Sketchbook and Libraries to the Web Editor

It is possible to import easily all your sketches and libraries from Arduino IDE (desktop Arduino software) to Arduino Web Editor (online version of Arduino IDE) in just a few clicks. This comes very handy as all your projects will be saved in the cloud and are accessible from any computer.

In addition, Arduino Web Editor allows you to import sketches and files in the following formats:

Single sketches in .ino, .pde and .zip format.
Libraries in .zip format.
Zipped folders containing sketches and libraries.

Make sure your libraries are in a folder called ‘libraries’. Be sure not to mix sketches and libraries in the same folder. But let’s import your whole sketchbook in a few clicks, so you will be all set up to start using the Arduino Web Editor.

![import 1](/assets/img/ImportYourSketchbookandLibrariestotheWebEditor/1.gif)

## 1. Find your sketchbook
On your PC find out where your sketchbook folder is (it is called ‘Arduino’, unless you renamed it) and you will find it under the following directory:
Windows: it’s usually under My Computer/Documents/Arduino
Mac: User/Documents/Arduino, and on Linux is $HOME/Arduino.

## 2. Zip your sketchbook
Make a .zip pack of your sketchbook, you should obtain a file called Arduino.zip. Make sure it is .zip format, any other archive formats will not work.

![import 2](/assets/img/ImportYourSketchbookandLibrariestotheWebEditor/2.jpg)

## 3. Import your sketchbook to the cloud
Go to create.arduino.cc/editor. When you are logged in and ready, hit the import button on the sketchbook panel. A popup with some instructions on how to import files into the Web Editor will be displayed. Press “Import” to continue.

You will now see a file system window, select your Arduino.zip pack. Wait for the import process to finish. If your sketchbook is big (containing lots of files), this may take a while.

![import 3](/assets/img/ImportYourSketchbookandLibrariestotheWebEditor/3.jpg)

## 4. You are done!
Once the import process is done there will be two reports, one for sketches and one for libraries.

If you already have sketches with the same name on the online IDE, these sketches will fail to import to avoid conflicts.

If you have libraries in your sketchbook, another report will tell you those that got successfully imported. If you have existing custom libraries with the same names, it’ll prompt you to overwrite the existing ones. Be sure to proceed with caution!

![import 4](/assets/img/ImportYourSketchbookandLibrariestotheWebEditor/4.png)
