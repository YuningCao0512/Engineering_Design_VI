# Lab 10: Blockchain
The purpose of this lab is to use terminal to achieve following purposes: 
- Run `hash_value.py` twice and compare results
- Run `snakecoin.py`
- Run `snakecoin-server-full-code.py` on Terminal 1 and mine a new block on Terminal 2
- Clone Python blockchain app and uncomment the last line of `node_server.py`
- Run `node_server.py` on Terminal 1 and `run_app.py` on Terminal 2

The information and instructions come from [this repository](https://github.com/kevinwlu/iot/tree/master/lesson10). 

---
## 1. hash_value.py
The main purpose of this part of the lab is to run [hash_value.py](https://github.com/kevinwlu/iot/blob/master/lesson10/hash_value.py) twice and compare results. I will use the following commands to achieve this task.
- `cd ~/iot/lesson10`
- `cat hash_value.py`
- `python3 hash_value.py` (This is the library running the first time)
- `python3 hash_value.py` (This is the library running the second time)

Based on the information provided, here is the corresponding output:

![hash_value](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/hash_value.png)

This library prints the information of the hash for 1, 1.0, 3.14, Python, a tuple of vowels and an object of person. After running the library twice, the hash for 1, 1.0 and 3.14 did not have any changes. However, the value for the rest three had significant changes. 

---
## 2. snakecoin.py
The main purpose of this part of the lab is to run [snakecoin.py](https://github.com/kevinwlu/iot/blob/master/lesson10/snakecoin.py) in terminal. The basic commands are:
- `cd ~/iot/lesson10`
- `cat snakecoin.py`
- `python3 snakecoin.py`

Here's the output of the commands in terminal:

![snakecoin1](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/snakecoin1.png)
![snakecoin2](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/snakecoin2.png)

20 blocks are added to the blockchain and the hash information is provided. 

---
## 3. snakecoin-server-full-code.py
The main purpose of this part of the lab is to run [snakecoin-server-full-code.py](https://github.com/kevinwlu/iot/blob/master/lesson10/snakecoin-server-full-code.py) on Terminal 1 and mine a new block on Terminal 2. 

To run the library, the commands I used are:
- `cat snakecoin-server-full-code.py`
- `python3 snakecoin-server-full-code.py`
- `cd`

Here's the output of the commands:

![snakecoin-server-full-code](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/snakecoin-server-full-code.png)

To mine a new block on Terminal 2, I used the following the commands:
- `curl "localhost:5000/txion" \`
     `-H "Content-Type: application/json" \`
     `-d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'`
- `curl localhost:5000/mine`

In case of ImportError: cannot import name 'soft_unicode' from 'markupsafe', I used the following commands to prepare extra libraries:
- `sudo pip3 install markupsafe==2.0.1`
- `python3 snakecoin-server-full-code.py`

After running both terminals at the same time, I was able to get an output from the terminal, and the output `SnakeCoin Server` was printed on the website. 

![final output](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/snakecoin-server-full-code_finaloutput.png)

---
## 4. node_server.py
The main purpose of this part of the lab is to clone Python blockchain app and uncomment the last line of `node_server.py`. I will use the following commands:
- `git clone https://github.com/satwikkansal/python_blockchain_app.git`
- `cd ~/python_blockchain_app`
- `nano node_server.py`

I was able to modify the library based on the commands provided. Here's the library after being modified:
![modified](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/node_server_modified.png)

---
## 5. node_server.py and run_app.py
The main purpose of this part of the lab is to run `node_server.py` on Terminal 1 and `run_app.py` on Terminal 2. The commands will be:

- `python3 node_server.py` (terminal 1)
- `cd ~/python_blockchain_app` (terminal 2)
- `python3 run_app.py` (terminal 2)

Here's the output of the conbined terminals:

![5](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab10_pictures/5.png)

## Conclusion
This lab uses command in terminals to help redirect the addresses of the websites. The utilization of block chain can be very useful in different ways and fields. 


