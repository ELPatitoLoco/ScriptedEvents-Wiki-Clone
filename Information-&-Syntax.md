## Automated Scripts
Scripts can be set to run automatically as soon as the round starts. This can be done by adding them to this list in the plugin's config.
```yml
auto_run_scripts: []
```

## Looped Scripts
Scripts can be set to repeat themselves automatically as soon as the script finishes. This can be done by adding them to this list in the plugin's config.
```yml
loop_scripts: []
```

## Per-script permissions
Scripts can be set-up with a per-script permission system, to only allow certain staff to execute certain events. This can be done in the plugin's configuration, by adding the following.
```yml
  required_permissions:
    ExampleScriptNameHere: examplepermission
```
Replace `ExampleScriptNameHere` with the name of the script, and `examplepermission` to the permission to use. The actual permission required will automatically become `script.execute.[whatever you put in the config]`.

## Comments
Lines that start with a hashtag (`#`) character will be ignored, allowing the use of comments.

## Disabling Scripts
Scripts can be disabled by adding `!-- DISABLE` to the beginning of the script. This will prevent the script from running automatically or being executed in a command.

### Uses
* Events that aren't finished that you don't want to be executed accidentally.
* Limited-time/seasonal events.