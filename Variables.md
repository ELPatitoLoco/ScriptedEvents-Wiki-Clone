The following is a list of all variables supported in various ScriptedEvents places. All of the numerical variables can be used in the place of numbers in math equations (such as the `LIGHTSOFF` duration parameter).

Variables can be paired with [conditions](https://github.com/Thundermaker300/ScriptedEvents/wiki/Conditions) very well; however, they can also be used in standalone math equations.

## Variables
### Numerical variables
#### Chance
* `CHANCE` - A random value between `0` and `1`.

#### World Time
* `DAYOFMONTH` - Current day of the month (1-31).
* `DAYOFWEEK` - Current day of the week (1-7).
* `DAYOFYEAR` - Current day of the year (1-366).
* `MONTH` - Current month. (1-12).
* `YEAR` - Current year. (1-9999).

#### Role Count
* `CDP` - Total amount of alive Class-D Personnel.
* `CHI` - Total amount of alive Chaos Insurgency.
* `MTF` - Total amount of alive MTF + Guards.
* `RSC` - Total amount of alive Scientists.
* `SCPS` - Total amount of alive SCPs.

#### Player Count
* `PLAYERS` - Total amount of players.
* `PLAYERSALIVE` - The amount of players currently alive.
* `PLAYERSDEAD` - The amount of players currently dead.

#### Round Time
* `ROUNDMINUTES` - Length of round in minutes.
* `ROUNDSECONDS` - Length of round in seconds.

#### Tickets
* `NTFTICKETS` - NTF spawn tickets.
* `CHAOSTICKETS` - NTF spawn tickets.

### Boolean variables
Each variable below supports adding an `!` before it, which flips the check (Eg. `!CASSIESPEAKING` will return True if cassie is *not* speaking).
* `CASSIESPEAKING` - True if CASSIE is currently speaking.
* `DECONTAMINATED` - True if LCZ is decontaminated.
* `ROUNDENDED` - True if the round has ended.
* `ROUNDINPROGRESS` - True if the round is currently in progress.
* `ROUNDSTARTED` - True if the round has started.
* `SCP914ACTIVE` - True if SCP-914 is active.
* `WARHEADCOUNTING` - True if the warhead is currently counting down.
* `WARHEADDETONATED` - True if the warhead has detonated.