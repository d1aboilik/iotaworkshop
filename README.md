![IOTA Workshop](https://i.ibb.co/q79SgmW/IOTA-WORKSHOP-BLACK.png)

# Statement of Purpose



# Installation

First please check with the [wiki](https://github.com/Tsangares/iotaworkshop/wiki) on the parts you need and the how to wire the device, then you can proceed on installing the software.


To run this program you need to clone the repo or pull the `iotaworkshop.py` file, then install the dependencies,

    pip install iotaescrow servo_lock pibeep piepd rc522
    
You will also need `RPi.GPIO`, which because I was running an arch arm operation system I installed it using the arch aur repo using,

    yay -S python-raspberry-gpio
	
If you are using ubuntu orrasbian you can use,

    pip install RPi.GPIO


# Contents

Please view the [wiki](https://github.com/Tsangares/iotaworkshop/wiki) to see a list of the components and how to compile them together to replicate the IOTA Workshop proof of concept. 

The following is a abstract on how the program runs. This project contains is the logic involved with creaing a vending equipment serivce. Fully autonomous and operated using the IOTA ledger. An e-paper display interfaces with the user to guiding them through depositing IOTA into an escrow account. This operates a servo that is pick proof to unlock a box that gives access to an tool which is the instrument of producion. When the user retuns the tool, an RFID sensor will detect and confirm the tool has been returned and will finish the escrow by returning the deposit on the tool. The servo then proceeds to lock the box, disabling people from trying to steal the tool inside. 

# Dependencies

All of the code used in this project is encapulsated into a easy to use pip package. Many of them have command line interfaces to use the tool and they can all be imported as a module to have enable advanced usage. The following project uses these packages that I built, each of which holds a general purpose beyond this project.

 - <a href="https://github.com/Tsangares/iotaescrow" target="_blank">iotaescrow</a>: A escrow implementation using IOTA.
 - <a href="https://github.com/Tsangares/servo_lock" target="_blank">servo_lock</a>: A general purpose, high level servo controller.
 - <a href="https://github.com/Tsangares/pibeep" target="_blank">pibeep</a>: A buzzer utility that offers a variety of sounds and enables tools to make any sound possible using buzzers.
 - <a href="https://github.com/Tsangares/piepd" target="_blank">piepd</a>: A e-paper controller that displays text or QR codes using any of the waveshare screens.
 - <a href="https://github.com/Tsangares/rc522" target="_blank">rc522</a>: An RFID sensor utility used to confirm and verify RFID tags for the rc522 sensor.

# Images of POC
![Front](https://i.imgur.com/urNxrml.jpg)
![Back](https://i.imgur.com/hEpKakq.jpg)
![Inside](https://i.imgur.com/opdZAft.jpg)
![Close Up](https://i.imgur.com/i3mrwzj.jpg)
