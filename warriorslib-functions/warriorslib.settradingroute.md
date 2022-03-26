# WarriorsLib.SetTradingRoute

## `WarriorsLib.SetTradingRoute(sourceBuildingID, destinationBuildingID, player)`

Set the target market/harbor of a market/harbor to establish a trading route.

#### return value

none

```lua
b1 = Buildings.GetFirstBuilding(1, Buildings.MARKETPLACE)
b2 = Buildings.GetFirstBuilding(3, Buildings.MARKETPLACE)
WarriorsLib.SetTradingRoute(b2, b1, 3)
WarriorsLib.TradeGood(b2, Goods.GOLDBAR, 100, 3)
```
