The `SPAWNRULE` action grants player control in a script.

## Usage
```
SPAWNRULE <ROLETYPE> [MAX]
```
**Must be used before the start of the round.** Overrides the default spawning mechanic by setting a certain amount of players as the given role at the start of the round.

## Arguments
### Role Type
The role that will be spawned.

### Max
The maximum amount of players that can be spawned as this role. **If this value is not provided**, every player that does not spawn as a different spawn rule will spawn as this rule, completely overwriting base-game spawning logic. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.

## Examples
### Case 1: Peanut Infection
```
# Spawn one SCP-173, make everyone else Class-D
SPAWNRULE Scp173 1
SPAWNRULE ClassD

# Set up infection - When a class-d dies, turn them into a peanut and move them to their death location.
INFECTRULE ClassD Scp173 TRUE
```

### Case 2: MTF vs CI
```
# Spawn half of players as MTF and half as CI
# This works by diving the amount of players by half and setting the first half to NtfSergeant.
# The remainder are set to ChaosRepressor.
# Note: There should be a delay between the server finishing the restart and running this script. Otherwise there's going to be A LOT of Chaos and very little NTF.
SPAWNRULE NtfSergeant {PLAYERS}/2
SPAWNRULE ChaosRepressor

# Optional bonus: On death, convert to the opposite team
INFECTRULE NtfSergeant ChaosRepressor FALSE
INFECTRULE ChaosRepressor NtfSergeant FALSE
```