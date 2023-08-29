The `DOOR` action grants control over facility doors.

## Usage
```
DOOR <MODE> <DOORSELECTOR>
```
Locks, unlocks, open, closes, or destroys doors.

## Notes
* This command will always ignore SCP-079's doors.

## Arguments
### Mode
The MODE argument indicates what action to take place. Valid options are: `OPEN`, `CLOSE`, `LOCK`, `UNLOCK`, AND `DESTROY`.

### DoorSelector
The DOORSELECTOR argument takes the following options: `*` for every door, the name of a zone for zone specific doors (`LightContainment`, `HeavyContainment`, `Entrance`, `Surface`), the exact door type (eg. `Hcz096`), or the door name as shown in the RemoteAdmin panel (eg. "106_PRIMARY"). A full list of door types can be found [here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.DoorType.html).