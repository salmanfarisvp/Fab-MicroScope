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

### Trying out OpenFelxure Model  

OpenFlexure is an open 3D printable microscope, including a precise mechanical stage to move the sample and focus the optics. There are many different options for the optics, ranging from a webcam lens to a 100x, 

More : [https://github.com/rwb27/openflexure_microscope](https://github.com/rwb27/openflexure_microscope)

I tried to implement its model by contacting its team (I met them in GOSH meetup in China), the problem is they didn't have good documentation, that's actually huge headache when you try to do something open, only available is a git repo 

#### 3D printed 
I 3D Printed all the required part by contacting the team and by utilizing the FabLab Kochi 

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/3d_print.jpg) 


#### Electronics 

After 3D Printing the Required Parts I start work with electronics parts, including its camera and lens module. 
The OpenFelxure is utilising the Pi Cam v2.0 by re-adjusting its stock lens, I tried to do that but that’s ended up broken Pi cam, the problem was I used Pi cam v.1.0 , and it’s not compatible to remove the lens , 

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/pi_cam_one.jpg) 


### ToDo

- [x] Complete the Electronics Parts : Try to use Pi cam v2.0 instead of v1.0,  also need to try out with different lenses 
- [x] Implement Computer Vision : To automate the testing we can use computer vision based on the available data.
- [x] Design Compatible Model : The current OpenFlexure Design is not that much compatible and Sophisticated, it working based on the model bend and material. So I will design a compatible,  easy maintainable design in parallel with the of the openflexure .


### Using the Pi Cam 2.0 

With the help of [Lens Adjustment Spanner](https://www.thingiverse.com/thing:1574661) from Thingiverse ,first I removed the Pi cam 2.0 lens 

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/lens_remover001.jpg)

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/pi_cam_two.jpg)

After that , I attached the Camera lens to 3D printed Optics tube in reverse order .

![Image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/reverse001.jpg)

and attached the camera sensor in the other end, this will help to increase the focal length

![image](https://raw.githubusercontent.com/salmanfarisvp/Fab-MicroScope/master/res/img/reverse002.jpg)






