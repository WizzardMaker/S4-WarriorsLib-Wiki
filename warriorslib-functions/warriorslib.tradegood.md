# WarriorsLib.TradeGood

## `WarriorsLib.TradeGood(buildingID, goodtype, amount, player)`

Specifies what goods and how many a market or harbor shall transport. Use [WarriorsLib.SetTradingRoute](warriorslib.settradingroute.md) to establish the destination building for the trade.

#### return value

none

```lua
b1 = Buildings.GetFirstBuilding(1, Buildings.MARKETPLACE)
b2 = Buildings.GetFirstBuilding(3, Buildings.MARKETPLACE)
WarriorsLib.SetTradingRoute(b2, b1, 3)
WarriorsLib.TradeGood(b2, Goods.GOLDBAR, 100, 3)
```
