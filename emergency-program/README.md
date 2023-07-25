# Emergency program

In these savegames, the game goes into "Emergency program" mode.

I googled a bit and the "Emergency program" is triggered, when there is not enough building material left (the exact conditions are unclear to me).

However, in my game there is plenty of wooden boards and stone blocks in the warehouse above the castle left (located at position `30348 (3811) (35/59)`:

* 44 wooden boards
* 26 stone blocks

## How to reproduce

* Load savefile `SAVE1.DS` (in-game name `16.7.2-NEW`), which should be at game time `02h 04m 00s`.
* Build a stonecutter building at the existing flag at position `26328 (3318) (54/51)`
* Fast-forward a bit, i.e. with 64-speed
* In a few moments the message "Emergency program activated" will appear

## The problem

As I understand it, this should not happen. Furthermore, when the game goes into "emergency mode", buildings don't get finished anymore - even if there is enough building material (at least in my savegame). Also, building new buildungs is delayed and/or they newer get finished. (when is "Emergendy mode" ending?). It looks kind of "buggy" to me...

## My environment

* Win 10, 64
* Serflings 2.0.0 (with integrated JRE)
* Map: `RIVAL` (campaign mission #16)
* Original game file: `SPAE.PA`

## Thanks

Thank you, `nicymike`, for the awesome "Serfings Remake Project". I hope this can help finding / resolving bugs and make it an even better game.
