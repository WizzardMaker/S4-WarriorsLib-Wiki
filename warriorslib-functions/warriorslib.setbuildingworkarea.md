# WarriorsLib.SetBuildingWorkarea

## `WarriorsLib.SetBuildingWorkarea(buildingID, x, y, player)`

Set the work area for a building. This is the same event that players can issue by clicking the target icon in the side panel of a selected building.

#### return value

none

```lua
WarriorsLib.SetBuildingWorkarea(Buildings.GetFirstBuilding(3, Buildings.BARRACKS),70, 33, 3)
WarriorsLib.RecruitWarriors(Buildings.GetFirstBuilding(3, Buildings.BARRACKS), Settlers.BOWMAN_03, 5, 3)
```
