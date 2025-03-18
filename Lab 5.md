# Lab 5: Paho-MQTT

In this lab, I will downlaod Paho-MQTT with instruction from [here](https://github.com/kevinwlu/iot/tree/master/lesson5). After, i will change directory to the iot repository and update the repository with git pull. Then, I will change directory to Lesson 5 and run [python3 subcpu.py](https://github.com/kevinwlu/iot/blob/master/lesson5/subcpu.py) on one Terminal and [python3 pubcpu.py](https://github.com/kevinwlu/iot/blob/master/lesson5/pubcpu.py) on another. 

---
## Downloading Paho-MQTT
I have a MacOS, so I used the follwoing command to download Paho-MQTT:
- `brew install mosquitto`
- `brew services start mosquitto`

Later in the terminal, I used command `pip3 install paho-mqtt` to download the MQTT. It is successfully downloaded and started running. 

---
## iot repository 
This is the first task for this lab. This step is to make sure the lab has a foundation to build upon. I used the following command to make sure this step is completed:
- `cd ~/iot`
- `git pull`

These two steps made sure I am able to change directory to the iot repository and update the repository with git pull. 

![iot](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab5_pictures/cd_iot.png)

---
## lesson 5
At this session, I will change direction back to lesson 5 and start running the code libraries provided above. Considering the two libraries need to take place in two different terminals. I complated the steps above for both terminals. 

![cd lesson5](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab5_pictures/cd_lesson5.png)

---
## Running commands 
After the above steps, all the fundamentals are set and the commands are ready to run. I used the following commands: 
- `python3 subcpu.py`
- `python3 pubcpu.py`

This is the output of `python3 subcpu.py`
![python3 subcpu.py](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab5_pictures/subcpu.png)

This is the output of `python3 pubcpu.py`
![python3 pubcpu.py](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab5_pictures/pubcpu.png)

### Conclusion 
Based on the above information, `pubcpu.py` demonstrates the relative data from the CPU of my laptop, while `subcpu.py` reprints the information with respect to the same timeline from `pubcpu.py`. The conclusion can be drawn by putting the terminals together. 

![together](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab5_pictures/together.png)
