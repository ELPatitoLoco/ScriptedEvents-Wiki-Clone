The `DISABLEPLAYER` action grants player interaction round control in a script.

## Usage
```
DISABLEPLAYER <PLAYERS> <KEY>
```
Disables a certain in-game feature for selected players unitl the round ended. (Can be later enblaed by ENABLEPLAYER action)

## Arguments
### Players
The players to disable a certain key.
### Key
The Key argument determines what in-game feature is disabled.
* `DROPPING`: Disables dropping items for selected players.
* `DYING`: Disables dying for selected players.
* `ESCAPING`: Disables escaping for selected players.
* `ELEVATORS`: Disables all elevators interaction for selected players.
* `GENERATORS`: Disables starting, stopping, and opening/unlocking generators for selected players.
* `HAZARDS`: Disables the effects of SCP-106 sinkholes and SCP-173 tantrums for selected players.
* `HURTING`: Disables taking any damage for selected players.
* `ITEMPICKUPS`: Disables picking up any items for selected players.
* `LOCKERS`: Disables opening/closing lockers/medkit stations for selected players.
* `MICROPIKUPS`: Disables picking up any Micro-HID for selected players.
* `PEDESTALS`: Disables opening/closing SCP pedestals for selected players.
* `SCP330`: Disables picking up candy from SCP-330 for selected players.
* `SCP914`: Disables operating or upgrading in SCP-914 for selected players.
* `SHOOTING`: Disables damage/bullets from shooting for selected players.
* `TESLAS`: Disables tesla gates for selected players.
* `WARHEAD`: Disables activatetion of warhead for certain players.
* `WORKSTATIONS`: Disables the workstations from being used for selected players.
