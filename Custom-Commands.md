Custom Commands allow you to define scripts to run when a user runs a specific command.

The following is the required structure in the plugin's configs.
```
  commands:
  - name: 'Test'
    description: ""
    permission: ""
    type: PlayerConsole
    run:
    - 'Script1'
    - 'Script2'
    - 'Script3'
```

The parameters are as follows.
* `name` - The name of the command.
* `description` - A description of the command to show in base-game help messages.
* `permission` - The permission required to use the command. It will be formatted as: `script.command.<your input here>`. Leave blank for no permission.
* `type` - The type of command. Must be: `PlayerConsole`, `RemoteAdmin`, or `ServerConsole`.
* `run` - A list of scripts to run when the command is executed.