# lgpio-InputButton
Project with lgpio library with the Raspberry Pi to accept an input signal from a physical switch.

This example uses the latest and most compatible library for the Raspberry Pi in Xojo 2023 r1.1. The Xojo library can be downloaded for free at: https://github.com/eugenedakin/lgpio-GPIO. This is a lgpio local library that is a replacement for the deprecated sysfs library that
is to be used with Xojo apps. This library uses local c language calls, which means updates should be minimal and your code should be stable for a very long time. 

![](https://github.com/eugenedakin/lgpio-InputButton/blob/main/LibGPIODInputScreenGrab.png)

Below is an electrical schematic for the input button project.

![](https://github.com/eugenedakin/lgpio-InputButton/blob/main/InputSchematic.png)

The lgpio library can be installed Raspberry Pi OS (5 July 2023) and instructions 
are available at http://abyz.me.uk/lg/download.html

Install instructions are:
1) sudo apt install swig python3-dev
2) sudo apt install python3-setuptools
3) sudo apt-get install libunwind8
4) wget https://github.com/joan2937/lg/archive/master.zip
5) unzip lg.zip
6) cd lg
7) make
8) sudo make install
9) create a Blink example program and copy the program and libraries to the RaspberryPi Desktop
10) give the executable permission to run with something like: 'sudo chmod +x LibGPIODInput'
11) run the program with something like: 'sudo ./LibGPIODInput'

This example project uses the lgpio libray and executes a loop to search for a signal from a physical button with an input electronic pin port on the Raspberry Pi.
