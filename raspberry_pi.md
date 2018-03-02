# Raspberry Pi for the Bitfab Core


## Objective

Set up and run a Raspberry Pi for using it with a Bitfab Core 3D printer. This includes preparing the SD card with the Octopi image, changing the machine hostname and password and connecting to the printer for the first time.


## Requeriments

### Skills

* Some terminal basic knowledge: `ssh`, `passwd`...

### Materials

* Raspberry Pi 3
* microSD card (we use SanDisk microSDHC UHS-I Ultra 16 GB)


### Software

* Etcher: https://etcher.io/
* Text editor, for example, Sublime Text: https://www.sublimetext.com/
* Bonjour support for connecting to Octoprint with `hostname.local` url:
	* Mac: supported out of the box
	* Windows: install Bonjour Print Services for Linux (https://support.apple.com/downloads/bonjour_for_windows)
	* Linux: `sudo apt-get install avahi-daemon` or `sudo apt-get install netatalk` (Source: https://learn.adafruit.com/bonjour-zeroconf-networking-for-windows-and-linux/overview)

### Downloads

* Download Octopi latest version (Raspbian image with Octopring configured): https://octoprint.org/download/

## Setting up Octoprint in the Raspberry Pi 3

* Burn the Octopi image in the SD card
	1. Unzip the Octopi image
	2. Insert SD card in your computer
	3. Open Etcher
	4. Open the Octopi image (extension `.img`) with Etcher to burn it in the SD carc
	5. Burn the image in the SD card by clicking Flash
* Configure the wifi connection
	1. Open the SD card directory
	2. Open the `octopi-network.txt` with the text editor. *Important: Do not use WordPad (Windows) or TextEdit (MacOS X)* ([source](https://octoprint.org/download/))
	4. Change the network settings. Leave the quotation marks.

	## WPA/WPA2 secured
	iface wlan0-octopi inet manual
    wpa-ssid "wifi name"
    wpa-psk "wifi password"

* Connect to the Raspberry Pi
	1. Insert the SD card in the Raspberry Pi
	2. Power the Raspberry Pi. LED lights will start to blink. The Raspbberry is booting up and connecting to the wifi network.
	3. Connect to the Raspberry Pi with SSH
		* The default Octopi hostname is `octopi`, so the Raspberry address is `octopi.local`
		* Default username is `pi`
		* Default password is `raspberry`
		* Therefore you have to run the following command in the terminal: `ssh pi@octopi.local` and give the password `raspberry`
	4. Change user password. Use Bitfab password rules for the printers (ask tutor if you need help).
		1. Run `sudo raspi-config` ([raspi-config documentation](https://www.raspberrypi.org/documentation/configuration/raspi-config.md))
		2. etc
	5. Change Raspberry Pi hostname for the printer identifier. Use Bitfab identifier rules for the printers (ask tutor if you need help).
		1. Run `sudo raspi-config` ([raspi-config documentation](https://www.raspberrypi.org/documentation/configuration/raspi-config.md))
		2. etc
* Connecting to the printer.
	1. Open a browser
	2. Go to `http://<hostname>.local`, where `<hostname>` is the Raspberry Pi hostname (also the machine identifier) that we have set up in the previous step.
	3. Octoprint should load up if everything is correct. You have connected to Octoprint for the first time.


## Additional resources:

* Octopi installation guide: https://octoprint.org/download/
* Raspberry Pi documentation for installing images (this is an alternative to using Etcher): https://www.raspberrypi.org/documentation/installation/installing-images/README.md