# WarriorsLib.StoreGood

## `WarriorsLib.StoreGood(buildingID, goodtype, enable, player)`

Specifies what goods a storagearea store.

`enable`

If **TRUE** the building will start to store goods of the specified type. If **FALSE** it will stop storing them.

#### return value

none

```lua
Buildings.AddBuilding(118, 58, 3, Buildings.STORAGEAREA)
WarriorsLib.StoreGood (Buildings.GetFirstBuilding(3, Buildings.STORAGEAREA), Goods.GOLDBAR, 1, 3, 1)
```
