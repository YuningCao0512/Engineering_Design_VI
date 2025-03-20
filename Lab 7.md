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
For this session of the lab, I started by creating an account on Google Cloud and started by creating my first project with the name `cpudata`. Then, I will go to APIs & Services menu and enable APIs & Services, which includes enabling both Drive API and Sheets API. 

![enables](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/enabling.png)

Next, I will go to Credential > Create Credentials > Create service account key > Service account. I named my account rpudata > JSON key type > Create > download rpidata-xxxxxxxxxxxx.json. 

![service](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/service%20.png)

The next step will be preparing for the use of google spreadsheet. I used the following commands in my terminal: 
- `cd demo`
- `cp ~/iot/lesson3/system_info.py .`
- `cp ~/iot/lesson7/rpi_spreadsheet.py .`

---
## 5. Google sheet
At this session of the lab, I started a new Google sheet named cpudata. I will share it with the client email in the JSON file, delete Rows 2 to 1000, and edit the header cells. I successfully shared the google sheet with the client email on the json file and allowed it to have editting access. 

![info](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/json_info.png)

![sheet](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/sheet.png)

---
## 6. cpu_spreadsheet.py
At this session, I will run `cpu_spreadsheet.py` with the JSON key file in a demo folder. However, before running the library, I have to change the address of my json file, as well as the name of the spreadsheet by using the following command:
- `nano cpu_spreadsheet.py`

![edit](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/nano.png)

I will use command `python3 cpu_spreadsheet.py` to get the final output. 

![terminal](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/final_output.png)
![excel](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab7_pictures/excel_output.png)

---
## Conclusion
This lab uses terminal to help with data exporting. This lab also helps with uploading data to ThingSpeak using the Google Cloud Platform to write information to Google Sheets.
















