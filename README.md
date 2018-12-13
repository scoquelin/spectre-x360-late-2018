I am owning an HP Spectre X360 13 (late 2018) and I wanted to share my experience on installing Linux.

At the time of writing there are no review / no report about Linux compatibility for this laptop and that's most likely why you landed here ;-)

# Model number
The reference number of the model I have is `13-ap0028ca`.

# BIOS
I flashed the BIOS from version F7 to F8a using a USB recovery drive.
Instructions are [here](https://support.hp.com/ca-en/document/c02693833).

# Docks
I was able to use a Dell USB-C DA200 (RJ45, USB and HDMI working well)

# Issues
- ELAN Touchpad not working on kernels > 4.15
- Webcam only works with uvcvideo (Zoom working but not Skype). Cheese does not recognize webcam either.
- Webcam integrated microphone not working

# TODO
- Test fingerprint reader
- Test Mint 19 and Ubuntu
- Mess with synaptics
- Report microphone issue

# Tested distros and current state

|                   | Kernel version | Auto-rotate | Touchpad | Microphone |
|-------------------|----------------|-------------|----------|------------|
| Debian stretch    | 4.9            | ?           | No       | No         |
| Debian testing    | 4.18           | ?           | No       | No         |
| Deepin 15.8       | 4.15           | No          | Yes      | No         |
| Deepin 15.8       | 4.16           | No          | No(!)    | No         |
| ElementaryOS 5.0  | 4.15           | Yes         | Yes      | No         |
| PopOS! 18.04 LTS  | 4.15           | Yes         | Yes      | No         |


# Bottom line

If you don't want to mess around too much for now I would recommend to install either PopOS! or ElementaryOS.
As for the microphone on my side I workaround it using a headset with integrated microphone for now...

My original intent was to run Debian on that laptop, I will keep trying though!