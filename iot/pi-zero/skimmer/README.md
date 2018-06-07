
Saw this project in Make Magazine Vol 68, June/July 2018

My notes from this project

## Use PiBakery to install a Raspberry Pi image onto the SD card 

1. On First Boot 
2. Setup Wifi so that the Pi Zero connects your wifi network and gets an IP address

## After getting a ssh session to the Raspberry Pi Zero, run the following commands

Install Python 
```
sudo apt-get install python python-pip
```

Install the bluetooth tools 
```
sudo apt-get install bluetooth libbluetooth-dev
sudo pip install pybluez
```

Software to drive the Adafruit OLED panel
```
sudo pip install RPi.GPIO
sudo pip install Adafruit_BBIO
sudo apt-get install python-imaging python-smbus 
```

Libraries for Adafruit for the OLED display
```
sudo apt-get install git
git clone https://github.com/adafruit/Adafruit_Python_SSD1306.git
cd Adafruit_Python_SSD1306/
sudo python setup.py install
```

## Get the Skimmer code and run it

```
cd ~
git clone https://github.com/photoresistor/raspi_skimscan
cd raspi_skimscan
python raspi_skimscan.py
```
