# uvc-exposure

Little console app that sets exposure to manual mode using libuvc

# Disclaimer

Hacked together in minutes, tested and works in OS X, may work in GNU/Linux too.
Tested on Logitech C920 (usb ids: ```046d:082d```)


# Installation

* ```brew install libuv```
* clone repo to any dir
* ```mkdir build```
* ```cmake ..```
* ```make```
* put executable 'uvc-exposure' to any location (I use ```~/bin```)

uses 2 calls from libUVC:

* [uvc_set_ae_mode](https://int80k.com/libuvc/doc/group__ctrl.html#gaa583133ed035c141c42061d5c13a36bf) - to switch to manual exposure (1 on C920)
* [uvc_set_exposure](https://int80k.com/libuvc/doc/group__ctrl.html#ga5309474eaea2ebc22ffc74c64c7a4b59) - sets the exposure

