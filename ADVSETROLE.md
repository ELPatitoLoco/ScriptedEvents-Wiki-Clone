The `ADVSETROLE` action grants player control in a script.

## Usage
```
Usage: ADVSETROLE <PLAYERS> <ROLE> [SPAWNPOINT] [INVENTORY] [MAX]
```
Sets the targeted players' role to the given role. Set TRUE or FALSE if player should spawn on spawnpoint position. Provide a max to limit the amount of players to change roles (randomly).

## Arguments
### PLAYERS
The players to change the roles of. [Player variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables#player-variables) can be used here.

### ROLETYPE
The role type to set. Valid RoleTypes can be found in the Exiled resources channel.

### Spawnpoint
When you spawn as role you can determine if it spawns at the spawnpoint (TRUE) or where it was before (FALSE).

### Inventory
When you spawn as role you can determine if it spawns with default inventory (TRUE) or without default inventory (FALSE).

### MAX
The maximum amount of players set the role of. Selected randomly. Math and [variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.