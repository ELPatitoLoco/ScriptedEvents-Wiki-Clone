The `COMMAND` action enables running admin commands.

## Usage
```
COMMAND <COMMAND>
```
Runs the admin command as the server (all permissions). Remote Admin commands must be prefixed with a `/`.

**[IMPORTANT]** Be mindful that the server has all permissions, and is able to execute any command successfully. Ensure that you lock actions that run sensitive commands behind custom permissions in the configuration file.

## Arguments
### Command
The command to execute.