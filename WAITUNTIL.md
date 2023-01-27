The `WAITUNTIL` action grants timing control in a script.

## Usage
```
WAITUNTIL <CONDITION>
```
Yields the execution of actions after this action until the provided condition is `true`. The condition is re-evaluated once per second until it returns `true` or until the script execution is canceled.

## Arguments
### Condition
The condition to yield for.