The `SAVEPLAYERS` action grants variable control in a script. See [Saving Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Saving-Variables) for more information.

## Usage
```
SAVEPLAYERS <VARIABLENAME> <CURRENTVARIABLE> [MAX]
```
Saves a new player variable by using a current variable. The new variable will not be changed at all until it is re-defined or removed. An optional maximum can be provided to set the maximum amount of players, random.

Note: It is encouraged to [delete the variable](https://github.com/Thundermaker300/ScriptedEvents/wiki/DELPLAYERVARIABLE) after its usage is complete. 

## Arguments
### VariableName
The name of the new variable. Braces, if not provided, will be added automatically.

### Current Variable
The current variable to use as a starting point for getting the list of players.

### Max
The maximum amount of players to include in the new variable. Selected randomly. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.