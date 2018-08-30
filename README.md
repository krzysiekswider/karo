# karo-gabi
Arduino-Raspberry Pi networking project

## Karo (Raspberry Pi 3 B+)

- WiFi
- Ethernet
- Bluetooth
- Surfstick (Huawei, ZTE)
- SimCon SIM900A (GSM/GPRS)
  - can be used to connect RPi to public server via GPRS (G2, G2.5, G3?)
  - to be reachable from outside a public IP is necessary
  - public APN (IP) is very hard to become at present due to IPv4 addressing limitation. In 2019 Telekom should make IPv6 officially available.
- 433Mhz RF Communication Receiver (RF=Radio Frequency)
- nRF24L01+ 2.4GHz
- see
  - https://electronics.stackexchange.com/questions/144358/wireless-home-automation-2-4ghz-versus-433mhz
  - https://forum.arduino.cc/index.php?topic=111847.0

- Web Stack:
  - Operating system -> Raspbian (Debian derivate)
  - Web server -> nginx, Apache
  - WSGI server -> Green Unicorn, uWSGI, mod_wsgi, CherryPy
  - Web microFramework -> Flask (Python)
  - Database -> OrientDB, MariaDB, SQLite
  
- Rasbpian
  - Mosh (MobileSSH)
  - Docker on RaspPi
    - https://blog.alexellis.io/live-deep-dive-pi-swarm/
    - https://blog.alexellis.io/getting-started-with-docker-on-raspberry-pi/
    - https://github.com/docker-library/official-images
    - https://hub.docker.com/r/arm64v8/mediawiki/
    - https://hub.docker.com/r/arm64v8/alpine/
  - https://github.com/alexellis/pizero-docker-demo/tree/master/iotnode

## Gabi (Arduino Uno Rev. 3)

- 433Mhz RF Communication Transmitter
  - https://www.instructables.com/id/Wireless-communication-Arduino-RF/
  - ESP8266, nRF24L01 and 433MHz module
  - In Europe, the 433MHz, 868MHz and 2.4MHz can be used with limited power
  - For the 433MHz, a transmitter may only transmit during 10% of the time
  - There are good transceiver modules for 433MHz and 2.4GHz. Google for "Sparkfun wireless buying guide" to see a nice list of possibilities. Or check the modules that are supported by the RadioHead library at airspayce.com/mikem.

## Fran (Public server)

- to be established
