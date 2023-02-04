Scripted Events allows you to save variables. As an example, you can select and save one random player, and then use that player in multiple commands.

## Example
The following example pulls a random NTF from a respawn wave, turns them into a Chaos, and shows them a broadcast.
```
# Wait for an NTF respawn wave.
WAITUNTIL WAVERESPAWNING
STOPIF LASTRESPAWNTEAM = ChaosInsurgency

# Grab one random respawned player and save them as a variable, "INTRUDER".
SAVEPLAYERVARIABLE {INTRUDER} {RESPAWNEDPLAYERS} 1

# Turn them into a CI
SETROLE {INTRUDER} ChaosRepressor

# Show a broadcast
BROADCASTPLAYER {INTRUDER} 10 You're an NTF intruder. Go get 'em tiger!

# Delete the variable so it isn't accidentally re-used later on.
DELPLAYERVARIABLE {INTRUDER}
```