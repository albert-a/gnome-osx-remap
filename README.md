# GNOME OSX Keyboard Remapper for Wayland

This keyboard remap is based on the [Xremap](https://github.com/k0kubun/xremap) functionality and works with Wayland and Xorg.

## How does it work?
Script downloads the latest version of the `xremap` remapper for your architecture. Configuration file `/etc/factory/default.yml` contains majority of the remapping instructions. On top of that the default GNOME shell and Mutter keybindings are modified. A systemd system service is created and enabled. 
Special tool is installed alongside the service, so that the other users can control remapping independantly.

## Installation
1. Make sure you are running **Wayland** display server. Logout from your session. On the GNOME login screen click ⚙ icon on the bottom right. Select `GNOME` (defaults to Wayland). Log in.
2. Check out this repository run `install` script in Terminal. Script will ask for administrator password.

```
git clone https://github.com/albert-a/gnome-osx-remap
cd gnome-osx-remap
./install
```

3. Restart your computer.

## How to uninstall

1. If repository was removed, check it out again. Navigate into the program directory in Terminal and run:

```
./uninstall
```

2. Restart your computer.

## Changelog

`Jan 06, 2025` • Initial commit. Based on this excellent project: [GNOME macOS Keyboard Remap for Wayland](https://github.com/petrstepanov/gnome-macos-remap-wayland)
