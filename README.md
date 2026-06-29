# Bazzite USB/Bluetooth Wake Configurator

A lightweight, dependency-free Bash script designed for [Bazzite](https://bazzite.gg/) (and other KDE Plasma-based Linux distributions) to easily manage which USB and Bluetooth devices can wake your system from sleep. 

Instead of manually configuring `udev` rules and looking up bus/port numbers, this script provides a simple graphical checklist using KDE's built-in `kdialog`. 

## Features
* **Zero Dependencies:** Uses `kdialog`, which is already built into KDE Plasma. No need to layer packages, use Python virtual environments, or alter Bazzite's immutable filesystem.
* **Wayland Safe:** The GUI launches in your standard user session space, only escalating to root (`sudo`) via the terminal when it actually needs to write the final rules file.
* **State Aware:** Automatically checks your system's current hardware mapping and pre-checks devices that already have wake-up enabled.

---

## Prerequisites
* A Linux distribution running KDE Plasma (like Bazzite).
* `kdialog` (included with KDE by default).
* `sudo` privileges.

---

## Installation

1. Clone this repository or download the `usb-wake-config.sh` script to your local machine. 
   *(Alternatively, you can just create a file using `nano usb-wake-config.sh` and paste the code in.)*
2. Navigate to the directory where the script is located.
3. Make the script executable by running:
   ```bash
   chmod +x usb-wake-config.sh
