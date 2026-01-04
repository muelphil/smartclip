---
title: Installation
nav_order: 1
---

# Installation

By downloading and installing Smartclip, you agree to the [Terms of Agreement](https://github.com/muelphil/smartclip/blob/main/LICENSE).

To install Smartclip head to either the [Website](https://muelphil.github.io/smartclip/) or the [Releases Page of the Github Repository](https://github.com/muelphil/smartclip/releases) and download the latest installer.
- Windows: [`smartclip-0.9.4-windows.exe`](https://github.com/muelphil/smartclip/releases/download/v0.9.4-beta/smartclip-0.9.4-windows.exe)
- Linux: [`smartclip-0.9.4-linux-amd64.deb`](https://github.com/muelphil/smartclip/releases/download/v0.9.4-beta/smartclip-0.9.4-linux-amd64.deb)
- MacOs: Discontinued, as I dont have access to a MacOs device to compile the app anymore

[//]: # (- [`smartclip-0.9.4-macos.dmg`]&#40;https://github.com/muelphil/smartclip/releases/download/v0.9.4-beta/smartclip-0.9.4-macos.dmg&#41;)

As of now the source code for Smartclip is not publicly available.

## Windows

Please note that upon installation you will get prompted with a warning:

<img src="{{ "/assets/images/Windows_Warning.png" | prepend: site.baseurl | prepend: site.url}}"/>

This will go away after a sufficient number of Windows users have installed Smartclip. The only other way for me to stop this message from coming up is paying somewhere around 1000$ to Microsoft for a license, which is currently not an option.

After clicking "Run anyway..." simply follow the instructions of the Installer.

## Linux

Please note that this tool will only work under non wayland display managers, like X11. To check if you are running on wayland type `echo $XDG_SESSION_TYPE` into your terminal, in case of running on wayland display manager this will yield `wayland`.

The Reason is that wayland prohibits sending keystrokes across windows, which makes it impossible to send a paste events, which is necessary for pasting clipboard entries, translations, and emojis.

For Ubuntu, right-click the `.deb` installer file and choose `Open with Software Install`. Depending on your operating system version, this may vary.

You can also install it via Command line using
```shell
cd ~/Downloads/
sudo dpkg -i ./smartclip-<VERSION_NUMBER>-linux-amd64.deb
```

If you have a previous version of Smartclip installed you can uninstall it using
```shell
sudo dpkg -r smartclip
```

For other Linux distributions please consult the Internet on how to install `.deb` files.

## MacOs

As this app is still in beta and I currently don't have the financial means to pay for an Apple Developer Account, this app isn't signed by Apple.
This means, that for installation you need to bypass the Security Settings:

### [Open a Mac app from an unknown developer](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unknown-developer-mh40616/mac)
1. Attempt to install the App by downloading the .deb file, double clicking it and dragging the Smarclip icon into the Applications folder. MacOs will initially block this.
2. On your Mac, choose `Apple menu  > System Settings`, then click `Privacy & Security`  in the sidebar.
2. Scroll down to Security, find the section notifying you about the attempted installation of Smartclip, then click Open. 
3. Click Open Anyway. (This button is available for about an hour after you try to open the app)
5. Enter your login password, then click OK.

<img src="{{ "/assets/images/macos-instructions.png" | prepend: site.baseurl | prepend: site.url}}"/>

You might need to enable Accessibility features on MacOs, which Smartclip uses to send paste events to the system. You can also find this in the System Settings
<img src="{{ "/assets/images/macos-accessibility.png" | prepend: site.baseurl | prepend: site.url}}"/>
