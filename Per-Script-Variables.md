The following variables become available only under special cases.
* If the script is executed via the `script execute` command, the `{SENDER}` variable can be used to access the player that ran the script.
* If the script is executed via the `On` config, the following variables MAY be available (based on the event):
  * `{EVPLAYER}` (player variable) - If the event involves a player.
  * `{EVITEM}` (conditional variable) - If the event involves an item (gives the ItemType).