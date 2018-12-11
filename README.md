# CENG-317

# BME280 TEMPERATURE APP
Implementing the BME280 temperature sensor with a Pi 3


## Table of Contents
1. [Build Instructions](#build-instructions)
2. [System Diagram](#Introduction-using-a-system-diagram)
3. [Material/Budget](#Bill-of-Materials/Budget)
4. [Time Commitment](#Time-Commitment)
5. [Mechanical Assembly](#Mechanical-Assembly)
6. [PCB](#PCB-Soldering)
7. [Power Up](#Power-Up)
8. [Unit Testing](#Unit-Testing)
9. [Production ](#Production-Testing)


[Image text](https://raw.githubusercontent.com/)

## Introduction 
You have to make a project for your science class in  school or just looking for a hobby to do during the weekend then the BME 280 sensor is for you. 

The BME280 is a humidity, pressure and temperature sensor that has fast response time and high overall accuracy. and in this project we would be implementing it, using a raspberry pi. together you have your own personal "weather device". 

## Build Instructions
Building a bme 280 below as follows:

## System Diagram
[psuedo image](Insert Link here)





# Material Required 

## Items Required: 
a) Raspberry pi
b) BME 280 Sensor Adafruit or Sparkfun either works fine.
c) Breadboard
d)jumper wires 
e) micro sd card
f) RJ-45 Cable
g) acyclic enclosure (housing for your case)

# Budget
The cost of this project was a dollar short of $180 CAD less than 200 dollars. thats a pretty decent amount for this type of project.
the link to the budget, revealing detailed amount for each item can be found [here](insert link to budget here ) 


## Time Commitment
this project personally took me 15 week to do in a span of 3 hours each day and that's because it was technically an inclass project but doing this outside of school or as a hobby like i stated above, it should take you an average of a weekend pending if you havee all your parts and source code before starting.

# Mechanical Assembly
![raspberry pi](https://raw.githubusercontent.com/sam9dadet/CENG-317/master/BME280%20image%20files%20and%20link/raspberry%20pi.jpg)
This is the image of my raspberry pi , so for these next steps i'm going to detail it in very easy steps below so anyone can folow them.

1.) get your raspberry pi

2.) the sd card you bought, you would want to download the latest raspbian O.S on it. which can me found at [raspbian OS] (https://www.raspberrypi.org/downloads/raspbian/) installation guide is all availabel on the webite and it take minutes to set up . what you're looking for is the "Raspbian Stretch with desktop and recommended software".

3.) insert the microsd card into the raspberry and power up (you would need a keyboard, mouse and a HDMI cord for display  for the next few steps) 
 
 i) you would plug in the mouse and keyboard to the USB outlets of the raspberry pi and the HDMI from the raspberry pi to a TV or monitor screen to give you a graphic environment.
  
  ii.) altenatively you can configure the raspberry pin to use Ethernet for remote desktop connection. eradicating the use of a mouse, keyboard and hdmi cord every single time you want to use a raspberry pi. this is a [link](http://www.circuitbasics.com/access-raspberry-pi-desktop-remote-connection/) to setup raspberry with remote desktop. 
  
  iii)when you're done configuring your pi your scrren output should look like this. 
  ![raspberry OS display](link here )
  
  
  4.) Now you would want to read the  12c address on your BME 280 to make sure that it is not broken, first step to doing that is :
  
  i) Soldering of your bme 280 header pins . now if you've never soldered in your entire life or have no clue please watch this video below on soldering . the [video](insert url here) uses a different sensor butit should look similar.
  
  ii) Breadboard Connection- now this step shouldn't be hard but it should be done carefully and thoroughly , because one wrong wire in the wrong output and you could fry your sensor . So to avoid that i would be including the image of both the raspberry pin configuration and that of the bme. 
  ![raspberry pin out]( insert url here )
  
  and below you can find the pin out for raspberry pi pending on if you got the adafruit or sparkfun
  ![bme 289 pin out](insert url here )
  
  iii) i2c configuration - 
  this is the [link](insert url here) to setup your i2c address on your raspberry
  and the code to run on the terminal is as follows with no quotation: "sudo i2cdetect -y 1"
  
  and you should have an output like this 
  ![i2cc](insert url here)
  
  
  
  
  5) designing of your PCB on the fritizing tool . now youre wondering "whats fritzing or what kind of tool is that". well fritizing is a tool used to design PCB and quite a number of electroics too. 
  foll0w this [link](insert URL here) to download the fritzing tool (very easy to install adn set up) 
  
  i)  make sure you have all your parts in the friting library or you would have to download it within the library.
  
  when you're done setting up fritzing. your connection should look like this.
  ![1](insert url here)
  ![2](insert url here)
  ![3](insert url here)
  
  
  
  
  
  ii) get your PCB printed and it should look similar to this. 
  ![pcb-sam](insert url here)
  
  
  
  5.) 
  
  
## Proposal/Scheduling
Follow the link to see how long it took me to make this project. In the real world it should take a weekend to do this project, pending if and when you have all your parts, downloading your OS, made your PCB and your acrylic case. 

