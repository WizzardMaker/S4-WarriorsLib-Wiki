# WarriorsLib.getPlayerName

## `WarriorsLib.getPlayerName(player)`

Return the PlayerName of the given Player.&#x20;

#### return value

name of player

```lua
dbg.stm(WarriorsLib.getPlayerName(1)..", you are ".. (WarriorsLib.isHuman(1) == 1 and "a Human" or "an AI"))
```
