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
- ELAN Touchpad not working on Debian out of the box
- Webcam only works with uvcvideo (Zoom working but not Skype). Cheese does not recognize webcam either.
- Webcam integrated microphone not working (all distros)
- Similar report has been issued for Arch [here](https://wiki.archlinux.org/index.php/HP_Spectre_x360_-_13-ap0xxxx)

# TODO
- Test fingerprint reader
- Mess with synaptics on Debian
- Report microphone issue

# Tested distros and current state

|                   | Kernel version | Auto-rotate | Touchpad | Microphone |
|-------------------|----------------|-------------|----------|------------|
| Ubuntu 18.04 LTS  | 4.15           | Yes         | Yes      | No         |
| Ubuntu 18.10      | 4.18           | Yes         | Yes      | No         |
| Mint 19 (Tara)    | 4.15           | Yes         | Yes      | No         |
| Mint 19.1 (Tessa) | 4.15           | Yes         | Yes      | No         |
| ElementaryOS 5.0  | 4.15           | Yes         | Yes      | No         |
| PopOS! 18.04 LTS  | 4.15           | Yes         | Yes      | No         |
| Debian stretch    | 4.9            | ?           | No       | No         |
| Debian testing    | 4.18           | ?           | No       | No         |
| Deepin 15.8       | 4.15           | No          | Yes      | No         |
| Deepin 15.8       | 4.16(upgraded) | No          | No(!)    | No         |



# Bottom line

If you don't want to mess around too much for now I would recommend to install Ubuntu-based distros.
As for the microphone on my side I workaround it using a headset with integrated microphone for now...

My original intent was to run Debian on that laptop, I will keep trying though!
