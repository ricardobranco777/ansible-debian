
Bluetooth:

```
bluetoothctl
[bluetooth]# default-agent 
Default agent request successful
[bluetooth]# power on
Changing power on succeeded
[bluetooth]# scan on
Discovery started
[bluetooth]# devices
Device MAC_ADDR Cool Shit
[bluetooth]# trust MAC_ADDR
[CHG] Device MAC_ADDR Trusted: yes
Changing MAC_ADDR trust succeeded
[bluetooth]# pair MAC_ADDR
Attempting to pair with MAC_ADDR
[bluetooth]# connect MAC_ADDR
Attempting to connect to MAC_ADDR
[CHG] Device MAC_ADDR Connected: yes
[NEW] Endpoint /org/bluez/hci0/dev_MAC_ADDR/sep1 
[NEW] Endpoint /org/bluez/hci0/dev_MAC_ADDR/sep2 
[NEW] Transport /org/bluez/hci0/dev_MAC_ADDR/sep1/fd0 
Connection successful
[CHG] Device MAC_ADDR ServicesResolved: yes
[CHG] Transport /org/bluez/hci0/dev_MAC_ADDR/sep1/fd0 Volume: 0x003f (63)
[Cool Shit]# 
```
