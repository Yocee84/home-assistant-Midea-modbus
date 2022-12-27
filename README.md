[![hacs_badge](https://img.shields.io/badge/HACS-Default-orange.svg)](https://github.com/hacs/integration) ![GitHub all releases](https://img.shields.io/github/downloads/wimb0/home-assistant-saj-modbus/total) ![License](https://img.shields.io/github/license/wimb0/home-assistant-saj-modbus)
# home-assistant-saj-modbus
Home Assistant Custom Component for reading data from Midea and clones Heat pump through modbus over TCP.
This integration should work with Concept, Hajdu, Immergas Heat Pump.


Implements Midea and clones Heat pump registers from [`KJR-120X user manual`](https://hajdurt.hu/files/downloads/b00000114hpdf-20221129154519.pdf).

Based on [`home-assistant-solaredge-modbus`](https://github.com/binsentsu/home-assistant-solaredge-modbus) from [@binsentsu](https://github.com/binsentsu).

## Installation
This integration is not available in the HACS default repository.

Search for "Midea-modbus" and install it.

After reboot of Home-Assistant, this integration can be configured through the integration setup UI

## Connection via Modbus TCP to a Midea Heat Pump
Connect a Modbus to Wifi device to the Modbus port of your SAJ Inverter.
I use a Hi-Flying Elfin-EW11 (www.hi-flying.com/elfin-ew10-elfin-ew11).

**Cable Layout for EW11A to KJR-120x Remote Controller:**

Both connectors are RJ45.
![cable](https://github.com/wimb0/home-assistant-saj-modbus/blob/dev/images/cable.png)

**EW11A settings:**

**Communication settings:**
* Configure Tcp Server, choose a port number.
* Security: Disable
* Route as Uart

**Serial port settings:**
* Baudrate 9600
* Databit 8
* Stopbit 1
* Parity None
* Cli Disable
* Protocol Modbus

[![saj_logo](https://github.com/wimb0/home-assistant-saj-modbus/blob/main/images/saj_modbus/logo.png)](https://www.saj-electric.com/)

