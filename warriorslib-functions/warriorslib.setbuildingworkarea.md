# WarriorsLib.SetBuildingWorkarea

## `WarriorsLib.SetBuildingWorkarea(buildingID, x, y, player)`

Legen Sie den Arbeitsbereich für ein Gebäude fest. Dies ist das gleiche Ereignis, das Spieler auslösen können, indem sie auf das Zielsymbol in der Seitenleiste eines ausgewählten Gebäudes klicken.

#### Rückgabewert

none

```lua
WarriorsLib.SetBuildingWorkarea(Buildings.GetFirstBuilding(3, Buildings.BARRACKS),70, 33, 3)
WarriorsLib.RecruitWarriors(Buildings.GetFirstBuilding(3, Buildings.BARRACKS), Settlers.BOWMAN_03, 5, 3)
```
