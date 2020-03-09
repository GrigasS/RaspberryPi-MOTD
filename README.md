# RaspberryPi-MOTD
Custom made and tweaked RaspberryPi "Message of the Day"
Make your SSH logins look cool

Original Thread: [Custom MOTD - Message of the Day](https://www.raspberrypi.org/forums/viewtopic.php?t=23440)

My changes include:

1. Code readability
2. RAM value is written in MB instead of kB
3. Capable of displaying free space on one, two or even more disks (need to edit yourself) 

Features:
* OS Version
* Up Time
* Free/Total Memory
* Running Processes Count
* Free Disk Space
* IP Addresses - LAN and WAN
* Weather Information

# Roadmap

Features that might never be implemented:

1. Automatically find disks and show their storage space
2. Automatic installation script

# Installatio

1. Clone this repo/download the "10-uname" file
2. Import/Overwrite the file to "/etc/update-motd.d" folder
3. CHMOD a+x /etc/update.motd.d/*
4. RM -F /etc/motd
5. EDIT /etc/ssh/sshd_config
```  
  USEPAM yes
  PasswordAuthentication no
  ChallengeResponseAUthentication no
```
Be careful editing this and google before what those values do!
