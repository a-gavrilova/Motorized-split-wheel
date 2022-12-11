# Motorized-split-wheel

I study Purkinje cells activity in cerebellum of mice undergoing locomotion adaptation task. I designed a behavioral setup consisting of 2 motorized wheels and head-fixation system. This method can be combined with various methods, allowing to record neuronal activity, such as regular two-photon calcium imaging, voltage imaging and electrophysiological recordings. 

Here is the hardware used and software developed for such behavioral setup.

## Hardware

1. https://teknic.com/model-info/CPM-SDSK-2310S-EQN/  Servo motor
2. https://teknic.com/ipc-5/    power supply
3. https://teknic.com/products/io-motion-controller/clcr-4-13/  ClearCore Controller
4. https://teknic.com/IPC35-CABLE110/   1 cable from power supply to the general power supply
5. https://teknic.com/CPM-CABLE-PWR-MS120/  2 cables from power supply to the motors
6. https://teknic.com/CPM-CABLE-CTRL-MU120/  2 cables from ClearCore Controller to the motors
7. https://teknic.com/CPM-CABLE-USB-120/      2 cables from motor to the PC (for calibrating motors)
8. https://teknic.com/CC-3TERM-PLUG-10PC/     
9. https://teknic.com/CPM-CABLE-USB-120AB/    from ClearCore Controller to the PC
10. https://teknic.com/PWR-IO-24VDC/        24 VDC power supply (I used analog from Amazon



## Software

All the programs used for calibration and running motors can be downloaded from the main ClearCore website: https://teknic.com/downloads/.

- ClearCore_Microchip_Installer
- ClearCore_Arduino_Wrapper_Installer
- ClearCore_Port_Driver_Install
- ClearPath-MC and -SD Series Motor Setup Program

Motors are controlled using Arduino board, which is represented in ClearCore Controller. However, before using the motors, it is necessary to calibrate them. I did it in the software. Also there is instruction how to set the Arduino connection: https://teknic.com/files/downloads/manual_install_instructions_arduino.pdf

![20221129_102230](https://user-images.githubusercontent.com/116614806/206883302-3178ab78-eb8b-4c29-b412-e0049efcbb11.jpg)


https://user-images.githubusercontent.com/116614806/206883289-c2d09c95-6587-4183-91dc-0f3674cbb988.mp4








