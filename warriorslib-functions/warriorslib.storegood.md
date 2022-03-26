# WarriorsLib.StoreGood

## `WarriorsLib.StoreGood(buildingID, goodtype, enable, player)`

Gibt an, welche Waren ein Lager lagern soll.

`enable`

Wenn TRUE, beginnt das Gebäude, Waren des angegebenen Typs zu lagern. Wenn FALSE, wird es aufhören, sie zu speichern.

#### Rückgabewert

none

```lua
Buildings.AddBuilding(118, 58, 3, Buildings.STORAGEAREA)
WarriorsLib.StoreGood (Buildings.GetFirstBuilding(3, Buildings.STORAGEAREA), Goods.GOLDBAR, 1, 3, 1)
```
