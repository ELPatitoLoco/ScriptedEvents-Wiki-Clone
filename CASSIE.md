The `CASSIE` action grants CASSIE control in a script.

## Usage
```
CASSIE <MESSAGE>
```
Adds a CASSIE message.

## Arguments
### Message
The message to announce. [Variables](https://github.com/Thundermaker300/ScriptedEvents/wiki/Variables) can be used here. Optionally, splitting the text by using a `|` will announce the first half of the text as a CASSIE message and use the second half as CASSIE's caption text. If the second half has no text, captions will be disabled. See samples below.

## Samples
### Case 1
Announce "Hello" with the caption of "Goodbye"
```
CASSIE Hello|Goodbye
```

### Case 2
Announce "Hello" with the caption of "Hello". No caption is needed in this sample, since by default the caption is equivalent to the text CASSIE speaks.
```
CASSIE Hello
```

### Case 3
Announce "Hello" with no caption.
```
CASSIE Hello|
```