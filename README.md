# i3wm_autows
Simple bash script for opening new workspaces automatically (that is, without having to manually pressing $mod and [1...0]). New workspaces are opened on the same output as the focused workspace unless no workspace is available (not focused, active or opened).

## Installation
Download the file new_ws wherever you want it to be on your system and add a bindsym in your i3WM config file
```css
bindsym your+bind+sym exec --no-startup-id path/of/your/script
```

## Customisation
Please check if the variable WS_MAX (line 7) correponds to your current amount of workspaces; otherwise you will be limited to that amount (unless workspaces are opened manually).

You might assign your workspaces to a given output. I personally assign the odd number workspaces to output 1 and the even number workspaces to output 2.
This script, with the variable "evenodd" (line 5) can open workspaces depending on that preference, i.e. open ws 5 on output 1 instead of output 2 even if the current focused workspace is on output 2.
By default, this var is set to false; ws 6 will be opened on output 1 if the script is ran on output 1. Otherwise, please consider:
```css
EVEN_ODD=true
```

## To do
* Translate this script in zsh
