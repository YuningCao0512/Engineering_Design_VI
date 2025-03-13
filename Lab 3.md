# Lab 3: Python
## Instruction
For this lab, the main purpose is to use the information provided in [lesson 3](https://github.com/kevinwlu/iot/tree/master/lesson3) to print certain outputs. Before achieving this goal, we need to download python packages first. 
- `dcal`
- `astral`
- `geopy`
---

To complete the download, I used the commands `pip3 install jdcal`, `pip3 install astral` and `pip3 install geopy`.
I created my own enviroment to prevent errors from happening (specifically when terminal shows externally managed error).

![download](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/download.png)
## Executing commands 
### 1. cd ~/iot
This command change direction of the terminal to iot, which is the overall document.

![~/iot](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/iot.png)

---
### 2. cd *3
This command guide us to lesson 3 directly, instead of using all the extra steps.

![cd *3](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/cd%20*3.png)

---
### 3. python3 julian.py
This command prints the Calender date, the Julian date and the modified Julian date in terminal.

![julian](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/python3%20julian.png)

---
### 4. python3 date_example.py
This command gives us the current date in two different types of ways. Meanwhile, information like day of the week, month, year, days after the first day of classes and days before the last day of classes. This can be used as a powerful tool for time tracking. 

![date_example](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/python3%20date_example.png)

---
### 5. python3 datetime_example.py
This command prints different examples to show date time 

![datetime_example](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/datetime_example.png)

---
### 6. python3 time_example.py
This command prints the time every 10 seconds. We are able to use command `Control C` to interupt (stop the command from running)

![time example](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/time%20example.png)

---
### 7. python3 sun.py "New York"
This prints the daily time information for New York. It gives basic information like the time for timezone, latitude, longtitude, as well as time for different stages of the day. 

![New York](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/New%20York.png)

---
### 8. python3 moon.py
This command prints different moon phases in the terminal on different dates.

![moon](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/moon.png)

---
### 9. python3 coordinates.py "Samuel C. Williams Library"
This command prints the exact address of the Samuel C. Williams Library on Earth, as well as including the street address and the county.

![library](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/library.png)

---
### 10. python3 address.py "40.74480675, -74.02532861159351"
This command uses the information from the library to determine the address of the location it provided. 

![address](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/address.png)

---
### 11. python3 cpu.py
This command presents the number of physical cores, the number of logical CPUs and the utilization per second as a percentage for each CPU. The information is presented in matrix form. 

![cpu](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/cpu.png)

---
### 12. python3 battery.py
This command presents the basic battery information about the local computer (my computer).

![battery](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/battery.png)

---
### 13. python3 documentstats.py document.txt
This command counts the number of words in the document, as well as giving counts of the appearance of certain selected words. 

![wordcount](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab3_pictures/wordcount.png)

---
## Conclusion
This lab demonstrates how we are able to use terminal to perform certain tasks based on the library downloaded. The terminal is able to achieve a lot of tasks we are not able to achieve by hand. This lab demonstartes the powerful utilization of terminal and python code libraries. 
