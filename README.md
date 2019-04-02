# Fab μ-Scope

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/scope_logo.jpg) 

## Overview

The study estimates that 5 million people die every year because of poor-quality health care in low- and middle-income countries. That's significantly more than the 3.6 million people in those countries who die from not having access to care.[source](https://www.npr.org/sections/goatsandsoda/2018/09/05/644928153/what-kills-5-million-people-a-year-its-not-just-disease)

So we can solve almost all the problem with utilizing technology, As I mentioned earlier based on the report peoples die without getting proper medical attention, and the most of them don’t have access medical equipment to determine the disease , so they don’t know the seriousness of the disease , and eventually it will make big problems . 

Open source hardware has the potential to revolutionise the way we build scientific instruments; with the advent of readily available 3D printers, mechanical designs can now be shared, improved, and replicated faster and more easily than ever before. However, printed parts are typically plastic and often perform poorly compared to traditionally machined mechanisms.
Fab μ-Scope is cheap, open source microscope that can easily build from a Fablab, main goal is to give quality health checkup to poor people and societies to get medical attention when it's needed. 

## Goals

1. Build Fabable Cheapest Open-Source Microscope that can perform the blood test to find out common diseases 
2. Fully Fabable and Cheap cost
3. Automatically detect diseases Using Image Processing 

## Specifications

I met a team from China during the GOSH -Open Hardware Summit 2018, they built an open source microscope as part of there PhD project, paper in [Review of Scientific Instruments](https://aip.scitation.org/doi/10.1063/1.4941068)  . also saw some amazing microscope from the internet, but most of them lack of documentation. 

Instead of building the microscope from scratch, I was planning to try out and implement the best one out there and modify it’s and make them better by utilizing fablab and release a newer version. 

* Listing some available scopes 

### Water Scope

Water Scope mission is to secure clean water to empower the bottom billion of the world's population. They are utilizing the OpenFlexure Microscope design. 

More : [https://www.waterscope.org/about-us/](https://www.waterscope.org/about-us/)

### Internet of Things Microscope

a low-cost IoT microscope based on the Raspberry Pi 3. Using easily changeable glass objectives. This microscope will provides various magnification. (40x, 100x, 400x). The microscope will scan the specimen on the x and y-axis and stitch the images together to create a large and very detailed image that can be reviewed on an internet connected phone, tablet or computer. We will be making the design as low cost as possible so that anyone in the world has access to a very powerful digital microscope.

More : [https://hackaday.io/project/11429-internet-of-things-microscope]( https://hackaday.io/project/11429-internet-of-things-microscope)

### Free and open-source automated 3-D microscope

Open-source technology not only has facilitated the expansion of the greater research community but by lowering costs it has encouraged innovation and customizable design. The field of automated microscopy has continued to be challenge inaccessibility due to the expense and inflexible, noninterchangeable stages

More : [https://www.appropedia.org/Free_and_open-source_automated_3-D_microscope
](https://www.appropedia.org/Free_and_open-source_automated_3-D_microscope
)



These are the open microscopes available today, but we can see that none of them is easy to build and also there no open documentation available to build our own, and some of the projects are dropped by the maintainer. so I contacted the OpenFlexure team and I  was planning to build one based on that, after it’s replication I will solve it’ limitation (known issues) and adding some features or build one from scratch 

## What I've done so far.

### - ...Trying out OpenFelxure Model  

...OpenFlexure is an open 3D printable microscope, including a precise mechanical stage to move the sample and focus the optics. There are many different options for the optics, ranging from a webcam lens to a 100x, 

... More :[https://github.com/rwb27/openflexure_microscope](https://github.com/rwb27/openflexure_microscope)

... I tried to implement its model by contacting its team (I met them in GOSH meetup in China), the problem is they didn't have good documentation, that's actually huge headache when you try to do something open, only available is a git repo 

... - #### 3D printed 
...I 3D Printed all the required part by contacting the team and by utilizing the FabLab Kochi 


