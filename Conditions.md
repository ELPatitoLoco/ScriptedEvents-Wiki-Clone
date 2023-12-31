ScriptedEvents supports a wide range of condition operators, specifically in the [IF](https://github.com/Thundermaker300/ScriptedEvents/wiki/IF), [STOPIF](https://github.com/Thundermaker300/ScriptedEvents/wiki/STOPIF), and [WAITUNTIL](https://github.com/Thundermaker300/ScriptedEvents/wiki/WAITUNTIL) actions. These conditions allow for simple operations in order to yield or completely cancel a script if certain conditions are not met.

It is highly encouraged that these are used in combination with [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables).

## Conditions/Operators
* `>` - Compares two numerical sides and returns true if the left side is greater than the right side.
* `<` - Compares two numerical sides and returns true if the left side is less than the right side.
* `=` - Compares two numerical sides and returns true if they are equal in value.

## AND/OR
The keywords `AND` and `OR` can be used to join multiple conditions together into one single action (cases 6 - 10). By default, ANDs have higher priorities over ORs. However, parenthesis can be used to determine the order at which the operators are read (see cases 9 and 10 for examples of this).

## Examples
### Case 1
Wait until there are more than five players alive.
```
WAITUNTIL {PLAYERSALIVE} > 5
```

### Case 2
Wait every second for a 5% chance of something to happen. (Remember: `WAITUNTIL` blocks are recalculated every second).
```
WAITUNTIL {CHANCE} < 0.05
```

### Case 3
Stop the script after anywhere from 500-700 seconds if there are more than 20 dead players.
```
WAITSEC 500 + (200 * {CHANCE})
STOPIF {PLAYERSDEAD} > 20
```

### Case 4
Black out all the lights UNLESS there are exactly 15 players in the server.
```
STOPIF {PLAYERS} = 15
LIGHTSOFF 50
```

### Case 5
Decontaminate LCZ after 500 seconds if there are more than 20 players in the server.
```
WAITSEC 500
IF {PLAYERS} > 20
DECONTAMINATE
```

### Case 6
Flicker the lights for 10 seconds if all the players are alive, or there are exactly 5 players on the surface.
```
IF {SPECTATOR} = 0 OR {SURFACE} = 5
LIGHTSOFF 10
```

### Case 7
Flicker the lights off for 10 seconds if there are exactly 8 players alive, exactly 5 players dead, exactly 3 SCPs, and at least 3 MTF.
```
IF {PLAYERSALIVE} = 8 AND {PLAYERSDEAD} = 5 AND {SCPS} = 3 AND {MTF} >= 3
LIGHTSOFF 10
```

### Case 8
Activate the warhead after 1,500 seconds if there are more than 20 players in the server, AND all the players are dead.
```
WAITSEC 1500
IF {PLAYERS} > 20 AND {PLAYERS} = {SPECTATOR}
DECONTAMINATE
```

### Case 9
Decontaminate LCZ after 500 seconds if there are more than 20 players in the server, OR if all the Class-D & Scientists are dead.
```
WAITSEC 500
IF {PLAYERS} > 20 OR ({CLASSD} = 0 AND {SCIENTIST} = 0)
DECONTAMINATE
```

### Case 10
Activate the alpha warhead after 500 seconds if there are more than 20 players and No SCPs, or if there are only MTF left alive.
```
WAITSEC 500
IF ({PLAYERSALIVE} > 20 AND {SCPS} = 0) OR ({MTF} = {PLAYERSALIVE})
WARHEAD START
```