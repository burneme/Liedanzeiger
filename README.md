# St. Martin, Liedanzeiger #

Many of the old-fashion displays in churches face problems when searching for spare parts i.e. bulbs and resting switches. I found a very nifty way to do a replacement using "https://github.com/mrazekv/church-numbers",
where a system with HDMI-Monitor and raspberry-Pi zero 2W is shown as a solution.
The invest is very small, currently used 24"-Monitors (in most cases this size is more than enough) are cheap, a "raspberry pi zero 2W" is less than 20€ and the input can be done with any browser on tablet/mobile-phone/notebook.

The minium you need is:

  **Full HD-Monitor** with HDMI input,
  
  **raspberry pi zero W** or **raspberry pi zero W** including **µSD-card 8GB minimum**,
  
  **tablet / mobile phone / PC / notebook**,
  
  **HDMI cable** and a **USB-power supply**.
  
The code for the µSD card "ready to start" you can get in the meanwhile from this site. It was my first intention to provide the final image to avoid the nasty work for people who are not trained to linux. You might use the link from mrazekv including all the steps to get a rocksolid installation (read-only file system). Github doesn't allow large files, even my available cloud cannot handle files beyond 1GB, so google helped me. See the link below the pictures.
If there is the requirement for one or more additional displays (side aisles), a Sat(telite) version is possible. In cases, when the second monitor is not far away, a HDMI-splitter can be used to connect two monitors to one single raspberry. In my home town this unit with satellite is now running for a year with good experience.

Finally it looks like this:

![Front](https://github.com/burneme/Liedanzeiger/blob/main/Front.JPG)
![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Ipad3.JPG)
ipad3 with a printed frame to hook it on the organists console
![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Back.JPG)
Neat arrangement of connection cables.

The specific python/html-code, which is more or less a translation from czech language is attached as sw.zip, expand it and store it below /home/admin.   You should see it as "home/admin/cisla/..".

Finally I found a download space for the image at google:

[Image for Single Display](https://drive.google.com/file/d/1Por2zFch3SOl4XRDp1puK9v_BIOZQSrb/view?usp=drive_link/ "An raspberry pi zero image for one display") 

When the download is complete, you need to flash a sd-card using "belena etcher", download this if you don't have and work as it is stated.

![BalenaFlasher](https://github.com/burneme/Liedanzeiger/blob/main/balena.png)

The password for the wifi-net is "Epiphany", you should change that as soon as you can, change this asap, otherwise you will end in a musical request concert :).

This pw is stored in /etc/...
Have fun and distribute it.

