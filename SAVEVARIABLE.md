**Will be available in ScriptedEvents Version 1.1**
***
The `SAVEVARIABLE` action grants variable control in a script. See [Saving Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Saving-Variables) for more information.

## Usage
```
SAVEVARIABLE <VARIABLENAME> <VALUE>
```
Saves a new variable. The new variable will not be changed at all until it is re-defined or removed.

Note: It is encouraged to [delete the variable](https://github.com/Thundermaker300/ScriptedEvents/wiki/DELVARIABLE) after its usage is complete. 

## Arguments
### VariableName
The name of the new variable. Braces, if not provided, will be added automatically.

### Value
The contents to be stored as a variable. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here. If the value is a number/variable converted to a number, or a math equation, it will be stored as a number and can be used in number-related parameters of other actions.