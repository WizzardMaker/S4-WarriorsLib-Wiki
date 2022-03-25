# Is the plugin loaded?

Example to check within new\_game() function of your mapscript if WarriorLib is installed by the player

```lua
function new_game()
	if WarriorLib then
		dbg.stm("WarriorLib has been found")
	else
		dbg.stm("WarriorLib is not installed")
	end
end
```
