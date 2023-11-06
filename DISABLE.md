The `DISABLE` action grants round control in a script.

## Usage
```
DISABLE <KEY>
```
Disables a certain in-game feature for the duration of the round.

## Arguments
### Key
The Key argument determines what in-game feature is disabled.
* `DROPPING`: Disables dropping items.
* `DYING`: Disables dying.
* `ESCAPING`: Disables escaping.
* `ELEVATORS`: Disables all elevators.
* `GENERATORS`: Disables starting, stopping, and opening/unlocking generators.
* `HAZARDS`: Disables the effects of SCP-106 sinkholes and SCP-173 tantrums.
* `HURTING`: Disables taking any damage.
* `ITEMPICKUPS`: Disables picking up any items.
* `LOCKERS`: Disables opening/closing lockers/medkit stations.
* `MICROPIKUPS`: Disables picking up any Micro-HID.
* `NTFANNOUNCEMENT`: Disables the CASSIE NTF spawning announcement.
* `PEDESTALS`: Disables opening/closing SCP pedestals.
* `RESPAWNS`: Disables NTF + CI respawns.
* `SCP330`: Disables picking up candy from SCP-330.
* `SCP914`: Disables operating or upgrading in SCP-914.
* `SHOOTING`: Disables damage/bullets from shooting.
* `TESLAS`: Disables tesla gates.
* `WARHEAD`: Disables the warhead from being activated.
* `WORKSTATIONS`: Disables the workstations from being used.

### SCP Ability Keys
Beginning in Version 2.5.0, the following keys can be used to disable SCP related actions.
#### SCP-049
* `SCP049SENSE`
* `SCP049ATTACK`
* `SCP049RECALL`
* `SCP049CALL`
#### SCP-049-2
* `SCP0492ATTACK`
* `SCP0492BLOODLUST`
* `SCP0492CONSUMECORPSE`
#### SCP-079
* `SCP079CHANGECAMERA` - Disabled until Exiled issue is fixed
* `SCP079SPEAKER`
* `SCP079ELEVATOR`
* `SCP079GAINEXPERIENCE` - Disabled for now as this breaks SCP-079
* `SCP079GAINLEVEL` - Disabled for now as this breaks SCP-079
* `SCP079TESLA`
* `SCP079LOCKDOWN`
* `SCP079PING`
* `SCP079BLACKOUT`
* `SCP079DOOR`
* `SCP079ZONEBLACKOUT`
#### SCP-096
* `SCP096ADDTARGET`
* `SCP096ATTACK`
* `SCP096CHARGE`
* `SCP096ENRAGE`
* `SCP096TRYNOTCRY`
#### SCP-106
* `SCP106ATTACK`
* `SCP106ATLAS`
* `SCP106STALK`
#### SCP-173
* `SCP173ATTACK`
* `SCP173BLINK`
* `SCP173BREAKNECKSPEED` - Doesn't work at the moment
* `SCP173TANTRUM`
#### SCP-939
* `SCP939ATTACK`
* `SCP939CLOUD`
* `SCP939FOCUS`
* `SCP939PLAYSOUND`
* `SCP939PLAYVOICE`
* `SCP939SAVEVOICE`
#### SCP-3114
* `SCP3114ATTACK`
* `SCP3114DISGUISE` - Broken due to an Exiled bug
