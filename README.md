# St. Martin, Liedanzeiger #

Many of the old-fashion displays in churches face problems when searching for spare parts i.e. bulbs and resting switches. I found a very nifty way to do a replacement using "https://github.com/mrazekv/church-numbers",
where a system with HDMI-Monitor and raspberry-Pi zero 2W is shown as a solution.
The invest is very small, currently used 24"-Monitors (in most cases this size is more than enough) are cheap, a "raspberry pi zero 2W" is less than 20€ and the input can be done with any browser on tablet/mobile-phone/notebook.

The minium you need is:

  **Full HD-Monitor** with HDMI input,
  
  **raspberry pi zero W** or **raspberry pi zero W** including **µSD-card 8GB minimum**,
  
  **tablet / mobile phone / PC / notebook**,
  
  **HDMI cable** and a **USB-power supply**.

This material can be conveniently sourced in Europe from berrybase.de or similar suppliers. Even optional material, shown in a separate directory, is available there.
  
The code for the µSD card "ready to start" you can get in the meanwhile from this site. It was my first intention to provide the final image to avoid the nasty work for people who are not trained to linux. You might use the link from mrazekv including all the steps to get a rocksolid installation (read-only file system). Github doesn't allow large files, even my available cloud cannot handle files beyond 1GB, so google helped me. See the link below the pictures.
If there is the requirement for one or more additional displays (side aisles), a Sat(telite) version is possible. In cases, when the second monitor is not far away, a HDMI-splitter can be used to connect two monitors to one single raspberry. In my home town this unit with satellite is now running for a year with good experience.

Finally it looks like this:

![Front](https://github.com/burneme/Liedanzeiger/blob/main/Front.JPG)
![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Ipad3.JPG)

ipad3 with a printed frame to hook it on the organists console

![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Back.JPG)

Neat arrangement of connection cables.

## Creating a working SD-card ##

Finally I found a download space for the image at google:

[Click here to download image for Single Display](https://drive.google.com/file/d/1Por2zFch3SOl4XRDp1puK9v_BIOZQSrb/view?usp=drive_link/ "An raspberry pi zero image for one display") 

When the download is complete, you need to flash a sd-card using "belena etcher", download this if you don't have it installed already and start it.

![BalenaFlasher](https://github.com/burneme/Liedanzeiger/blob/main/balena.png)

When you have  the finished card, insert this into the slot of raspberry pi zero and apply power, the already operating monitor should show for a second a colored pattern followed by a spinner. When the spinner disapears, you should be able to connect to a Wifi-net called "StMartin", you will be asked for the password "Epiphany". The system gives your device an IP-adress in the net 192.168.4.0.
The next step is to call the index.html, insert into your favourite browser "192.168.4.1" as the URL and press enter, the entry mask should appear.
You can enter a three-digit main number and a substring followed by "Scribe!" (Write!), "Detege!" clears the display.

>  ## Password change ##
>
>  The password for the wifi-net inside the given image is "Epiphany", you should change that as soon as you can. Change this asap, otherwise you will end in a musical request concert :).
>
>  This pw is stored in /etc/hostapd/hostapd. To change it, you need to connect to the system.
>
>  For linux, beeing in the same network, use
>
>  **ssh admin@192.168.4.1**
> (for windows install "putty" before)
>
>  you answer with "admin" and get the message "connected to..."
>
> Change to the subdirectory
> 
>  **admin@raspberrypi(ro):~$** *cd /etc/hostapd*
>
>  Since you are in a read-only mode, you need to switch to read-write-mode:
>
>  **admin@raspberrypi(ro):/etc/hostapd$** *rw*
>
>  Then call the editor (i use joe, behaves like old wordstar) 
>
>  **admin@raspberrypi(rw):/etc/hostapd$** *sudo joe hostapd.conf* 
>
>  Change the pw accordingly to your personal requests.
>
>  To store it, type 
>  **cntl-k**
>  and 
>  **x**,
>
>  then set back to read-only:
>
>  **admin@raspberrypi(rw):/etc/hostapd$** *ro*
>
>  reboot (replug) and use your new wifi pw.

The small changes for a second system, acting as a slave, will follow on request.
Have fun and distribute it.

P.S.:
**Issues during operation**
After nearly one year we faced a problem with difficult reception, the system could not recognize commands and did not react. The cause was a noisy USB power suppyly. Changing this to and old one from the surplus, it worked fine again. Since the noisy one was brandnew (1year) from China, it might be a reason why your setup is not working as excepted. It might be that the raspberry is not very resistant to noisy supply. If you can, use a supply recommended for raspberry Pi. Attached see the output voltage of the faulty supply (AC-Coupling, 20mV/div):

![Faulty supply voltage](https://github.com/burneme/Liedanzeiger/blob/main/NOISY.PNG)
