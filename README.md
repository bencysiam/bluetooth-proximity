# BLE and Classic Bluetooth Proximity

Some basic python3 PoC code to scan for nearby devices and 'follow' a device given a specific device address. This will identify when that device is in or out of range and show on screen an updating RSSI giving an indication as to how far away that device is.

## There are some dependencies!

Make sure you have python 3 and pip working first off, then install the dependencies...

```
sudo apt update
sudo apt install bluetooth bluez libbluetooth-dev libglib2.0-dev
sudo pip3 install pybluez
sudo pip3 install bluepy
```

## Usage

### Bluetooth Classic 

```
Usage:
  ./btclassic-prox.py -h or --help = print this help
  ./btclassic-prox.py -s = scan for Bluetooth IDs
  ./btclassic-prox.py -s 10 = scan for Bluetooth IDs for 10 seconds
  ./btclassic-prox.py -f xx:xx:xx:xx = continuously scan for this device
```

### BLE

```
Usage:
  ./ble-prox.py -h or --help = print this help
  ./ble-prox.py -s = scan for Bluetooth IDs
  ./ble-prox.py -s 10 = scan for Bluetooth IDs for 10 seconds
  ./ble-prox.py -f xx:xx:xx:xx = continuously scan for this device

```
