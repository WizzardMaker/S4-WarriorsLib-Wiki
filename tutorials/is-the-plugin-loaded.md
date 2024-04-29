# Ist das Plugin geladen?

Beispiel um zu überprüfen innerhalb der new_game() Funktion ob das WarriorLib Plugin vom Spieler installiert ist

```lua
function new_game()
	if WarriorsLib then
		dbg.stm("WarriorsLib has been found")
	else
		dbg.stm("WarriorsLib is not installed")
	end
end
```



So ermittelt ihr die aktuelle Version der WarriorsLib (erst verfügbar ab V1.3):

```lua
function new_game()
	if WarriorsLib then
		if WarriorsLib.VERSION then
			dbg.stm("WarriorsLib has been found in V".WarriorsLib.VERSION)
		else
			dbg.stm("WarriorsLib has been found - your Version is old, please consider to update your Plugin")
		end
	else
		dbg.stm("WarriorsLib is not installed")
	end
end
```

`WarriorsLib.VERSION` - Gibt die aktuelle vollständige Version an (Beispiel: 1.4.0)
`WarriorsLib.MAJOR_VERSION` - Gibt die aktuelle Hauptversion an (Beispiel: 1)
`WarriorsLib.MINOR_VERSION` - Gibt die aktuelle Nebenversion an (Beispiel: 4)
`WarriorsLib.AUTHOR` - Gibt die aktuellen Author(en) an
