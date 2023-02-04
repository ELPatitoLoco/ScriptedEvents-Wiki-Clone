The `EXECUTESCRIPT` action grants the ability to execute a script from another script.

## Usage
```
EXECUTESCRIPT <SCRIPTNAME>
```
Executes the script with the given name.

## Arguments
### Script Name
The name of the script to execute.

## Examples
### Case 1: Hub Script
It is possible to have one script that executes other scripts.

```
# Prevent any event for the first 5 seconds of the round.
WAITSEC 5

EXECUTESCRIPT MyScript1
EXECUTESCRIPT MyScript2
EXECUTESCRIPT MyScript3
```

### Case 2: Optional Delay
Let's say by default, a "door malfunction" event has a delay before it. However, using this action, it's possible to make the delay "optional" for forcing a door malfunction, and required for automatic door malfunctioning.
```
# Script 1: All this script does is delay and chance checking. This is the script that is set to run automatically in plugin configs.
STOPIF {CHANCE10} < 5
WAITSEC 300 + (300 * {CHANCE})

# Execute the script that actually does the malfunction.
EXECUTESCRIPT DoorMalfunction
```