---
title: Installation
nav_order: 1
---

# Installation

To install Smartclip head to the [Releases Page of the Github Repository](https://github.com/muelphil/smartclip/releases) and download the latest installer. If you are on Windows, download the `.exe` file, on Linux download the `.deb` file. As of now the source code for Smartclip is not publicly available.

## Windows

Simply follow the instructions of the Installer.

## Linux

Please note that this tool will only work under non wayland display managers, like X11. To check if you are running on wayland type `echo $XDG_SESSION_TYPE` into your terminal, in case of running on wayland display manager this will yield `wayland`.

The Reason is that wayland prohibits sending keystrokes across windows, which makes it impossible to send a paste event, which is necessary for pasting clipboard entries, translations, and emojis.

For Ubuntu, right-click the `.deb` installer file and choose `Open with Software Install`. Depending on your operating system version, this may vary.

For other Linux distributions please consult the Internet on how to install `.deb` files.
