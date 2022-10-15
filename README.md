# ESE-5190-Lab2-SetUpGuide

This guide describes the steps for getting started with setting up **C/C++ SDK** development environment to communicate with Adafruit QT Py RP2040.

### **System Specifications**
1. Processor - AMD Ryzen 7 5700U
2. OS - Windows 11 Home
3. RAM - 8GB

### Basic Installations Required:
1. Terminal:
You can use any terminal of your liking. I have used pre-installed windows terminal. 

2. Text Editor:
I have used VS Code. You can download it through the link attached: [Download Visual Studio Code](https://code.visualstudio.com/download). Vim is also a good alternative. ( [Vim Text Editor](https://vim.en.softonic.com/) )

3. Serial Console:
I have used Putty as my serial console to connect to the RP2040's REPL. Follow the Adafruit tutorial for your machine here: [Advanced Serial Console](https://learn.adafruit.com/welcome-to-circuitpython/advanced-serial-console-on-windows)
</br>
After installation, check Device Manager -> Ports (COM and LPT). Check the port of your USB connection. Open Putty -> Connection Type: Serial, Baud rate: 115200. 
</br>
Enter and save the required specs in a file to re-load it anytime in the future.
Click ‘Open’ to open the PuTTy program terminal.
PuTTy is all set to be used.

![image](https://user-images.githubusercontent.com/114099174/195966562-34c876a4-23a5-42e7-8b84-177f66df5566.jpeg)



### Useful References:
1.[Raspberry Pi Pico C/C++ SDK - Libraries and Tools](https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf)

2.[RP2040 Datasheet](https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf)

3.[Getting Started  with Raspberry Pi Pico](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf)

Tools required for successful installation and setting up the board to work with C/C++ SDK:
1. [Arm GNU Toolchain](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads)
2. [CMake](https://cmake.org/download/)
3. [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022)
4. [Git](https://git-scm.com/download/win)

After the necessary installations and lookups to references, you need to clone the github repository using following commands:

```
$ cd ~/
$ mkdir pico
$ cd pico
```
Then clone the **pico-sdk** and **pico-examples** git repositories.
```
$ git clone -b master https://github.com/raspberrypi/pico-sdk.git
$ cd pico-sdk
$ git submodule update --init
$ cd ..
$ git clone -b master https://github.com/raspberrypi/pico-examples.git
```
Next Set Environment variables:








