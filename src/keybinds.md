# Key / AUX switch binds

## Creating a keybind

You can create keybinds for AUX switches using the `bind` command.

The command is structured like this:

`/bind aux SWITCH_NUMBER VALUE COMMAND`

The SWITCH_NUMBER for your real AUX switches starts at 4, with 0, 1, 2, 3 being your gimbals.

The VALUE can be low, mid, high.

The COMMAND can be any of the other available commands.
Only one command is supported per keybind, but you can create multiple binds for a single switch.

Examples:

Save checkpoint location when setting AUX 2 to HIGH.

`/bind aux 5 high saveloc`

Respawn at checkpoint when setting AUX 3 to HIGH.

`/bind aux 6 high loadloc`

## Checking what keybinds are configured

You can get a list of all configured keybinds using

`/listbinds`

## Removing a keybind

You can remove a keybind using

`/unbind BIND_ID`

where BIND_ID is the # from the `/listbinds` command.

## HELP ITS NOT WORKING!!

For the AUX switch to be detected by the game, it must be configured in your Radio's Mixer.
Please double check if there is something being sent from your Radio when pressing the switch using the Channels monitor.

If that works, you can enable the Channel monitor in-game using the command

`/debugger`

It will show you all the channels the game is receiving and their corresponding values.
