**New Feature in Scripted Events V2.0.0**
***
The `HELP` action allows for reading plugin documentation in a script.

## Usage
```
HELP <ACTION NAME/LIST> <FILE?>
```
Returns documentation for the given action or variable. Provide `LIST` to get a list of every available action, or `LISTVAR` to list every variable.

## Arguments
### Action Name / List / Variable / Variable List
The action to view information of, the variable to view information of, `LIST` to list every action, `LISTVAR` to list every variable.

### FILE?
If "FILE" is provided after the mode, and the executor is the server console, the help menu will be opened in a file. Eg. `HELP LISTVAR FILE` will show every variable in a file. The file will be located in the configs folder, and will be auto-deleted after 5 minutes (assuming the server console isn't closed/stopped).