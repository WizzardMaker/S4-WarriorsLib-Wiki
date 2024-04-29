# WarriorsLib.SelectWarriors

## `WarriorsLib.SelectWarriors(x, y, r, party, settlertype)`

Wähle alle Einheiten eines Typs (z.B. Settlers.SWORDSMAN_01) innerhalb des angegebenen Radius von der angegebenen Spielerpartei

#### Rückgabewert

Gibt einen Index als Referenz für die selektierten Einheiten zurück. Wenn keine Einheiten gefunden werden, ist der Wert **nil**.&#x20;

#### Beispiel

```lua
militaryUnits = {Settlers.SWORDSMAN_01,Settlers.SWORDSMAN_02,Settlers.SWORDSMAN_03,Settlers.BOWMAN_01,Settlers.BOWMAN_02,Settlers.BOWMAN_03,Settlers.AXEWARRIOR_01,Settlers.AXEWARRIOR_02,Settlers.AXEWARRIOR_03,Settlers.BLOWGUNWARRIOR_01,Settlers.BLOWGUNWARRIOR_02,Settlers.BLOWGUNWARRIOR_03,Settlers.BACKPACKCATAPULTIST_01,Settlers.BACKPACKCATAPULTIST_02,Settlers.BACKPACKCATAPULTIST_03,Settlers.MEDIC_01,Settlers.MEDIC_02,Settlers.MEDIC_03,Settlers.SQUADLEADER}
function sendAllSoldierstoPoint(fromX, fromY, id, targetX, targetY, radius, move)
	local move = move or WarriorsLib.MOVE_FORWARDS
	local radius = radius or 15
	local i, settlertype = next(militaryUnits,nil)
	while i do
		warriors = WarriorsLib.SelectWarriors(fromX, fromY, radius, id, settlertype)
		if warriors ~= nil then
			WarriorsLib.Send(warriors, targetX, targetY, move)
		end
		i, settlertype = next(militaryUnits, i)
	end
end
```
