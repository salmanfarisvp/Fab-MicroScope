# Fab μ-Scope

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/scope_logo.jpg) 

## Overview

The study estimates that 5 million people die every year because of poor-quality health care in low- and middle-income countries. That's significantly more than the 3.6 million people in those countries who die from not having access to care.  [source](https://www.npr.org/sections/goatsandsoda/2018/09/05/644928153/what-kills-5-million-people-a-year-its-not-just-disease)

So we can solve almost all the problem with utilizing technology, As I mentioned earlier based on the report peoples die without getting proper medical attention, and the most of them don’t have access medical equipment to determine the disease , so they don’t know the seriousness of the disease , and eventually it will make big problems . 

Open source hardware has the potential to revolutionise the way we build scientific instruments; with the advent of readily available 3D printers, mechanical designs can now be shared, improved, and replicated faster and more easily than ever before. However, printed parts are typically plastic and often perform poorly compared to traditionally machined mechanisms.
Fab μ-Scope is cheap, open source microscope that can easily build from a Fablab, main goal is to give quality health checkup to poor people and societies to get medical attention when it's needed. 

## Goals

1. Build Fabable Cheapest Open-Source Microscope that can perform the blood test to find out common diseases 
2. Fully Fabable and Cheap cost
3. Automatically detect diseases Using Image Processing 

## Required Matrials 

#### Hardware 

1. Raspberry Pi 2/3/4
2. Pi cam v2.0/later
3. OpenFelxure Scope Base
4. M3 Screws and Nuts

#### Software 

1. Raspbian OS 
2. SD card 8GB+
3. OpenCV


## Building Instructions 

This Instructions  Go through very minimalist way to build the <b>Fab-scope</b> . 

### Step 1 : 3D Print the Microscope Base 

I met a team from China during the GOSH -Open Hardware Summit 2018, they built an open source microscope as part of there PhD project, paper in [Review of Scientific Instruments](https://aip.scitation.org/doi/10.1063/1.4941068) . also saw some amazing microscope from the internet, but most of them lack of documentation.

Instead of building the microscope from scratch, I was planning to try out and implement the best one out there and modify it’s and make them better by utilizing fablab and release a newer version.

For the base I choosed [OpenFelxure Model](https://github.com/rwb27/openflexure_microscope) , (The OpenFlexure Microscope is a 3D printable microscope, including a precise mechanical stage to move the sample and focus the optics. There are many different options for the optics, ranging from a webcam lens to a 100x, oil immersion objective.) 

#### 1.1 Download the Design files and 3D Print without Support

1. Main Body.stl
2. Optics.stl
3. illumination.sl

> Note : These files are licenced under [CERN](https://github.com/salmanfarisvp/Fab-MicroScope/blob/master/Licence) by OpenFlexure team .

#### 1.2 Assembling the part 

![Assembled](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/3d_print.jpg)

I 3D Printed all the required part by support of the OpenFexlure team and utilizing the FabLab Kochi , where I worked . 

### Setup 2 : Modify Raspberry Pi Cam

we are getting the zoom by increasing the focal length between the pi cam and stock lens, for that first, we need to remove the lens form the sensor and add 3D printed optics part in between the lens and sensor. 

> try to use Raspberry Pi Cam V2.0 , other version is little bit difficult to remove the lens and it break the cam , like I did in past

#### 2.1 Remove Pi Cam lens 

With the help of (Lens Adjustment Spanner)[https://www.thingiverse.com/thing:1574661] from Thingiverse ,first I removed the Pi cam 2.0 lens

![Lens remove](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/lens_remover001.jpg)

Removed the lens , make sure that keep the bare sensor from dust . 

![bare lens](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/pi_cam_two.jpg)

#### 2.2 Installing in to Optics Model

After removing the lens from the sensor we need install it on the 3D printed optics part . 

![Install lens](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/reverse001.jpg)

next, attach the camera sensor in the other end, this will help to increase the focal length and we can obtain microimaging 

![install sensor](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/reverse002.jpg)


### Setup Illumination 

Light is very important when it comes to microscopic images, we are using 5mm LED to give the illumination for our Scope. Simply insert the 5mm LED on the 3D printed Illumination Part .

![Illumination Install](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/ledlight_source-small.jpg)


### Assembling Together 














