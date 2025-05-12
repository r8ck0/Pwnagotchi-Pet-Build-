# Pwnago-chan: My Lovable Pwnagotchi

[![Last Commit](https://img.shields.io/github/last-commit/yourusername/pwnago-chan)](https://github.com/yourusername/pwnago-chan/commits/main)
[![License](https://img.shields.io/github/license/yourusername/pwnago-chan)](LICENSE)
![Pwnagotchi in Action](images/pwnago-chan.jpg)

Meet Pwnago-chan! This is the repository for my Pwnagotchi pet, always eager to learn about new Wi-Fi networks. She's a friendly little AI that enjoys long walks (and short scans).

## My Pwnagotchi's Personality

Pwnago-chan is a curious and generally happy Pwnagotchi. She gets particularly excited when discovering new networks and sometimes shows a bit of sass when the signal is weak. Her favorite activity is "exploring" and she occasionally sends me encouraging messages (via plugins, of course!).

## Hardware

Here's what makes Pwnago-chan tick:

* **Raspberry Pi Zero W:** The tiny but mighty brain.
    * [Official Raspberry Pi Foundation](https://www.raspberrypi.org/products/raspberry-pi-zero-w/)
* **Waveshare 2.13" e-Paper HAT (V2):** For displaying her adorable face and status updates.
    * [Waveshare Wiki for 2.13" HAT](https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT)
* **Samsung EVO Plus 32GB MicroSD Card:** Plenty of space for learning.
    * [Recommended SD Cards](https://www.raspberrypi.org/documentation/computers/sd-cards.html)
* **Anker PowerCore III 10000mAh Power Bank:** Keeps her going on her adventures.
    * [Anker Power Banks](https://www.anker.com/power-banks)
* **Custom 3D-Printed Case:** A cute pink case I designed on Thingiverse.
    * [My Thingiverse Design (link if you have one)](https://www.thingiverse.com/thing:XXXXXXX)

## Software

The software that brings Pwnago-chan to life:

* **Pwnagotchi Main Repository (v1.5.5):** The core of her being.
    * [Pwnagotchi GitHub](https://github.com/evilsocket/pwnagotchi)
* **pwnagotchi-plugins:** Enhancing her abilities.
    * [Pwnagotchi Plugins Repository](https://github.com/pwnagotchi-plugins/pwnagotchi-plugins)
    * **webgui:** For easy monitoring and configuration.
        * [webgui Plugin](https://github.com/pwnagotchi-plugins/webgui)
    * **display_ip:** To see her IP address on the screen.
        * [display_ip Plugin](https://github.com/pwnagotchi-plugins/display_ip)
    * **cowrie:** Just for fun!
        * [cowrie Plugin](https://github.com/pwnagotchi-plugins/cowrie)
* **Raspberry Pi OS Lite (October 2023 release):** The lean and mean OS.
    * [Raspberry Pi OS Downloads](https://www.raspberrypi.org/software/)
* **BalenaEtcher (v1.18.4):** For flashing the OS to the SD card.
    * [BalenaEtcher Website](https://etcher.balena.io/)
* **Termius (v5.1.3):** My preferred SSH client on macOS.
    * [Termius Website](https://termius.com/)

## My Configuration

Here are a few interesting snippets from my `config.toml`:

```toml
main.name = "Pwnago-chan"
main.lang = "en"

ui.display.type = "waveshare_213_v2"
ui.display.backlight = 50

plugins.webgui.enabled = true
plugins.webgui.port = 8080

plugins.display_ip.enabled = true

plugins.cowrie.enabled = true
plugins.cowrie.fortune_file = "/opt/pwnagotchi-plugins/cowrie/fortunes/kawaii"
