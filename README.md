# [FocusME](https://github.com/dixflat/FocusME/)
Helper script to focus open Linux/X window apps or launch another instance if window is already active or not found. 
You can forget the hordes of orphaned terminals or myriads of app windows.

It works by querying the open window names/classes for a string, then:

- If found it activates/focuses it.
- If not found it will launch the specified command.
- If the window is found and it's active it will launch a new one.

## Installation / required packages
1. Install xdotool (apt install xdotool / apk add xdotool)
2. Copy focusme to /usr/local/bin or somewhere inside your PATH
3. chmod ug+x /usr/local/bin/focusme
4. Setup shortcuts in your favorite window manager

## Usage, examples
```
focusme <windowname> <command_to_launch>

windowname - text part of the window name
command_to_launch - the command to launch if window not found or already active

focusme terminal xfce4-terminal
focusme firefox "firefox -P MAIN"

```

## In action
![FocusME in action](https://raw.githubusercontent.com/dixflat/focusME/main/focusme_example.gif)
