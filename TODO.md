- okay so the plan is for now make a unit skill, or a weapon idk:
    https://openxcom.org/forum/index.php/topic,7974.0.html
    - that sets a tag saying THIS UNIT FIRED THE TELEPORT
    - that spawns an invisible dummb unit
    - when that unit spawns, call battleunit.getposition on the firer from the tag, then position.setX/y/z, see if that moves the unit
    - also need to expose `_save->getTileEngine()->isPositionValidForUnit(newPos, unit)` that the debug warp command runs or you'll teleport onto water or whatever. or do you - can you spawn units onto water? I assume not.
- code the rest of the mod
