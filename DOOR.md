The `DOOR` action grants control over facility doors.

## Usage
```
DOOR <MODE> <DOORSELECTOR> [DURATION]
```
Locks, unlocks, open, closes, or destroys doors. A duration can be provided to revert the action (minus destroying) after a certain amount of time, in seconds, has passed.

## Notes
* This command will always ignore SCP-079's doors.

## Arguments
### Mode
The MODE argument indicates what action to take place. Valid options are: `OPEN`, `CLOSE`, `LOCK`, `UNLOCK`, AND `DESTROY`.

### DoorSelector
The DOORSELECTOR argument takes the following options: `*` for every door, the name of a zone for zone specific doors (`LightContainment`, `HeavyContainment`, `Entrance`, `Surface`), the exact door type (eg. `Hcz096`), or the door name as shown in the RemoteAdmin panel (eg. "106_PRIMARY").

### Duration (optional)
The duration to apply before reverting the action. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.