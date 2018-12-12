# CENG-317

# BME280 TEMPERATURE APP
Implementing the BME280 temperature sensor with a Pi 3


## Table of Contents
1. [Build Instructions](#build-instructions)
2. [System Diagram](#Introduction-using-a-system-diagram)
3. [Material/Budget](#Materials-Budget)
4. [Time Commitment](#Time-Commitment)
5. [Mechanical Assembly](#Mechanical-Assembly)
6. [PCB](#PCB-Soldering)
7. [Power Up](#Power-Up)
8. [Unit Testing](#Unit-Testing)
9. [Production](#Production-Testing)


![Image text](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/enclosure.jpg)

## Introduction 
You have to make a project for your science class in  school or just looking for a hobby to do during the weekend then the BME 280 sensor is for you. 

The BME280 is a humidity, pressure and temperature sensor that has fast response time and high overall accuracy. and in this project we would be implementing it, using a raspberry pi. together you have your own personal "weather device". 

## Build Instructions
Building a bme 280 below as follows:

## Introduction-using-a-system-diagram
![psuedo-image](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/PSUEDO%20CODE%20UML%20DIAGRAM.JPG)


## Materials-Budget

## Items Required: 
1. Raspberry pi
2. BME 280 Sensor Adafruit or Sparkfun either works fine.
3. Breadboard
4.jumper wires 
5. micro sd card
6. RJ-45 Cable
7. acyclic enclosure (housing for your case)

# Budget
The cost of this project was a dollar short of $180 CAD less than 200 dollars. thats a pretty decent amount for this type of project.
the link to the budget, revealing detailed amount for each item can be found [here](https://github.com/sam9dadet/CENG-317/blob/master/BME280%20image%20files%20and%20link/Budget%20for%20BME280%20Sensor.xlsx) 


## Time Commitment
this project personally took me 15 week to do in a span of 3 hours each day and that's because it was technically an inclass project but doing this outside of school or as a hobby like i stated above, it should take you an average of a weekend pending if you havee all your parts and source code before starting.

# Mechanical Assembly
![raspberry pi](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/raspberry%20pi.jpg).

This is the image of my raspberry pi , so for these next steps i'm going to detail it in very easy steps below so anyone can folow them.

1.) get your raspberry pi

2.) the sd card you bought, you would want to download the latest raspbian O.S on it. which can me found at [raspbian-OS] (https://www.raspberrypi.org/downloads/raspbian/) installation guide is available on the webite and it take minutes to set up . what you're looking for is the "Raspbian Stretch with desktop and recommended software".

3.) insert the micro sd card into the raspberry and power up (you would need a keyboard, mouse and a HDMI cord for display  for the next few steps) 
 
 i) you would plug in the mouse and keyboard to the USB outlets of the raspberry pi and the HDMI from the raspberry pi to a TV or monitor screen to give you a graphic environment.
  
  ii.) altenatively you can configure the raspberry pi to use Ethernet for remote desktop connection. eradicating the use of a mouse, keyboard and hdmi cord every single time you want to use the raspberry pi. this is a [link](http://www.circuitbasics.com/access-raspberry-pi-desktop-remote-connection/) to setup raspberry with remote desktop. 
  
  iii)when you're done configuring your pi your screen output should look like this. 
  ![raspberry OS display](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/pi%20IDE.JPG)
  
  
  4.) Now you would want to read the  12c address on your BME 280 to make sure that it is not broken, first step is :
  
  i) Soldering of your bme 280 header pins . now if you've never soldered in your entire life or have no clue please watch this video below on soldering . the [video](insert url here) uses a different sensor but it should look similar.
  
  ii) Breadboard Connection- now this step shouldn't be hard but it should be done carefully and thoroughly , because one wrong wire in the wrong output and you could fry your sensor . So to avoid that i would be including the image of both the raspberry pin configuration and that of the bme. 
  ![raspberry-pin-out](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/pi3_gpio.jpg)
  
  and below you can find the pin out for raspberry pi pending on if you got the adafruit or sparkfun
  ![bme-280-pin-out](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/bme280%20pin%20config.JPG)
  
  iii) i2c configuration - 
  this is the [link](https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup/configuring-i2c) to setup your i2c address on your raspberry
  and the code to run on the terminal is as follows with no quotation: "sudo i2cdetect -y 1"
  
  and you should have an output like this 
  ![i2cc](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/i2c.jpg)
  
  
  
  
  5) designing of your PCB on the fritizing tool . now you're wondering "whats fritzing or what kind of tool is that". well fritizing is a tool used to design PCB and quite a number of electroics too. 
  follow this [link](http://fritzing.org/download/) to download the fritzing tool (very easy to install and set up) 
  
  i)  make sure you have all your parts in the friting library or you would have to download it within the library.
  
  when you're done setting up fritzing. your connection should look like this.
  
  this is the schematic for your conncetion.
  ![Schematic](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/schematic%20fzz.jpg)
  
  
  This is how it should look like your connection from breadboard to raspberry pi.
  ![Breadboard](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/breadboard%20fzz.jpg)
  
  
  
  this is the pcb design of your connection. this is how it is gonna look like when you print it out.
  ![pcb](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/PCB_pcb.jpg)
  
  
  
  
  
  ii) get your PCB printed and it should look similar to this. 
  ![pcb-sam](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/pcb%20image%20.jpg)
  
  ## PCB-Soldering
   Again just like above you would have to do some soldering here and if you're not familair with soldering ill post a link to a  soldering video [here](https://www.youtube.com/watch?v=oqV2xU1fee8) please review this video.
   
   and here is the final output of how your sensor should look like on the pcb ( you would also need GPIO/HEADERS to avoid soldering directly onto your pi).
   ![pcbb](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/pcb%20soldered.jpg)
  
  
  ## Power Up
  After connecting your soldered senor to the pi you would want to run a python code to read the output of your sensor .
  
  you can run this [python script](https://learn.adafruit.com/adafruit-bme280-humidity-barometric-pressure-temperature-sensor-breakout/python-circuitpython-test) to test the output .
  
  your output should look like this. 
  ![powerup](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/bmetestscreenshot.png)





 ## Unit Testing 
 
 
 
 
 ## Production-Testing
  
  
  
  
  
  ## References
  
  Adafruit BME280 Humidity Barometric Pressure Temperature Sensor Breakout. (n.d.). Retrieved from [link] (https://learn.adafruit.com/adafruit-bme280-humidity-barometric-pressure-temperature-sensor-breakout/python-circuitpython-test)
  
  How to Access the Raspberry Pi Desktop with a Remote Desktop Connection. (2018, June 21). Retrieved from  [link] (http://www.circuitbasics.com/access-raspberry-pi-desktop-remote-connection/)
  
  
  T., I. (n.d.). Retrieved from [link](https://xdevs.com/guide/thp_rpi/)
  
  
  
   
  
  

