The `LIGHTSOFF` action grants control over facility lights.

## Usage
```
LIGHTSOFF <ROOMS> <DURATION>
```
Turns the lights off for the provided amount of seconds.

## Arguments
### Rooms
The rooms to turn the lights off in. Valid inputs include:
- `*` or `ALL` for every room.
- The ID of the room (eg. "Hcz049"). Full list of IDs available [here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.RoomType.html).
- A zone name to affect an entire zone: `LightContainment`, `HeavyContainment`, or `EntranceZone`.

### Duration
The duration to apply before turning the lights back on. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.