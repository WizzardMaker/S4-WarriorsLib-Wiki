# WarriorsLib.SelectWarriors

## `WarriorsLib.SelectWarriors(x, y, r, party, settlertype)`

Selects all entities of type (e.g. Settlers.SWORDSMAN\_01) of a around a circle with the center of / and radius

#### Rückgabewert

Returns an index with a reference to the selection. Can be **nil** if no soldiers found

#### Beispiel

```lua
militaryUnits = {Settlers.SWORDSMAN_01,Settlers.SWORDSMAN_02,Settlers.SWORDSMAN_03,Settlers.BOWMAN_01,Settlers.BOWMAN_02,Settlers.BOWMAN_03,Settlers.AXEWARRIOR_01,Settlers.AXEWARRIOR_02,Settlers.AXEWARRIOR_03,Settlers.BLOWGUNWARRIOR_01,Settlers.BLOWGUNWARRIOR_02,Settlers.BLOWGUNWARRIOR_03,Settlers.BACKPACKCATAPULTIST_01,Settlers.BACKPACKCATAPULTIST_02,Settlers.BACKPACKCATAPULTIST_03,Settlers.MEDIC_01,Settlers.MEDIC_02,Settlers.MEDIC_03,Settlers.SQUADLEADER}
function sendAllSoldierstoPoint(fromX, fromY, id, targetX, targetY, radius, move)
	local move = move or WarriorLib.MOVE_FORWARD
	local radius = radius or 15
	local i, settlertype = next(militaryUnits,nil)
	while i do
		warriors = WarriorLib.SelectWarriors(fromX, fromY, radius, id, settlertype)
		if warriors ~= nil then
			WarriorLib.Send(warriors, targetX, targetY, move)
		end
		i, settlertype = next(militaryUnits, i)
	end
end
```
