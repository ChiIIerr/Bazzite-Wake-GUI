# Bazzite USB/Bluetooth Wake Configurator

Welcome to Linux! If you're using [Bazzite](https://bazzite.gg/) (or another KDE Plasma-based system) and want your Bluetooth controller or USB mouse to wake your PC from sleep, you're in the right place.

Normally, setting this up requires typing commands to find hardware ID numbers and manually editing system files. This script handles all of that for you by providing a simple, familiar graphical menu. Just check the boxes for the devices you want to use, and the script does the rest.

## Features
* **Built for Bazzite:** Uses the graphical tools already built into your system (`kdialog`). You don't need to install any extra software or mess with Bazzite's core files.
* **Beginner Friendly:** Automatically scans your hardware and shows you plain-English names (like "Logitech Mouse" or "Intel Bluetooth") instead of confusing system paths.

---

## Step 1: Making the Script Executable

Before Linux will allow a script to run, you have to explicitly give it permission. This is a built-in security feature to stop malicious files from running on their own. You can do this using your mouse or the terminal.

### Method A: The GUI Way (Recommended)
1. Open your file manager and find the `usb-wake-config.sh` file you downloaded or created.
2. **Right-click** the file and select **Properties** at the bottom of the menu.
3. Click on the **Permissions** tab at the top of the window.
4. Check the box next to **Is executable** (it might also say "Allow executing file as program").
5. Click **OK**.

### Method B: The Terminal Way
If you prefer using the terminal, open your console, navigate to where the file is saved, and run this command:
```bash
chmod +x usb-wake-config.sh
