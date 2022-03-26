# WarriorsLib.SetTradingRoute

## `WarriorsLib.SetTradingRoute(sourceBuildingID, destinationBuildingID, player)`

Legen Sie den Zielmarkt/-hafen eines Marktes/Hafens fest, um eine Handelsroute einzurichten.

#### Rückgabewert

none

```lua
b1 = Buildings.GetFirstBuilding(1, Buildings.MARKETPLACE)
b2 = Buildings.GetFirstBuilding(3, Buildings.MARKETPLACE)
WarriorsLib.SetTradingRoute(b2, b1, 3)
WarriorsLib.TradeGood(b2, Goods.GOLDBAR, 100, 3)
```
