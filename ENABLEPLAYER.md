The `ENABLEPLAYER` action grants player interaction round control in a script.

## Usage
```
ENABLEPLAYER <PLAYERS> <KEY>
```
Enables a certain in-game feature for selected players unitl the round ended. (Can be later disabled by DISABLEPLAYER action)

## Arguments
### Players
The players to enable a certain key.
### Key
The Key argument determines what in-game feature is disabled.
* `DROPPING`: Enables dropping items for selected players.
* `DYING`: Enables dying for selected players.
* `ESCAPING`: Enables escaping for selected players.
* `ELEVATORS`: Enables all elevators interaction for selected players.
* `GENERATORS`: Enables starting, stopping, and opening/unlocking generators for selected players.
* `HAZARDS`: Enables the effects of SCP-106 sinkholes and SCP-173 tantrums for selected players.
* `HURTING`: Enables taking any damage for selected players.
* `ITEMPICKUPS`: Enables picking up any items for selected players.
* `LOCKERS`: Enables opening/closing lockers/medkit stations for selected players.
* `MICROPIKUPS`: Enables picking up any Micro-HID for selected players.
* `PEDESTALS`: Enables opening/closing SCP pedestals for selected players.
* `SCP330`: Enables picking up candy from SCP-330 for selected players.
* `SCP914`: Enables operating or upgrading in SCP-914 for selected players.
* `SHOOTING`: Enables damage/bullets from shooting for selected players.
* `TESLAS`: Enables tesla gates for selected players.
* `WARHEAD`: Enables activatetion of warhead for certain players.
* `WORKSTATIONS`: Enables the workstations from being used for selected players.