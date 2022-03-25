# Ist das Plugin geladen?

Beispiel um zu überprüfen innerhalb der new\_game() Funktion ob das WarriorLib Plugin vom Spieler installiert ist

```lua
function new_game()
	if WarriorLib then
		dbg.stm("WarriorLib has been found")
	else
		dbg.stm("WarriorLib is not installed")
	end
end
```
