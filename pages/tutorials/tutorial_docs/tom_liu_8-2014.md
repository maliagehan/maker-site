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
    
    #If the "camera" option is not listed, you will need to update your Raspberry Pi:
    
    sudo apt-get update
    sudo apt-get upgrade

  ```
<p>2. From the prompt, run: 
</p>

  ```python
    sudo raspi-config
    
    #you should now see the "camera" option.
  ```
  
<p>3. Navigate to the camera option, and enable it. Select Finish and reboot your Raspberry Pi.
</p>

<b><font color="green">Optional:</font></b> Changing focus of the camera  

<p>See video from George Wang:
</p>
<iframe width="560" height="315" src="//www.youtube.com/embed/u6VhRVH3Z6Y?rel=0" frameborder="0" allowfullscreen></iframe>
<br>
<p>1. The Raspberry Pi camera's focus is initially set to infinite, if you want a different focus it takes precision and special care.
</p>
<p>2. To change the focus, use a sharp object and carefully remove the glue around the lens.
</p>
<p>3. Every few incisions with the sharp edge carefully turn the lens counter clockwise with some tweezers to check if it will turn.
</p>
<p>4. When it does turn, use the following command to check the focal length:
</p>

  ```python
    raspistill -o image.jpg
  ```
<p><b><font color="orange">Note:</font></b> It is suggested to use a ruler and place the camera at one end of the ruler. Place an object at the desired distance (we use a business card to look for fine detail) and adjust the focus until sharp.
</p>

<b><font color="green">Optional:</font></b> Cutoff filters

<p>1. We use a 730 nm cutoff filter (Lee #87) to block visible light when combining the NoIR camera with an 880 nm LED array to image plants under diurnal cycles. The cutoff filter helps prevent changes in contrast during imaging, making image processing easier.
</p>
<p><b><font color="orange">Note:</font></b> If you are using a camera holder See [here](http://www.thingiverse.com/thing:256960) for a Raspberry Pi case and Camera holder with ball joint, we just tape the filter over the hole for the camera.

<a href="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img2.png" target="_blank">
<img src="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img2.png" align="center" width="400"></a><br>
Figure 1. Raspberry Pi with 730nm cutoff filter over lens. 


<b><font color="green">Optional:</font></b> 3D Print a computer and camera case

Again, See [here](http://www.thingiverse.com/thing:256960) for a Raspberry Pi case and Camera holder with ball joint

<b><font color="green">Optional:</font></b> Disabling LED light in camera

<p>1. If you are imaging plants, then the red light on the camera could cause unwanted responses. To turn off the LED, add the command to the <b>config.txt file</b>.:
</p>

  ```python
    disable_camera_led=1
  ```
  
<p><b><font color="orange">Note:</font></b> To edit the config.txt file you can use Nano:

  ```python
    sudo nano /boot/config.txt
  ```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1. Use the arrow keys to scroll to the end of the file and add to the last line:

  ```python
    disable_camera_led=1
  ```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2. Press CTRL-x to quit. If prompted press Y followed by Return or Enter.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3. After you reboot the camera the red LED will be disabled. Reboot with the following:

  ```python
    sudo reboot
  ```
<p><b><font color="orange">Note:</font></b> There is not a way to disable the LEDs on the circuit board of the Raspberry Pi itself, however, puffy black fabric paint is opaque and can be used to block light from the board.

<a href="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img3.png" target="_blank">
<img src="{{site.baseurl}}/images/tutorial_imgs/tom_liu_8-21-14/img3.png" align="center" width="400"></a><br>
Figure 2. LEDs covered with puffy black fabric paint.

<b>Time lapse imaging:</b>

There are many methods to setting up timelapse imaging on the Raspberry Pi, and the one that we use is to set up a crontab job. This is essentially a script that will run in the background, and take a picture at a prescribed minute/hour/day/month/and day of week.
To edit crontab:

  ```python
    sudo reboot
  ```

