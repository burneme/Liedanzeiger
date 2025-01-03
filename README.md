# St. Martin, Liedanzeiger #

Many of the old fashioned displays in churches face problems when searching for spare parts i.e. bulbs and resting switches. I found a very nifty way to do a replacement using "https://github.com/mrazekv/church-numbers",
where a system with HDMI-Monitor and raspberry-Pi zero 2W is shown as a solution.
The invest is very small, currently used 24"-Monitors are cheap, a "raspberry pi zero 2W" is less than 20€ and the input can be done with any browser on tablet/mobile-phone/notebook.

The minium you need is:

  **Full HD-Monitor** with HDMI input,
  
  **raspberry pi zero W** or **raspberry pi zero W** including **µSD-card 8GB minimum**,
  
  **tablet / mobile phone / PC / notebook**,
  
  **HDMI cable** and a **USB-power supply**.
  
The code for the µSD cards ready to start you can get from this site. If there is the requirement for a second display (side aisles) a here called Sat(telite) version can be downloaded and enabled in the code. 

Finally it looks like this:
![Front](https://github.com/burneme/Liedanzeiger/blob/main/Front.JPG)
![ipad3](https://github.com/burneme/liedanzeiger/blob/main/Ipad3.JPG)



# What you need to do #

Download the image file and use "Balena_etcher" and flash your µSD-card. Insert the card into the raspberry pi zero, connect HDMI-output to monitor and power on.

![balena](https://github.com/burneme/liedanzeiger/blob/main/Balena.png)

It is necessary for a proper start to have a connected, ready monitor. After boot time of approx. half a minute (rasp pi zero 2W), you should recognize a Wifi-station "StMartin", the password is set to "Epiphany", you can change it later.
