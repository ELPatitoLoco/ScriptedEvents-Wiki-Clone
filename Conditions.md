ScriptedEvents supports a wide range of condition operators, specifically in the [IF](https://github.com/Thundermaker300/ScriptedEvents/wiki/IF), [STOPIF](https://github.com/Thundermaker300/ScriptedEvents/wiki/STOPIF), and [WAITUNTIL](https://github.com/Thundermaker300/ScriptedEvents/wiki/WAITUNTIL) actions. These conditions allow for simple operations in order to yield or completely cancel a script if certain conditions are not met.

It is highly encouraged that these are used in combination with [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables).

## Conditions/Operators
* `>` - Compares two numerical sides and returns true if the left side is greater than the right side.
* `<` - Compares two numerical sides and returns true if the left side is less than the right side.
* `=` - Compares two numerical sides and returns true if they are equal in value.

## AND/OR
The keywords `AND` and `OR` can be used to join multiple conditions together into one single action. ANDs are always calculated __after__ ORs (see cases 6 and 7 for examples).

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
Decontaminate LCZ after 500 seconds if there are more than 20 players in the server, OR if all the Class-D are dead.
```
WAITSEC 500
IF {PLAYERS} > 20 OR {CLASSD} = 0
DECONTAMINATE
```

### Case 7
Activate the alpha warhead after 500 seconds if there are more than 20 players and No SCPs, or if there are only MTF left alive.
```
WAITSEC 500
IF ({PLAYERSALIVE} > 20 AND {SCPS} = 0) OR ({MTF} = {PLAYERSALIVE})
WARHEAD START
```