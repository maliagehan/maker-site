---
layout: tutorials
title: RasPi Imager
subtitle: RasPi Imager
---
<h2 align="center">Meter-Made: Raspberry Pi Imaging Station Tutorial</h2>

<h3 align="center">by Tom Liu (STARS Summer Intern) and Dmitri Nusinow</h3>
<br>
<b>Setting up Raspberry Pi:</b>  

<p>1. Open the Raspberry Pi Complete Starter Kit and take out its contents.
</p>
<p>2. Insert the Noobs Preloaded SD Card 8Gb, Ethernet cable, USB mouse, USB keyboard and a HDMI Cable into the right ports.
</p>
<p>3. Connect the HDMI Cable into the monitor (you may need a HDMI to VGA/DVI adapter depending on the monitor.)
</p>
<p>4. Internet connection is not required, however, if you want internet, plug in an Ethernet cable to the Raspberry Pi.
</p>
<p>5. Plug in the Micro USB Power Supply, Pi will start automatically.
</p>
<p>6. If this is the first time you are using the Pi, then load Raspbian OS.
</p>
<p>7. The after it is finished, click OK. The Pi will reboot (if not, reboot the Pi (unplug and replug in) and take you to the Raspberry Pi Software Configuration tool (raspi-config).
</p>
<p>8. Setup Options to change: enable camera, change password, set to local timezone.
</p>
<p>9. The default username and password is pi and raspberry.
</p>

<b><font color="orange">Note:</font></b> Do not be alarmed when no writing appears when you are typing in the password, this is just a security feature of Linux. However, to change the password, type in the command:
</p>

  ```python
    sudo raspi-config 
  ```

<a href="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img1.png" target="_blank">
<img src="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img1.png" align="center" width="600"></a><br>

<p>
10. After you have successfully logged in, the command line prompt should read: 
</p>

  ```python
    pi@raspberrypi~$ 
  ```
<br>
<b>Setting the Time and Date on your Raspberry Pi.</b>

<p>  
<b><font color="orange">Note:</font></b> The Rasberry Pi does not have a very accurate clock, so the time needs to be reset and coordinated frequently to avoid drift. To set the date:
</p>
<p>
1. Type the following:
</p>

  ```python
    #sudo date -s Day Of Week Month Day Hours:Minutes:Seconds Timezone Year
    #for example if it is 07/11/2014 at 11:59:30 on Friday in the Central timezone:
    
    sudo date -s Fri Jul 11 11:59:30 CDT 2014
    
  ```

<p>
2. This will update the time. If the Raspberry Pi reboots, check the time and date using the command:
</p>

  ```python
    date
  ```
<br>
<b>Setting up the Raspberry Pi camera</b>

We followed instructions that can be found [here](http://thepihut.com/pages/how-to-install-the-raspberry-pi-camera)

<p>1. Open up your Raspberry Pi Camera module. Be aware that the camera can be damaged by static electricity. Before removing the camera from its grey anti-static bag, make sure you have discharged yourself by touching a grounded object (e.g. a radiator or PC Chassis).
</p>
<p>2. Install the Raspberry Pi Camera module by inserting the cable into the Raspberry Pi. The cable slots into the connector situated between the Ethernet and HDMI ports, with the silver connectors facing the HDMI port.1
</p>
<p>3. Boot up your Raspberry Pi.
</p>
<p>4. To take a photo, enter the command:  
</p>
  ```python
    raspistill -o image.jpg
  ```

<p>5. The picture is now in your home folder, "labeled image.jpg"
</p>

<b><font color="green">Optional:</font></b> If you did not enable the camera option after installing the OS and running raspi-config for the first time.

<p>1. From the prompt, run:

  ```python
    sudo raspi-config
    
    #If the "camera" option is not listed, you will need to run a few commands to update your Raspberry Pi.
    
    sudo apt-get update
    sudo apt-get upgrade

  ```

