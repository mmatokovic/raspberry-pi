# Raspberry-Pi

instructions for configuring Raspberry Pi Zero 2 w with docker running:
* Portainer
* AdGuard
* nginx proxy manager
* Heimdall

## Requirements

* Raspberry Pi Zero 2 w
* USB SD card reader adapter
* micro usb to usb for Power
* Zenmap software

## 1. PreInstallation

* Using [Raspberry Pi Imager](https://www.raspberrypi.com/software/) boot [Raspberry Pi OS Lite](https://www.raspberrypi.com/software/operating-systems/#raspberry-pi-os-64-bit)

* Setup WiFi on a Pi Manually using `wpa_supplicant.conf` by moving a file to :/boot

* Open nmap and Quick scan `nmap -T4 -A -v 192.168.5.0/24`
    * W8 few mi for RaspberryPi to boot
    * try to see if you can see if there is a IP and green light stoped flashing
    * Login to router and check	> Active clients to see hostname and IP address and MAC address


## Installation

SSH into pi `ssh pi@raspberrypi.local`.

Update OS `sudo apt update && sudo apt upgrade -y`

Install docker `sudo apt install docker.io`.

### Useful links

https://docs.docker.com/engine/install/ubuntu/  
https://docs.portainer.io/start/install/server/docker/linux

https://www.youtube.com/watch?v=vBgCZvCDFh8
https://www.youtube.com/watch?v=o7nn