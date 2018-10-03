# Gamepad Zero: a Raspberry Pi Retro Gaming Rig inside an Original NES Controller

## Overview

For this project, we're going to build a Raspberry Pi retro gaming rig inside of an original NES controller. The top half of the controller will be reused, along with the original printed circuit board and button. Of course, we'll be installing RetroPie.

We're going to print a new bottom half to hold our Raspberry Pi and then solder the existing NES controller circuit board to the Raspberry Pi so that it can be used to play games.

Finally, we'll install RetroPie, and the Gamepad Zero will connect directly to your television or computer monitor using a power and HDMI cable.

## Print the bottom half of the controller

Download the model and print it using your filament of choice (we used PLA+, which is a slightly stronger variant of PLA).

## Install RetroPie

RetroPie will allow us to play emulated retro video games. We wrote a separate guide on how to install RetroPie -- it's a super simple process.

## Disassemble your NES controller

We used a copy, with original ports, of the NES controller. The original controller made by Nintendo work as well.

To disassemble the controller, use a small Phillips screwdriver to remove the six small screws from the back of the controller. You can either toss these screws or reuse them -- I decided to toss and replace them with some stainless steel Torx screws to prevent them from stripping in case we need to open my controller a few times.

Note:
Once inside, you may want to give your controller a good cleaning with some rubbing alcohol and Q-tips. There's going to be a lot of strange build-up in there after 30+ years.

## Solder your connections
![Connections](/images/gpio-connections.png)
Cut the cord off your NES controller, leaving about 6" of excess wire. We're going to reuse the old wires and solder them directly to the Pi Zero.

Using the attached wiring diagram, solder the 5 wires from your original NES controller onto the Pi Zero's GPIO header.

## Mount your Pi

Use four 5mm screws to secure your Pi Zero into the controller housing.

## Reassemble the housing

Finally, reassemble the controller using five 8mm screws.

Note:
You can also use the controller's original screws here.

## Configure your NES controller for RetroPie

You'll need to add a bit of configuration to let RetroPie recognize your original NES controller. You will need to use a USB keyboard or separate USB gamepad to do this.

Navigate to RetroPie Setup > Manage Packages > Manage Driver Packages and select Option 809: gamecondriver.

Note: Different versions of RetroPie might list gamecondriver as a different index (e.g. 813: gamecondriver). Just select whichever gamecondriver listing you have.

Install from binary, accept the firmware warning, wait for everything to install, and select "no" if prompted to install SNES configs. Exit the setup menu.

Next, you'll need internet access to connect to your Pi -- you can connect to your wireless network using either the RetroPie settings menu or by dropping a file on your SD card.

Finally, connect to your Raspberry Pi and run the following command:
```
sudo sh -c 'echo "gamecon_gpio_rpi" >> /etc/modules && echo "options gamecon_gpio_rpi map=0,0,2,0,0,0" > /etc/modprobe.d/gamecon.conf && reboot'
```
Finally, while your PI is rebooting unplug your keyboard or USB controller and you will see the configuration menu for your NES controller! Woot woot

Note: If you don’t see the configuration menu, don’t panic. Connect a keyboard or different controller and use it to navigate to Start > Configure Input, and then use your GamePad Zero to fill out the confirmation options.

Note:
If you're using the non-wireless version of the Raspberry Pi Zero, you'll need to connect a USB WiFi or ethernet adapter before you can connect to your Pi.

## Ready Player Two!

To play with a buddy or to play games that require more buttons than the NES controller offers, you have two options:

### 1. Connect a USB gamepad:
You can connect a second USB controller directly into your Gamepad Zero. You'll need a small USB to Micro USB adapter to make the connection.

## All done!

This was a super easy but fun project. We hope you enjoyed reading it.
