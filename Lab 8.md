# Lab 8: Data Analysis
This lab, the main purposes are to: 
- Install Python packages
- Save the [Lab 7 Google sheet](https://docs.google.com/spreadsheets/d/1nbYyeGmE9Q35VCDbZDn72-6ZoZWu6IT9RHJPYSlYppg/edit?gid=0#gid=0) in CSV format to `~/demo`
- Copy `~/iot/lesson8/plt_final.py` and `plt_cv2.py` to `~/demo`
- Edit `plt_final.py` and `plt_cv2.py` to read the CSV file with customized plot titles
- Run `plt_final.py` and `plt_cv2.py`

The tasks will be achieved using the information from [here](https://github.com/kevinwlu/iot/tree/master/lesson8)

---
## 1. Python packages 
I will use the command provided from the resource to download the Python packages.
- `sudo pip3 install numpy scipy scikit-learn matplotlib pandas tensorflow keras`

I have to use an older version of python (python3.10) to complete this part of the lab because the newer versions have issues with the packages downloading. 

![download](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab8_pictures/download.png)

---
## 2. Google sheet to CSV format
At this session, I will save the [Lab 7 Google sheet](https://docs.google.com/spreadsheets/d/1nbYyeGmE9Q35VCDbZDn72-6ZoZWu6IT9RHJPYSlYppg/edit?gid=0#gid=0) in CSV format to `~/demo`. To co pomplete this, I download the google sheet as an csv file on my laptop, then I used command:
- `mv /Users/yuningcao/Desktop/cpudata\ -\ Sheet1.csv ~/Demo/` 

![move](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab8_pictures/move%20csv.png)

## 3. Copy libraries to demo
The purpose of this session is to copy `~/iot/lesson8/plt_final.py` and `plt_cv2.py` to `~/demo`. 
- `cd ~/demo`
- `cp ~/iot/lesson8/plt_final.py .`
- `cp ~/iot/lesson8/plt_cv2.py .`

![copy](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab8_pictures/files%20copy.png)

![demo](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab8_pictures/demo.png)

---
## 4. Editting
This session aims to edit `plt_final.py` and `plt_cv2.py` to read the CSV file with customized plot titles





