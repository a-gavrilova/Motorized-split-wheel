# Motorized split-wheel

I study Purkinje cells activity in cerebellum of mice undergoing locomotion adaptation task. For this purpose in the Optical Neuroimaging Unit (Prof. Bernd Kuhn, OIST, Japan), we designed a behavioral setup consisting of 2 motorized wheels and head-fixation system. This method can be combined with various methods, allowing to record neuronal activity, such as two-photon calcium imaging, voltage imaging and electrophysiological recordings. 

Here is the hardware used and software developed for such behavioral setup.

## Hardware

### Electronic supplies
1. https://teknic.com/model-info/CPM-SDSK-2310S-EQN/  servo motor
2. https://teknic.com/ipc-5/    power supply
3. https://teknic.com/products/io-motion-controller/clcr-4-13/  ClearCore Controller
4. https://teknic.com/IPC35-CABLE110/   1 cable from power supply to the general power supply
5. https://teknic.com/CPM-CABLE-PWR-MS120/  2 cables from power supply to the motors
6. https://teknic.com/CPM-CABLE-CTRL-MU120/  2 cables from ClearCore Controller to the motors
7. https://teknic.com/CPM-CABLE-USB-120/      2 cables from motor to the PC (for calibrating motors)
8. https://teknic.com/CC-3TERM-PLUG-10PC/     for grounding
9. https://teknic.com/CPM-CABLE-USB-120AB/    cable from ClearCore Controller to the PC
10. https://teknic.com/PWR-IO-24VDC/        24 VDC power supply (analog from Amazon can be also used)

### Materials for the wheel
1. Acrylic mirror
2. Acrylic plastic 600 x 900 x 1 mm  
3. Acrylic plastic 600 x 900 x 0.5 mm
4. 
The CAD files of the prototype are located in the corresponding subfolder of the current repository.

- A6061P-6F-BS-SSN-143-60-12: https://jp.misumi-ec.com/vona2/detail/110310113039/?HissuCode=A6061P-6F-BS-SSN-143-60-12
- A6061P-6F-BS-SSN-155-88-12: https://jp.misumi-ec.com/vona2/detail/110310113039/?HissuCode=A6061P-6F-BS-SSN-155-88-12
- A6061P-6F-BS-SSN-100-88-12: https://jp.misumi-ec.com/vona2/detail/110310113039/?HissuCode=A6061P-6F-BS-SSN-100-88-12
- ACSH-500-300-2: https://jp.misumi-ec.com/vona2/detail/110300535170/?HissuCode=ACSH-500-300-2
- ACA-500-300-4: https://jp.misumi-ec.com/vona2/detail/110302695910/?HissuCode=ACA-500-300-4
- ACA-500-300-3: https://jp.misumi-ec.com/vona2/detail/110302695910/?HissuCode=ACA-500-300-3
- アクリミラー 鏡シルバー色 厚さ2mm幅180mm長さ320mm M001 SS 2 : https://www.monotaro.com/p/0228/7477/
- ポリカーボネート樹脂板 透明色 厚さ1mm幅600mm長さ900mm 1枚 KPAC901-1: https://www.monotaro.com/p/8626/9523/?t.q=%83%7C%83%8A%83J%81%5B%83%7B%83l%81%5B%83g
- ポリカーボネート樹脂板 透明色 厚さ0.5mm幅600mm長さ900mm 1枚 KPAC9005-1: https://www.monotaro.com/p/8626/9575/?t.q=%83%7C%83%8A%83J%81%5B%83%7B%83l%81%5B%83g
- A6061-BP-30-100: https://jp.misumi-ec.com/vona2/detail/110310150299/?HissuCode=A6061-BP-30-100
- JTDZS-SUD-A200-B200-T1: htps://jp.misumiec.com/vona2/detail/110302699930/KWSearch=%e3%82%b9%e3%83%86%e3%83%b3%e3%83%ac%e3%82%b9%e6%9d%bf%201.0mm&searchFlow=results2products

To avoid paws slipping form the wheel, the round holes are made in the wheel surface. There is also a 2-cm lip on the edge of the wheel for the mouse's safety and balance control. 

### Head-fixation

For the fixation of a mouse's head, we used Thorlabs connectors and 1/2" posts. 

## Software

All the programs used for calibration and running motors can be downloaded from the main ClearCore website: https://teknic.com/downloads/.

- ClearCore_Microchip_Installer
- ClearCore_Arduino_Wrapper_Installer
- ClearCore_Port_Driver_Install
- ClearPath-MC and -SD Series Motor Setup Program

Before using the motors, it is necessary to calibrate them using Motor Setup Prgram (MSP). After calibration, motor are ready to use. 
Here is instruction how to set the Arduino connection: https://teknic.com/files/downloads/manual_install_instructions_arduino.pdf
The code used for the motor speed control can be found in the subfolder of the current repository.

## Split-wheel setup all together
The wheel is made with the 19 cm diameter, to fit under our microscope stage. 





## Contact us
Feel free to ask questions via opening an issue here or directly to the email: aleksandra.gavrilova@oist.jp

## Contributors
The project is led by myself with advices from Kuhn Unit current members. Design and making the pieces for the treadmill was done with the help of Machine Engineering Section at OIST. 
