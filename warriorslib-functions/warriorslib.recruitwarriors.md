# WarriorsLib.RecruitWarriors

## `WarriorsLib.RecruitWarriors(`buildingid, warriortype, amount, party`)`

Let a building start or stop recruiting settlers.

The amount of units that you want to queue for recruitment. This value is besides some exceptions additive. You can pass negative values to reduce the amount of units in the queue. The game does only use the following values.

| Value | Description                                                                 |
| ----- | --------------------------------------------------------------------------- |
| -5    | Subtract five unit from the queue.                                          |
| -1    | Subtract one unit from the queue.                                           |
| 0     | Clears the queue. This will stop the building from producing further units. |
| 1     | Add one unit to the queue.                                                  |
| 5     | Add five units to the queue.                                                |
| 100   | The game will interpret this as infinity and will never decrease the queue. |

#### return value

none

```lua
WarriorsLib.RecruitWarriors(Buildings.GetFirstBuilding(1, Buildings.BARRACKS), Settlers.BOWMAN_03, 5, 1)
```
