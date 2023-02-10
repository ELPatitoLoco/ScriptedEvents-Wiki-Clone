Scripted Events allows you to save variables, or values to be used later. As an example, you can select and save one random player, and then use that player in multiple commands. Or you can store a number to use later.

By default, variables defined in one script can be used in any other script. If you are intending to create script-unique variables, it is encouraged to prefix the variable names. On the flip side, since variables can be read and written to from any script, it is possible to create a form of value system by accessing the same variable in multiple different scripts.

## Variable Actions
### Create
* [SAVEVARIABLE](https://github.com/Thundermaker300/ScriptedEvents/wiki/SAVEVARIABLE/) - Creates a variable.
* [SAVEPLAYERVARIABLE](https://github.com/Thundermaker300/ScriptedEvents/wiki/SAVEPLAYERVARIABLE/) - Creates a player variable by combining a pre-existing player variable and a maximum value (optional).

### Delete
* [DELVARIABLE](https://github.com/Thundermaker300/ScriptedEvents/wiki/DELVARIABLE/) - Deletes a previously defined variable.
* [DELPLAYERVARIABLE](https://github.com/Thundermaker300/ScriptedEvents/wiki/DELPLAYERVARIABLE/) - Deletes a previously defined player variable.

## Example
The following example pulls a random NTF from a respawn wave, turns them into a Chaos, and shows them a broadcast.
```
# Wait for an NTF respawn wave.
WAITUNTIL {WAVERESPAWNING}
STOPIF {LASTRESPAWNTEAM} = ChaosInsurgency

# Grab one random respawned player and save them as a variable, "INTRUDER".
SAVEPLAYERVARIABLE {INTRUDER} {RESPAWNEDPLAYERS} 1

# Turn them into a CI
SETROLE {INTRUDER} ChaosRepressor

# Show a broadcast
BROADCASTPLAYER {INTRUDER} 10 You're an NTF intruder. Go get 'em tiger!

# Delete the variable so it isn't accidentally re-used later on.
DELPLAYERVARIABLE {INTRUDER}
```