# winbox-linux-installer
Helper script for installing the linux version of Winbox
This code is a modification of https://github.com/mriza/winbox-installer

## Feature:
1. Only Supported GNU/Linux distributtions: Debian Base (Ubuntu, Elementary OS, Zorin OS, Linux Mint, Kali Linux)
2. Download the latest Winbox from the Mikrotik website
3. Extract the downloaded ZIP file
4. Check if ImageMagick is installed, and install it if not
5. Resize the icons to 48, 64, 128, and 256 px
6. Copy the executable file to the /usr/local/bin/ directory
7. Copy the resized icons to /usr/share/icons/hicolor/*/apps
8. Create a launcher for Winbox
9. Update desktop menu and icon cache

## How to install:
Copy and paste this commands to your terminal:

1. `cd /tmp`
2. `git clone https://github.com/origrata/winbox-linux-installer.git`
3. `cd winbox-installer`
4. `sudo ./Winbox-Setup install` **OR** `sudo bash Winbox-Setup install`

## Icon cache in GTK based desktop:
Optional step for GTK based desktop, if the icon is not loaded or loaded with wrong size. Update icon cache with this command:

`gtk-update-icon-cache -f -t /usr/share/icons/hicolor`

## How to remove:
If you want to remove winbox, just run this command:

sudo ./Winbox-Setup remove` **OR** `sudo ./Winbox-Setup remove`

