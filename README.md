# Statement of Purpose

# Contents

This project contains the logic involved with creaing a vending equipment serivce. Fully autonomous and operated using the IOTA ledger. An e-paper display interfaces with the user to guiding them through depositing IOTA into an escrow account. This operates a servo that is pick proof to unlock a box that gives access to an tool which is the instrument of producion. When the user retuns the tool, an RFID sensor will detect and confirm the tool has been returned and will finish the escrow by returning the deposit on the tool. The servo then proceeds to lock the box, disabling people from trying to steal the tool inside. 

# Dependencies

All of the code I used in this project I encapulsated into a easy to use pip package. Many of them have command line interfaces to use the tool and they can all be imported as a module to have enable advanced usage. The following project uses these packages that I built, each of which holds a general purpose beyond this project.

 - [iotaescrow](https://github.com/Tsangares/iotaescrow){:target="_blank"}: A escrow implementation using IOTA.
 - [servo_lock](https://github.com/Tsangares/servo_lock){:target="_blank"}: A general purpose, high level servo controller.
 - [pibeep](https://github.com/Tsangares/pibeep){:target="_blank"}: A buzzer utility that offers a variety of sounds and enables tools to make any sound possible using buzzers.
 - [piepd](https://github.com/Tsangares/piepd){:target="_blank"}: A e-paper controller that displays text or QR codes using any of the waveshare screens.
 - [rc522](https://github.com/Tsangares/rc522){:target="_blank"}: An RFID sensor utility used to confirm and verify RFID tags for the rc522 sensor.

<a href="http://example.com/" target="_blank">Hello, world!</a>
