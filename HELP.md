The `HELP` action allows for reading plugin documentation in a script.

## Usage
```
HELP <ACTION NAME/LIST> <NOFILE?>
```
Returns documentation for the given action or variable. Provide `LIST` to get a list of every available action, or `LISTVAR` to list every variable.

## Arguments
### Action Name / List / Variable / Variable List
The action to view information of, the variable to view information of, `LIST` to list every action, `LISTVAR` to list every variable.

### NOFILE?
By default, if the help command is executed in the server console, a file is generated to show the result. The file will be located in the configs folder, and will be auto-deleted after 5 minutes (assuming the server console isn't closed/stopped). If "NOFILE" is provided after the mode, a file will not be generated, and the result will be shown in the server console instead.