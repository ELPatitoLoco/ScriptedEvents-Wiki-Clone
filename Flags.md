Scripted Events employs the use of "Flags", which are single line-strings following `!--` that determine certain functionality of the script. Lines that start with a `!--` are skipped over when the script is running, but they are important as they change how the script works.

# Flags
## Admin Event
The `!-- ADMINEVENT` flag prevents the script from running automatically, requiring that it be executed via command only. Additionally, scripts with this flag can be used through the [CedMod Panel](https://github.com/CedModV2/CedMod) (Exiled version only). Courtesy of [@ced777ric](https://github.com/ced777ric) for enabling this compatibility.

## Disable
The `!-- DISABLE` flag disables the script entirely. Scripts with this flag can be read via the "script read" command, but they cannot be executed by any command or by configs.

## Debug
The `!-- DEBUG` flag enables debug logs for the script it is defined in.

## Help Reponse
The `!-- HELPRESPONSE` flag is added automatically to files generated via the `HELP <INPUT> FILE` action. This flag makes a file completely undetectable by the plugin.

## Suppress Warnings
The `!-- SUPPRESSWARNINGS` flag disables all non-fatal warnings from command execution.