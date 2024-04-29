# Is the plugin loaded?

Example to check within new_game() function of your mapscript if WarriorsLib is installed by the player

```lua
function new_game()
	if WarriorsLib then
		dbg.stm("WarriorsLib has been found")
	else
		dbg.stm("WarriorsLib is not installed")
	end
end
```
