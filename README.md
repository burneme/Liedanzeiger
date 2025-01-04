# St. Martin, Liedanzeiger #

Many of the old fashioned displays in churches face problems when searching for spare parts i.e. bulbs and resting switches. I found a very nifty way to do a replacement using "https://github.com/mrazekv/church-numbers",
where a system with HDMI-Monitor and raspberry-Pi zero 2W is shown as a solution.
The invest is very small, currently used 24"-Monitors are cheap, a "raspberry pi zero 2W" is less than 20€ and the input can be done with any browser on tablet/mobile-phone/notebook.

The minium you need is:

  **Full HD-Monitor** with HDMI input,
  
  **raspberry pi zero W** or **raspberry pi zero W** including **µSD-card 8GB minimum**,
  
  **tablet / mobile phone / PC / notebook**,
  
  **HDMI cable** and a **USB-power supply**.
  
The code for the µSD cards ready to start you can't get from this site. It was my intentioni to provide the final image, however they are too large to upload. Therefore you might to use the link from mrazekv including all the steps to get a rocksolid installation or I can provived physical µSD for the net cost price, currently below 5€. Github doesn't allow large files, even an available cloud cannot handle files beyond 1GB.
If there is the requirement for one or more additional displays (side aisles) a Sat(telite) version is possible. In cases, when the second monitor is not far away, a HDMI-splitter can be used to connect two monitors to one raspberry. In my home town this unit is now running for a year with good experience.

Finally it looks like this:
![Front](https://github.com/burneme/Liedanzeiger/blob/main/Front.JPG)
![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Ipad3.JPG)


# What you need to do #

Download the image file and use "BalenaEtcher" and flash your µSD-card. Insert the card into the raspberry pi zero, connect HDMI-output to monitor and power on.

![balena](https://github.com/burneme/liedanzeiger/blob/main/Balena.png)

It is necessary for a proper start to have a connected, ready monitor. After boot time of approx. half a minute (rasp pi zero 2W), you should recognize a Wifi-station "StMartin", the password is set to "Epiphany", you can change it later.
