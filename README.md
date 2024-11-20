# i3wm_myenv

Custom environment for i3WM.

## Scripts

### switch_ws
Switch between workspaces on a single output (rather than using `workspace next` in the config which switches between ALL workspaces on ALL outputs. Please set `$out1` and `$out2` accordingly (`$> xrandr`)

### open_ws
Open a new workspace automatically, on the same screen. Please setup and run <b>list_ws</b> before, this will generate a ws_list.txt file associating the $ws variable with a name and an output <b>that open_ws</b> will use to look for new workspaces.
