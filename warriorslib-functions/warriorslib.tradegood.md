# WarriorsLib.TradeGood

## `WarriorsLib.TradeGood(buildingID, goodtype, amount, player)`

Gibt an, welche Waren und wie viele ein Markt oder Hafen transportieren soll. Verwenden Sie [WarriorsLib.SetTradingRoute](warriorslib.settradingroute.md), um das Zielgebäude für den Handel festzulegen.

#### Rückgabewert

none

```lua
b1 = Buildings.GetFirstBuilding(1, Buildings.MARKETPLACE)
b2 = Buildings.GetFirstBuilding(3, Buildings.MARKETPLACE)
WarriorsLib.SetTradingRoute(b2, b1, 3)
WarriorsLib.TradeGood(b2, Goods.GOLDBAR, 100, 3)
```
