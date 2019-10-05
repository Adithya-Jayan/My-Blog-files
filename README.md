# Deep Space 1: How and what does it do on Space??
Deep Space 1 or DS1 is a satellite launched by National Aeronautics and Space Administration (NASA) in 1998 to serve its purpose as a technology demonstration spacecraft. It was launched to test various upcoming technologies in space, its conditions, outcomes, threats or limitations of the proposed technology etc. in real time in space rather than earthly simulations.
We are interested to learn how DS1 or any satellite in outer space carry out efficient communications to Space stations in Earth. For this, we must first be aware of Deep Space Network (DSN).
## Deep Space Network
Deep Space Network is a network of large antennas positioned in Earth to capture various signals from the spacecrafts, used to provide scientific data, instructions to spacecraft, health of the spacecraft etc. NASA has positioned three antennas on three locations on Earth, namely California, Spain and Australia, each oriented at an angle of 120 degrees with each other and are spread onto three equidistant points on Earth as above so that at any 
Each location has ultra-sensitive receiver systems with huge antennas namely
* High Efficiency Antenna (HEF) for high gain (34m in diameter)
* Two or more Beam Waveguide Antennas (BWG) (34m in dia)

and several other independent antennas for tracking the spacecraft.

![alt text](https://github.com/ashrikant39/My-files/blob/master/images%20(1).jpg)
![alt text](https://github.com/ashrikant39/My-files/blob/master/images.jpg)
![alt text](http://www.qrg.northwestern.edu/projects/vss/docs/media/Communications/Dsn2.GIF)

## Uplink and Downlink
Tracking of the satellite is mainly achieved by uplink and downlink communications by satellites and space stations on Earth. Uplink refers to communication from a space station to the satellite, whereas downlink refers to communication from satellite to station. When both uplink and downlink occur, it is referred to as Two Way communication. Communication is mainly done using RF signals (mainly microwaves, i.e. in GHz range). 

![alt text](https://github.com/ashrikant39/My-files/blob/master/images%20(2).jpg)
## Lag
Lag is another term that decides the efficiency of communication in DSN. It is the time gap between sending of signal by source and receiving it by the receiver. Lag should be taken care, as when a satellite sends signals for help, instant solutions to the problems must be ready, otherwise making it too late for anything more.
So back to our satellite DS1. 
 
DS1 also uses DSN as the network to downlink data. DS1 mainly transmits two kinds of data :
* 	Health of spacecraft: It refers to the status of the spacecraft with its surroundings in terms of temperature, pressure, voltages, images etc. These measurements (which may go around 1000 in number) are collected and transmitted as radio waves. These are radio waves are simple enough to be received by any receiver on Earth. They contain mainly information like All OK, Track urgent, Red Alert etc. 
* Scientific data: The critical tests and measurements, images of various locations of interests, objects of scientific importance etc.  come under this category. These messages are specially encrypted and can be received only by high gain DSN receivers. 
