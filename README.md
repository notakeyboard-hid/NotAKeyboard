![nak](https://prankapple.is-a.dev/resc/nak_logo.png)

# NotAKeyboard
Another USB HID device. The name is inspired by NaK, the extremely dangerous Na and K alloy.

**(if you do not want to go thru this setup you can use [the automatic NaK builder](https://github.com/notakeyboard-hid/notakeyboard_builder) for the software)**
## This project is intended for educational and learning purposes only. It is not designed, tested, or intended for use in production, commercial, or real-world environments. The authors assume no responsibility for any misuse of this material.

#### Documentation website
- [NotAKeyboard site](https://notakeyboard-hid.github.io/)

## Setup
![EXAMPLE](docs/example.png)
- You first need to connect GPIO11 with a switch to GND like the upper image, set the switch to off
- Connect the Raspberry Pi Pico to your computer while holding down the BOOTSEL button. When it appears as a removable storage device, release the BOOTSEL button.
- Download this repository and extract it, open the **format_pico** folder from the files provided. Copy the **flash_nuke.uf2** file to the Raspberry Pi Pico. Wait until it restarts. This process clears the existing firmware.
- Open the **software** folder. Copy the **adafruit-circuitpython-raspberry_pi_pico-en_US-9.1.1.uf2** file to your Raspberry Pi Pico. Wait until it restarts. After restarting, the Pico should appear as a drive named CIRCUITPY.
- Copy the **lib** folder on the CIRCUITPY drive, click replace if it asks.
- Copy the **payload.py**, **code.py** and **boot.py**, click replace if it asks. Congratulations! Your NaK is set up and ready to go. (WARNING: MAKE SURE THAT THE SWITCH IS NOT ON)

## Payloads
Head to [NaK DuckyScript converter](https://notakeyboard-hid.github.io/converter.html) and paste your script click convert(keep in mind that very much DuckyScript does not work.) then download and plug in the pico with the switch off.
Copy the **payload.py** you downloaded to the root of your pico and click replace if it asks.

## Usage
Eject and unplug the pico from your device. Turn the switch on.
#### Warning: As long as the pico has the switch on it will be armed. That means if you plug it in while armed it will run the payload with very fast speeds. YOU HAVE BEEN WARNED. I AM NOT RESPONSIBLE FOR ANY DAMAGE CAUSED TO DEVICES.

## Editing the payload
Take your pico and turn the switch off, plug it in and edit

### Have fun.
