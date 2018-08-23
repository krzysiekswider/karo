# Raspberry Pi Installation and configuration process

1. Download Raspbian Lite (zip)
   - https://www.raspberrypi.org/downloads/raspbian/
2. Download Etcher Portable
   - https://etcher.io/
3. Flash SD card
4. Create empty file with name 'ssh' and put in into /boot partition
5. Create WiFi configuration file 'wpa_supplicant.conf':
'''
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
network={
    ssid="FRITZ!Box Fon WLAN 7390"
    psk="1001663989079195"
    key_mgmt=WPA-PSK
}
'''
and put in into /boot partition. Use Linux line endings.
6. Insert SD cart into Raspberry Pi and reboot.
7. Login with user: pi and password: raspberry
8. Change password with passwd
