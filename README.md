# Installing DSRC simulation tools on Ubuntu

## Downloading tools

## [VEINS](https://veins.car2x.org/download/)
## [OMNeT++](https://omnetpp.org/download/)
## [INET](https://inet.omnetpp.org/)

Before downloading, scroll down in VEINS download to check the compatibility.

# Installing OMNeT++ 
## Installing the prerequisite packets
> $ sudo apt install -f

> $ sudo apt update

> $ sudo apt-get install build-essential gcc g++ bison flex perl python python3 qt5-default libqt5opengl5-dev tcl-dev tk-dev libxml2-dev zlib1g-dev default-jre doxygen graphviz libwebkitgtk-1.0

> $ sudo apt-get install openscenegraph-plugin-osgearth libosgearth-dev

## Adding environment variable

> $ cd omnetpp-6.0.1

> $ . setenv 

> $ gedit ~/.bashrc

### Adding the path: export PATH=$PATH:/home/user/Downloads/omnetpp-5.6.2/bin

> $ sudo -s

> $ ./configure

> $ make

## Running OMNeT++

> $ omnetpp

# Adding INET and Veins into OMNeT++

## INET
### File &rarr; Import &rarr; Existing Projects into Workspace &rarr; Next &rarr; Select root directory &rarr; Browse &rarr; inet4.4 &rarr; Finish
## VEINS
### File &rarr; Import &rarr; Existing Projects into Workspace &rarr; Next &rarr; Select root directory &rarr; Browse &rarr; veins-veins-5.2 &rarr; Finish

![](1.png)
![](2.png)
![](3.png)

# Installing SUMO

> $ sudo add-apt-repository ppa:sumo/stable

> $ sudo apt-get update

> $ sudo apt-get install sumo sumo-tools sumo-doc

# Running an example

Open file veins/examples/veins/omnetpp.ini

Right click &rarr; Run as &rarr; OMNeT++ Simulation / Click Run on the Toolbar.

Open terminal and run:

> $ '/home/mike/Documents/dsrc_cv2x/veins-veins-5.2/sumo-launchd.py' -vv -c '/usr/bin/sumo-gui'

Press F5 or click Run with full animation on the Toolbar to run simulation.
