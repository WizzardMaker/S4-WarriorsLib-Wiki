# Ist das Plugin geladen?

Beispiel um zu überprüfen innerhalb der new\_game() Funktion ob das WarriorLib Plugin vom Spieler installiert ist

```lua
function new_game()
	if WarriorsLib then
		dbg.stm("WarriorsLib has been found")
	else
		dbg.stm("WarriorsLib is not installed")
	end
end
```
