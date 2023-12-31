The following is a list of all variables supported in various ScriptedEvents places. All of the numerical variables can be used in the place of numbers in math equations (such as the `LIGHTSOFF` duration parameter).

Variables must be surrounded with curly braces (eg. `{CHANCE}`) in order to work as expected.

Variables can be paired with [conditions](https://github.com/Thundermaker300/ScriptedEvents/wiki/Conditions) very well; however, they can also be used in standalone math equations.

Certain scripts may have special variables that are only available in certain cases. See [this page](https://github.com/Thundermaker300/ScriptedEvents/wiki/Per-Script-Variables) for more info.

## Variable Types
Standard variables are variables which hold a single value, such as a message, number, etc. Standard variables come in three flavors:
* Built-In Variables - Variables that are defined by the plugin. These variables cannot be changed/erased/etc, and hold a value that can regularly change. These variables can be used in any script.
* Per-Script Variables - Variables that are defined by the plugin, but only in special cases. These variables are only available in the script that they are defined for. These variables cannot be changed/erased/etc.
* Custom Variables - Variables defined by the server host, via a script with the `SAVE` action. Custom variables can be used in any script, even outside of the script they were defined in. Custom variables reset each round, and can be modified by using the `SAVE` action again to reset the value.

Some of these variables are also player variables. This means that they also consist of a list of players, and can be used in player-related actions that take a player variable, such as `SETROLE` and `SIZE`.

Custom player variables can be created through the `PLAYERVAR` action. The created variable also holds a value representing the amount of players in the variable, and as such can be used in actions like `BROADCAST` as well as player-related actions. These variables can also be used in any script.

## Built-In Variables Variables
### Numerical variables
#### Chance
* `CHANCE` - A random value between `0` and `1`.
* `CHANCE3` - A random whole number between `1` and `3`.
* `CHANCE5` - A random whole number between `1` and `5`.
* `CHANCE10` - A random whole number between `1` and `10`.
* `CHANCE20` - A random whole number between `1` and `20`.
* `CHANCE100` - A random whole number between `1` and `100`.

#### World Time
* `DAYOFMONTH` - Current day of the month (1-31).
* `DAYOFWEEK` - Current day of the week (1-7).
* `DAYOFYEAR` - Current day of the year (1-366).
* `MONTH` - Current month. (1-12).
* `YEAR` - Current year. (1-9999).
* `TICK` - Amount of seconds that have passed since Jan 1st, 1970 (epoch).

#### Zone
* Each individual RoomType can be used as a variable to count the amount of players in the room. [All RoomTypes here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.RoomType.html).
* `LCZ` - Every player in Light Containment Zone.
* `HCZ` - Every player in Heavy Containment Zone.
* `EZ` - Every player in Entrance Zone.
* `SURFACE` - Every player on the surface.
* `POCKET` - Every player in the pocket dimension.

#### Role Count
* Each individual RoleType can be used as a variable to count the amount of players alive. Eg, `{NTFCAPTAIN}` to count the amount of alive captains.
* `CI` - Total amount of alive Chaos Insurgency.
* `GUARDS` - Total amount of alive facility guards.
* `MTF` - Total amount of alive MTF, not including guards.
* `MTFANDGUARDS` - Total amount of alive MTF and guards.
* `SCPS` - Total amount of alive SCPs.
* `SH` - Total amount of alive Serpent's Hand (always 0 if the plugin is not installed).
* `UIU` - Total amount of alive Unusual Incidents Units (always 0 if the plugin is not installed).

#### Player Count
* `PLAYERS` - Total amount of players.
* `PLAYERSALIVE` - The amount of players currently alive.
* `PLAYERSDEAD` - The amount of players currently dead.

#### Kills and Deaths
* `KILLS` - Total amount of kills in the round.
* `SCPKILLS` - Total amount of SCP kills in the round.

#### Escapes
* `ESCAPES` - Total amount of escapes.
* `CLASSDESCAPES` - Total amount of Class-D escapes
* `SCIENTISTESCAPES` - Total amount of Scientist escapes.

#### Server Info
* `PORT` - The port of the server.
* `MAXPLAYERS` - The maximum amount of players on the server.

#### Round Time
* `ROUNDMINUTES` - Length of round in minutes.
* `ROUNDSECONDS` - Length of round in seconds.

#### Tickets & Respawns
* `NTFTICKETS` - NTF spawn tickets.
* `CHAOSTICKETS` - NTF spawn tickets.
* `RESPAWNEDPLAYERS` - Amount of players that were respawned. This variable will not function before the first respawn wave.
* `TIMESINCELASTWAVE` - Amount of time since the last respawn wave, in seconds. **If a respawn wave has not occurred yet, this value will be very large.**
* `TIMEUNTILNEXTWAVE` - Amount of time until the next respawn wave, in seconds.
* `TOTALWAVES` - Total amount of respawn waves.

### Boolean variables
Each variable below supports adding an `!` before it, which flips the check (Eg. `{!CASSIESPEAKING}` will return True if cassie is *not* speaking).
* `CASSIESPEAKING` - True if CASSIE is currently speaking.
* `DECONTAMINATED` - True if LCZ is decontaminated.
* `ROUNDENDED` - True if the round has ended.
* `ROUNDINPROGRESS` - True if the round is currently in progress.
* `ROUNDSTARTED` - True if the round has started.
* `SCP914ACTIVE` - True if SCP-914 is active.
* `WARHEADCOUNTING` - True if the warhead is currently counting down.
* `WARHEADDETONATED` - True if the warhead has detonated.
* `WAVERESPAWNING` - True if a wave just respawned recently (within 5 seconds).
* `HEAVILYMODDED` - True if the server is heavily modded.

### String variable
* `LASTRESPAWNTEAM` - The most-recently spawned team. This variable will not function before the first respawn wave.
* `LASTRESPAWNUNIT` - The unit name of the most-recently spawned team. This variable will not function before the first respawn wave.
* `NEXTWAVE` - The next wave that is going to spawn. Options: `None` (not determined), `ChaosInsurgency`, `NineTailedFox`.
* `IP`- The IP of the server.

### Player variables
These variables __CANNOT__ be used in normal commands, and can only be used in parameters that are expecting players (such as the first parameter of the `SETROLE` action).

#### Roles
* Each individual RoleType can be used as a variable to get each player in that role. Eg, `{NTFCAPTAIN}` to get each alive NTF captain.
* `CI` - Chaos Insurgency.
* `GUARDS` - Facility guards.
* `MTF` - MTF, not including guards.
* `MTFANDGUARDS` - MTF and guards.
* `SCPS` - SCPs.
* `SH` - Serpent's Hand (always 0 if the plugin is not installed).
* `UIU` - Unusual Incidents Units (always 0 if the plugin is not installed).

#### Zone
* Each individual RoomType can be used as a variable to get the players in the room. [All RoomTypes here](https://exiled-team.github.io/EXILED/api/Exiled.API.Enums.RoomType.html).
* `LCZ` - Every player in Light Containment Zone.
* `HCZ` - Every player in Heavy Containment Zone.
* `EZ` - Every player in Entrance Zone.
* `SURFACE` - Every player on the surface.
* `POCKET` - Every player in the pocket dimension.

#### Custom Variables
Custom player variables can be used in any command that takes a player or list of players. For more information, see [this wiki page](https://github.com/Thundermaker300/ScriptedEvents/wiki/Saving-Variables).

#### Miscellaneous
* `RESPAWNEDPLAYERS` - The players that respawned in the most recent spawn wave. This variable will not function before the first respawn wave.
* `SERVERSTAFF` - The players on the server with RemoteAdmin access.