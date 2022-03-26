# WarriorsLib.isHuman

## `WarriorsLib.isHuman(player)`

Indicates whether the player is controlled by a human

#### return value

boolean (0 or 1)

```lua
dbg.stm(WarriorsLib.getPlayerName(1)..", you are ".. (WarriorsLib.isHuman(1) == 1 and "a Human" or "an AI"))
```
