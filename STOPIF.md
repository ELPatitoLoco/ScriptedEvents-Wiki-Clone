The `STOPIF` action grants logic control in a script.

## Usage
```
STOPIF <CONDITION>
```
Stops the script immediately if the provided condition is `true`. If the condition is `true`, any actions located after this action will not be executed and the script will be finished early. If the condition is `false`, this action is ignored and any actions after it will execute.

## Arguments
### Condition
The condition to check.