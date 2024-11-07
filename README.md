# Setup Pimoroni HyperPixel Round 2.1 on Raspberry Pi (Bookworm Lite)

## Step 1: Set dtoverlay
```
# Add to end of boot/firmware/config.txt
dtoverlay=vc4-kms-dpi-hyperpixel2r
```
then reboot `sudo reboot`

## Step 2: Disable i2c
`sudo raspi-config nonint do_i2c 1`

## Step 3: Install sdl2
`sudo apt install libsdl2-2.0-0 libsdl2-image-2.0-0 libsdl2-mixer-2.0-0 libsdl2-ttf-2.0-0`

## Step 4: Install libgl
`sudo apt install libegl-dev`

## Install pygame
`sudo apt install python3-pygame`

## Install ALSA (unsure if necessary)
`sudo apt install alsa-utils`
