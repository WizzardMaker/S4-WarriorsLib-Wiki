# WarriorsLib.UnGarrisonWarriors

## `WarriorsLib.UnGarrisonWarriors(buldingid, column, bowman, player)`

Ungarrison a building. This makes a military building eject units.

`column`

The column of the unit to eject. Use 0 (zero) to eject the leftmost unit (in regards to the side panel of the selected building) . Use -1 to eject as much units as possible. This value is usually in the range -1..5.

`bowman`

If **TRUE** a bowman is ejected. Otherwise a swordman is ejected. This parameter is ignored if _column_ is -1.

#### return value

none

```lua
WarriorsLib.UnGarrisonWarriors(Buildings.GetFirstBuilding(1, Buildings.GUARDTOWERSMALL),-1,1,1)
```
