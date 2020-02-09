# Neurolab Desktop

[![Build Status](https://travis-ci.org/fossasia/neurolab-desktop.svg?branch=master)](https://travis-ci.org/fossasia/neurolab-desktop)
[![Gitter](https://badges.gitter.im/fossasia/neurolab.svg)](https://gitter.im/fossasia/neurolab?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![Mailing List](https://img.shields.io/badge/Mailing%20List-FOSSASIA-blue.svg)](https://groups.google.com/forum/#!forum/pslab-fossasia)
[![Twitter Follow](https://img.shields.io/twitter/follow/pslabio.svg?style=social&label=Follow&maxAge=2592000?style=flat-square)](https://twitter.com/pslabio)

Neurolab Desktop is a software to read EEG data from a serial stream, do basic DSP, and then output interpreted data to OpenGL, audio, files, OSC and serial. The project goes back to the Neurophlex.

The desktop app requires the Neurolab Hardware. The goal of the Neurolab project is to develop an easy to use open hardware measurement headset device for brain waves that can be plugged into an Android smartphone and a software application and enables us to understand our brains better.

Our brains communicate through neurotransmitters and their activity emits electricity. The neuroheadset measures that electricity on the skin of the forehead and the software processes the signal so that it can translated into a visual or auditory representation. The data that can be collected can be analysed to identify mental health, stress, relaxation and even diseases like Alzheimer. 

Current devices in the medical industry are usually not accessible by doctors due to their high pricing. They are also complicated to use. The idea of the device is to integrate it into a headband and focus and focus on signals that can be obtained through the frontal lobe.

A difference to existing projects like OpenBCI is that it will not be necessary to 3D print large headsets. Instead we are focusing on creating a device that collects as much data as possible through the forehead. To achieve this goal we are using high-grade sensors and flexible electronics.

# Neurolab Desktop Libraries and Components

_**Used Libraries**_:<br><br>
**JTransforms**: BSD 2-Clause<br>
**Jogamp**:  BSD 2-Clause<br>
**JSyn**: Apache License V2<br>
**jSSC**: ?<br>
**ini4j**: Apache License V2<br>
**jfreechart**: LGPL<br>
**log4j**: Apache License V2<br>
**JavaOSC**: BSD 3-Clause<br>

# Set up (Ubuntu 19.04)

### Dependencies
1. Java JDK & JRE
2. Maven
3. Java IDE that supports Maven

### Install NetBeans on Ubuntu 19.04
1. **Install Oracle Java JDK 8**
`sudo add-apt-repository ppa:webupd8team/java
sudo apt update
sudo apt install oracle-java8-installer
sudo apt install oracle-java8-set-default`
That completes your installation. You can check you java version by running following command.
`javac -version`

2. **Downloading NetBeans**
`cd /tmp && wget -c http://download.netbeans.org/netbeans/8.2/final/bundles/netbeans-8.2-linux.sh`

3. **Install NetBeans**
`chmod +x netbeans-8.2-linux.sh 
sudo ./netbeans-8.2-linux.sh`
You should then see NetBeans installation wizard started. The default choices should be just fine. You don’t have to customize too much. However, if you know what you’re doing, you can customize all you want.

### Build Neurolab
1. Fork & clone the Neurolab-desktop repo to the local machine.
2. Import Neurolab-desktop as an existing Maven project in Netbeans
  * In Netbeans, File->New Project->Select maven in left Pane -> Select Project with existing POM on right pane and finish.
  * Now you will be asked to open a eclipse project, just open it and that's it.
3. Build the project in Netbeans (F11)
4. Run and explore Neurolab (F6)
