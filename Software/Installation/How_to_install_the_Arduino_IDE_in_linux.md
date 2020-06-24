# How to install the Arduino IDE in linux

> **WARNING!**
>
> If you use `sudo apt-get install arduino`  you will probably get an extremely outdated and possibly non-standard version of the Arduino IDE.

## Step 0:

Before starting, make sure that you have the latest version of the IDE from the download page. Also, choose the right version according to your setup (32, 64 or ARM).

> Note: If you are not sure about the bit-width of your operating system you can open a terminal window and use the command uname -a.
> * If the outcome contains x86, download the 32 bits version.
> * If the outcome is x64 or x86_x64 download 64 bits version.
> * If the outcome contains arm please check [this table](https://en.wikipedia.org/wiki/ARM_architecture#Cores) to confirm the version.

Now that you have downloaded the correct version of the IDE, it is time to move on into the installation process. Follow the steps below:

## Step 1: extract the package.

 Double click over the file or use the terminal to extract the content of the file you just downloaded, however make sure you place the content of the package in a suitable place for example the Home folder, since it will be executed from there.

## Step 2: find the install script.

Inside the folder you just extracted you will find a file called install.sh, right click over this file and select properties. Under the Basic tab you will see the Parent Folder. This path will be used in the next step.

![IDE folder](/assets/img/software/installation/IDE-Linux1.png)

## Step 3: run the install script.

1. Open a terminal window and use the cd command together with the path that you found in the previous step and press enter. It should look something like:
   `cd /home/USER/arduino-1.8.10`. Note that you should change the version number according to the one you are installing.
2. Type `./install.sh` and enter. In case you get a permission denied message, please execute the command as administrator together with your password, using the following line: `sudo ./install.sh`.
3. Wait until the process finishes.


At the end of this process, you will get the desktop icon and the serial port communication setup.

Additionally, in some cases the desktop icon seems to be broken, however by double clicking and accepting that you trust the application, you will be able to see the Arduino icon on your desktop.
