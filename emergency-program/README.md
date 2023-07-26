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
* The stonecutter at `26328 (3318) (54/51)` will be finished, but there is also a castle under construction at `12004 (1529) (57/23)`. If you connect the roads, so that the building can be resumed, no wood will be delievered (only stones).
* Additionaly, building new buildings is not possible anymore: new "small" buildings don't get a builder assigned, new "big" buildings don't even get a guy leveling the foundation. This is not a matter of missing building material. Fast forwarding to 3h, the game will pile up more than 100 wooden planks and more than 60 stone blocks.

## The problem

As I understand it, this should not happen. Furthermore, when the game goes into "emergency mode", buildings don't get finished anymore - even if there is enough building material (at least in my savegame). Also, building new buildungs is delayed and/or they newer get finished. (when is "Emergendy mode" ending?).

Maybe it has something to do the stock buildings somehow not beeing recognized? I also tried shifting stones and wooden planks from the northerly stock back to the castle, but it didnt work, too. Having more than 40 stones and wooden planks in the castle does not deactivate emergency mode nor finishes new buildings.

Seems like the issue is not unknown: http://www.mag64.de/index.php?page=nds/siedds/siedds&server=1&ext=1

> Wehe Ihr lest hier die Meldung "Das Notprogramm wurde aktiviert". Je nach Gutdünken des Spiels und damit reine Glückssache, kann es nämlich passieren das trotz kurz darauf fertigem Sägewerk das Notprogramm nicht deaktiviert wird und alle neuen Bretter direkt in das HQ wandern, anstatt zu den Baustellen.

## Workaround

Building (another) sawmill deactivated the emergency program and the game could be contiuned normally.

## My environment

* Win 10, 64
* Serflings 2.0.0 (with integrated JRE)
* Map: `RIVAL` (campaign mission #16)
* Original game file: `SPAE.PA`

## Thanks

Thank you, `nicymike`, for the awesome "Serfings Remake Project". I hope this can help finding / resolving bugs and make it an even better game.
