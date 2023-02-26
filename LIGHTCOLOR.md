The `LIGHTCOLOR` action grants control over facility lights.

## Usage
```
LIGHTCOLOR <ROOMS> <R> <G> <B>
```
Sets the light color of the given room(s).

## Arguments
### Rooms
The rooms to modify the light color of. Valid inputs include:
- `*` or `ALL` for every room.
- The ID of the room (eg. "Hcz049"). Full list of IDs available [here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.RoomType.html).
- A zone name to affect an entire zone: `LightContainment`, `HeavyContainment`, or `EntranceZone`.

### R
The R component of the room color.

### G
The G component of the room color.

### B
The B component of the room color.