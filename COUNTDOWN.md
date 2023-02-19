The `COUNTDOWN` action grants broadcast control in a script.

## Usage
```
COUNTDOWN <PLAYERS> <DURATION> [TEXT]
```
Creates a new countdown on the players screens with the given duration. Countdowns will override any other broadcasts.

## Arguments

### Players
The players to show the countdown to.

### Duration
The duration of the countdown. Note that math _cannot_ be used for this property. A single number must be provided.

### Text
The broadcast to show. [Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here. Default: "Countdown"