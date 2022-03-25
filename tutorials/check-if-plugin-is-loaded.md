# Check if plugin is loaded

Example to check within new\_game() of your mapscript if WarriorLib is installed by the player

```lua
function new_game()
	if WarriorLib then
		dbg.stm("WarriorLib has been found")
	else
		dbg.stm("WarriorLib is not installed")
	end
end
```
