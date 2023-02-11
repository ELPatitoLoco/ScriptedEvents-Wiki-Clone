**Will be available in ScriptedEvents Version 1.1**
***
The `TESLA` action grants control over the tesla gates.

## Usage
```
TESLA <MODE> <TARGET> [duration]
```
Executes a tesla gate action. Any modifications to tesla gates via this action are reverted at the end of the round.

## Arguments
### Mode
The MODE argument indicates what action to take place. Valid options are: `PLAYERS`, `ROLETYPE`, `DISABLE`.
* `PLAYERS`: Disables tesla gates for the specific player.
* `ROLETYPE`: Disables tesla gates for the specific role.
* `DISABLE`: Disables tesla gates entirely.
* `ENABLE`: Enables tesla gates entirely, if they were previously disabled by the DISABLE mode.

### Target
The target to affect. Based on the Mode parameter...
* `PLAYERS`: Target should be a valid player or list of players.
* `ROLETYPE`: Target should be a valid roletype (eg. ClassD, Scp173, etc).
* `DISABLE`: Target should not be provided.
* `ENABLE`: Target should not be provided.

## Duration
The amount of time until the mode is reversed.
* `PLAYERS`: Time until the tesla gates are re-enabled for the given players.
* `ROLETYPE`: Time until the tesla gates are re-enabled for the given RoleTypes.
* `DISABLE`: Time until the tesla gates are re-enabled.
* `ENABLE`: Time until the tesla gates are re-disabled.