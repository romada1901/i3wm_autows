# i3wm_myenv

Custom environment for i3WM.

## Scripts

### new_ws
Open a new (unused, not focused) workspace automatically, based on the number associated with the workspace. Set `$EVEN_ODD` to false if you don't have a specific pattern in workspace distribution per output and `$WS_MAX` according to the number of workspaces you have.

### switch_ws
Switch between workspaces on a single output (rather than using `workspace next` in the config which switches between ALL workspaces on ALL outputs. Please set `$out1` and `$out2` accordingly (`$> xrandr`)
