The `BROADCAST` action grants broadcast control in a script.

## Usage
```
BROADCAST <DURATION> <MESSAGE>
```
Adds a broadcast to the broadcast queue.

## Arguments
### Duration
The duration of the broadcast. Note that math _cannot_ be used for this property. A single number must be provided, <s>or a range can be provided (eg. _5-10_) for a random number of seconds within the range</s> Ranges are being removed in the next version of the plugin, please use a single number.

### Message
The broadcast to show. [Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here.