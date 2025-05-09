
# Lab 5

This lab was aimed at demonstrating real time data exchange between IoT devices where one script publishes cpu data and the other recieves it. Before starting this lab I had to install Mosquitto. 

With the following commands, I installed Paho, cloned the IoT repository for this lesson and redirected to it, and established a client.
```
$ sudo pip3 install paho-mqtt
$ git clone https://github.com/eclipse/paho.mqtt.python.git
$ cd ~/iot/lesson5
$ python3 client.py
```
After updating the cloned repository using gitpull, I changed the directory to lesson 5 and ran subcpu.py on one terminal and pubcpu.py on another. subcpu.py acts as a subscriber and waits to recieve CPU usage data. pubcpu.py acts as a publisher and collects CPU usage data and sends it via mqtt. 

## subcpu.py (Terminal 1)
![App Screenshot]()
## pubcpu.py (Terminal 2)
![App Screenshot]()


