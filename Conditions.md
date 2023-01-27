ScriptedEvents supports a wide range of conditions & condition variables, specifically in the [STOPIF](https://github.com/Thundermaker300/ScriptedEvents/wiki/STOPIF) and [WAITUNTIL](https://github.com/Thundermaker300/ScriptedEvents/wiki/WAITUNTIL) actions. These conditions allow for simple operations in order to yield or completely cancel a script if certain conditions are not met.

## Conditions/Operators
* `>` - Compares two numerical sides and returns true if the left side is greater than the right side.
* `<` - Compares two numerical sides and returns true if the left side is less than the right side.
* `=` - Compares two numerical sides and returns true if they are equal in value.

## Variables
### Numerical variables
* `CHANCE` - A random value between `0` and `1`.
* `PLAYERSALIVE` - The amount of players currently alive.
* `PLAYERSDEAD` - The amount of players currently dead.

### Boolean variables
Each variable below supports adding an `!` before it, which flips the check (Eg. `!CASSIESPEAKING` will return True if cassie is *not* speaking).
* `CASSIESPEAKING` - True if CASSIE is currently speaking.
* `DECONTAMINATED` - True if LCZ is decontaminated.
* `ROUNDENDED` - True if the round has ended.
* `ROUNDINPROGRESS` - True if the round is currently in progress.
* `ROUNDSTARTED` - True if the round has started.
* `WARHEADDETONATED` - True if the warhead has detonated.