# Ansible wifi router

Wifi router setup playbook based on articles [Turn a Raspberry Pi into a WiFi router](http://raspberrypihq.com/how-to-turn-a-raspberry-pi-into-a-wifi-router/) and [Configuring your Onboard Computer as a WiFi Access Point](https://pixhawk.org/peripherals/onboard_computers/access_point). Thanks for article writers. Only default hostapd package used in this version. It worked with my `Ralink RT2870/RT3070` component.

This script is best used in local network. Connect Raspberry Pi with ethernet cable to working router and use this script from the same network.

Scripts are made for [Raspbian Jessie](https://www.raspberrypi.org/downloads/raspbian/), but might also work with other linux distros using APT package manager.

## Setup

- You need Raspberry Pi with SSH connection and connection to internet.
- Add your used SSH key as authorized keys.
- Copy `./hosts.example` to `./hosts` and change target IP.
- Change default variables if needed from `group_vars/all`.

## Make installation

**Notice!** Last playbook task will reboot target.

```
ansible-playbook -i hosts provision.yml
```
