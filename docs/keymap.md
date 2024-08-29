---
title: Keymap
parent: Settings
nav_order: 4
---

# Keymap

You can register custom hotkeys to open the plugins in the Keymap setting. To create a new hotkey, simply press the `+` button. Then specify the plugin, the action and the hotkey.

In the Installed Plugins section, you’ll find the IDs for each plugin in the upper right corner.

For actions, you can choose between `Open Plugin` (this simply opens the desired plugin) and `Open current selection in Plugin`, which will copy the current selection in any other app and load it into the search bar of Smartclip.

To input hotkeys that are currently bound to system functions and would close Smartclip, simply just input the desired key without modifies like `Ctrl` or `Super` and activate the modifiers by clicking them. After that, you can submit the hotkey.

## Windows

Please be aware of a bug related to the global hotkeys: When locking your display with `Super` + `L`, this will currently pin the Windows key after logging back in, leading to all input being handled as though the Windows key was pressed. To resolve this issue, just tap the Windows key once.

## Linux

Please also note that key combinations work via setting custom gnome settings key combinations. If you want to override system behavior, you need to go to `Settings -> Keyboard -> View and Customize Shortcuts` and remove the default system behavior attached to the key combinations you want to