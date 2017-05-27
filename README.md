# Ansible wifi router

Wifi router setup playbook based on [How-To: Turn a Raspberry Pi into a WiFi router](http://raspberrypihq.com/how-to-turn-a-raspberry-pi-into-a-wifi-router/).

## Setup

Change [router] group target IP to your target machine.

## Make installation

```
ansible-playbook -i hosts provision.yml
```
