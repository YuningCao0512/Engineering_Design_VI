# Lab 9: YANG
The main purpose of this lab is to install pyang and PlantUML, copy ~/iot/lesson9/intrusiondetection.yang to ~/demo, run pyang to generate intrusiondetection.yin and intrusiondetection.uml and lastly run PlantUML to generate intrusiondetection.png. The instruction can be found [here](https://github.com/kevinwlu/iot/tree/master/lesson9).

## Install pyang and PlantUML
As usual, to make sure the installing can be achieved without interruption, I decided to use my own environment. The command I used to install are: 
- `pip install pyang`
- `pip install PlantUML`
I am able to install them successfully

![download](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab9_pictures/download.png)

---
## Copy website
To copy the address, I used the command `cp` to help me achieve this purpose.
- `cp ~/iot/lesson9/intrusiondetection.yang ~/demo/`

![copy](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab9_pictures/copy.png)

---
## Running commands 
At first, unfortunately, I was not able to run pyang to generate the corresponding files because I did not have the download tools installed in my laptop. By using the command `pip install setuptools`, I was able to use complete the assignment. 
