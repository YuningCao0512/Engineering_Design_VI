# Lab 7: ThingSpeak and Google Sheets
There are a couple requirements for this lab. The main tasks including: 
- Sign up and log in MathWorks [ThingSpeak](https://thingspeak.mathworks.com/channels)
- Run [thingspeak_cpu_loop.py](https://github.com/kevinwlu/iot/blob/master/lesson7/thingspeak_cpu_loop.py) or [thinkspeak_feed.py](https://github.com/kevinwlu/iot/blob/master/lesson7/thingspeak_feed.py) in a demo folder
- Install gspread and oauth2client
- Log in the Google Cloud Platform Identity and Access Management, create a project cpudata, enable both Drive API and Sheets API, create and download service account JSON key file
- Start a new Google sheet cpudata, share it with the client email in the JSON file, delete Rows 2 to 1000, and edit the header cells
- Run [cpu_spreadsheet.py](https://github.com/kevinwlu/iot/blob/master/lesson7/cpu_spreadsheet.py) with the JSON key file in a demo folder

The resources come from [this repository](https://github.com/kevinwlu/iot/tree/master/lesson7)

---
## 1. MathWorks ThingSpeak
The main purpose of this session is to introduce MathWorks ThingSpeak. I already had a ThingSpeak account before for MATLAB use, so all I did was logging into my account. The tasks for this part of the lab is to: 

- Create new channel cpu_loop with field1 cpu_pc and field2 mem_avail_mb
- Copy the Write API Key from channels

![channel](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/ThingSpeak_channel.png)

![LICC5CVEXZ0FJ2R1](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/Write_API_key.png)

---
## 2. thingspeak_feed.py
The main purpose of this session of the lab is to run `thingspeak_feed.py` in a demo folder. To do so, I used the command provided: 

- `sudo pip3 install -U psutil`
- `cd ~/demo`
- `cp ~/iot/lesson7/thingspeak_feed.py .`
- `cat thingspeak_feed.py`
- `python3 thingspeak_feed.py`

After using the commands mentioned, I have gotten the following output:

![output](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/output_1.png)

---
## 3. gspread and oauth2client
At this session, the main goal is to download gspread and oauth2client to my laptop. This task can be achieved by using command:

- `sudo pip3 install -U gspread oauth2client`

![installing](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/installing.png)

---
## 4. Google Cloud Platform Identity and Access Management














