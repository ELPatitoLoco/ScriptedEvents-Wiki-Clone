The `RESETLIGHTCOLOR` action grants control over facility lights.

## Usage
```
RESETLIGHTCOLOR <ROOMS>
```
Resets the light color of the given rooms.

## Arguments
### Rooms
The rooms to reset the light color of. Valid inputs include:
- `*` or `ALL` for every room.
- The ID of the room (eg. "Hcz049"). Full list of IDs available [here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.RoomType.html).
- A zone name to affect an entire zone: `LightContainment`, `HeavyContainment`, or `EntranceZone`.