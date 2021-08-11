# Serial Communication ESP32 via PC

Python is used in many applications including data science, machine learning, and web development. Another area where we can use Python is external hardware control. A piece of external hardware could be a light or a sensor. External hardware includes multimeters or spectral analyzers. Python is used to control an LED that is connected to an Arduino. Python running on a computer will turn the Arduino LED on and off.

# Requirements

**1. Install Anaconda**

*In your browser, download the Anaconda installer for Linux.*
```
https://repo.anaconda.com/archive/Anaconda3-2021.05-Linux-x86_64.sh
```
*To use GUI packages with Linux, you will need to install the following extended dependencies for Qt:*
```
apt-get install libgl1-mesa-glx libegl1-mesa libxrandr2 libxrandr2 libxss1 libxcursor1 libxcomposite1 libasound2 libxi6 libxtst6
```
*Enter the following to install Anaconda for Python 3.7:*
```
bash ~/Downloads/Anaconda3-xxxx.xx-Linux-x86_64.sh
```
*Enter the following to install Anaconda for Python 2.7:*
```
bash ~/Downloads/Anaconda2-xxxx.xx-Linux-x86_64.sh
```

**2. Install PySerial**

To start a new Python project, best practice is to create a new virtual environment. When you install Anaconda, it comes with the very useful Anaconda Prompt. Using the Anaconda Prompt is a bit like using the terminal Linux. Using the Anaconda Prompt, create a new virtual environment for our Arduino LED project.

```
conda create --name arduino python=3.7

```
The conda create command builds the new virtual environment. The --name arduino flag gives new virtual environment the name arduino. Including python=3.7 ensures the new virtual environment has an up to date version of Python. Type y to confirm and create the new virtual environment. To use the new virtual environment arduino, you need to first activate it by typing:
```
conda activate arduino
```
Install the PySerial package to communicate with the ESP8266 Node MCU using Python.

```
conda install pyserial
```

# Instructions

1. Change the location of device **/dev/USB0** if it is connected at an other address.
2. Change the baudrate **9600** if the baudrate is something else of the connected device.

# ESP32 PinOut

![ESP32 PinOut](https://github.com/syedmohiuddinzia/SerComESP32uino/blob/main/ESP32PinOut.JPG)
