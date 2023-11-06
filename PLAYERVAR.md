The `PLAYERVAR` action grants manipulation of player variables in a script. See [Saving Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Saving-Variables) for more information.

## Usage
```
PLAYERVAR <MODE> <VARIABLENAME> <PLAYERS> [MAX]
```
Allows manipulation of player variables.

## Arguments
### Mode
The action to perform SAVE or DELETE or ADD or REMOVE.

### VariableName
The name of the new variable. Braces, if not provided, will be added automatically.

### Players
The players. Not required if mode is 'DELETE', but required otherwise.

### Max
The maximum amount of players to include in the new variable. Selected randomly. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.