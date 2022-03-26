# WarriorsLib.getPlayerName

## `WarriorsLib.getPlayerName(player)`

Gibt den Spielernamen des angegebenen Spielers zurück.

#### Rückgabewert

`Spielername`

```lua
dbg.stm(WarriorsLib.getPlayerName(1)..", you are ".. (WarriorsLib.isHuman(1) == 1 and "a Human" or "an AI"))
```
