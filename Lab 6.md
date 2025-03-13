# Lab 6: Node.js and Pystache
For this lab, the main purpose are: 
  1. Install [Node.js](https://nodejs.org/en/download/) and run hello-world.js, hello.js, and http.js
  2. Install Pystache and run say_hello.py that uses the template in say_hello.mustache
This lab is achieved using resources from [repository Lesson 6](https://github.com/kevinwlu/iot/tree/master/lesson6)
---
## Using Node.js to accomplish certain tasks 
### I used the link above to successfully download Node.js. 
I used command `node hello-world.js` to run the hello-world.js file in the terminal. This is the output:
![output](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab6_pictures/hello_world.png)
I used command `node hello.js` to run the hello-world.js file in the terminal. This is the output:
![output](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab6_pictures/hello.png)
I used command `node http.js` to run the hello-world.js file in the terminal. This is the output:
![output](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab6_pictures/http.png)
Each command have different outputs at the websites. Based on the pictures above, hello-world.js printed hello world once. Hello.js had outputs as "response end call done" and "request end event fired" in the terminal after displaying the words. The command http.js printed the amount of output of the website being refreshed. 

---
## Pystache 
I used the command `sudo pip3 install pystache` to download Pystache on my laptop. Then I used the following command to finish the lab assignment: 
  `cat say_hello.mustache`
  `cat say_hello.py`
  `python3 say_hello.py`
However, the downloading was not working at first. Here is the mistake:
![mistake](https://github.com/YuningCao0512/Engineering_Design_VI/tree/main/lab6_pictures)
I tried to use `brew install pipx` command combined with `pip install pystache` to download Pystache in my environment. Here is the successful output:
![work](https://github.com/YuningCao0512/Engineering_Design_VI/blob/main/lab6_pictures/work.png)

---
## Conclusion
In this lab, I learned how to use terminal to run certain commands on my laptop. With certina commands provided, I will be able to display certain outputs. 
