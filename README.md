# OpenGOAL Random Cell Order

Jak 1 but you must collect Power Cells in some specific order, randomly determined when you start a new game! Once you collect the specified cell, the next in the list is revealed. [Original idea and version](https://teamrun.web.app/rco) by SixRock and Dexz.

![image](https://github.com/OpenGOAL-Mods/OG-RCO/assets/2515356/f6c5bbcf-627d-43af-9571-654042cf19f2)

## Settings (preventing softlocks / required speedrun tech)

Some cell orderings would be impossible, like if the very first cell chosen was from Lava Tube. To avoid these cases, there are a handful of restrictions enforced when randomly choosing cells. Additionally, depending on which speedrun tricks you are comfortable with, you can toggle other restrictions on/off. (shoutout to Six & Dexz again for originally working out most of these)

Restrictions:
- Unless all 4 Geyser Rock cells have been chosen, cells outside Geyser Rock cannot be chosen (the first 4 cells are always from Geyser Rock)
- For each hub level, Oracle cell #2 cannot be chosen before Oracle cell #1
- Similarly, the Volcanic Crater miners' cells cannot be chosen out of order
- Unless Purple Rings cell has been chosen, Blue Rings cell cannot be chosen
- Unless Fish Game cell has been chosen, Misty Island cells cannot be chosen
- Unless End of Fire Canyon cell has been chosen, cells beyond Fire Canyon cannot be chosen
- Unless End of Mountain Pass cell has been chosen, cells beyond Mountain Pass cannot be chosen
- Unless End of Mountain Pass cell has been chosen, and 2 more cells have been chosen since then, Snowy Mountain cells cannot be chosen
- If any Forbidden Jungle cells have been chosen, the Mayor's 90 orbs cell cannot be chosen before his cell from Forbidden Jungle Mirrors
- If any Precursor Basin cells have been chosen, the Geologist's 90 orbs cell cannot be chosen before her cell for the Lightning Moles
- If any Precursor Basin cells have been chosen, the Gambler's 90 orbs cell cannot be chosen before his cell for Dead Man's Gorge

Toggle-able restrictions:
- **No early Forbidden Temple** - Unless Top of FJ Tower cell has been chosen, Blue Eco Switch and Plant Boss cells cannot be chosen
- **No early Plant Boss** - Unless Blue Eco Switch cell has been chosen, Plant Boss cell cannot be chosen
- **No early Beach Tower** - Unless Blue Eco Switch cell has been chosen, Sentinel Beach Cannon Tower cell cannot be chosen
- **No Fire Canyon Skip** - Unless 20 cells have been chosen, cells from Fire Canyon (or beyond, by earlier restriction) cannot be chosen
- **No early MP secret cell** - Unless Yellow Eco Switch cell has been chosen, Mountain Pass secret cell cannot be chosen
- **No Tree/Rock/Stalag Hops** - Unless End of Mountain Pass cell has been chosen, Mountain Pass secret cell cannot be chosen
- **No Snowy Fort w/o FlutFlut** - Unless Sentinel Beach FlutFlut cell has been chosen, the Snowy Fort Gate cell cannot be chosen
- **No Snowy Fort break-in** - Unless Snowy Fort Gate cell has been chosen, the cell inside Snowy Fort and Snowy Scout Flies cell cannot be chosen
- **No Lava Tube Skip** - Unless 72 cells have been chosen, cells from Lava Tube or beyond cannot be chosen
- **No Citadel Hops** - Unless End of Lava Tube has been chosen, cells in Citadel cannot be chosen
- **No Citadel Skip** - Unless Blue, Red, and Yellow Sage cells have been chosen, Green Sage cell cannot be chosen

You can toggle these from the in-game pause menu: `OPTIONS` > `GAME OPTIONS` > `RANDOM CELL ORDER SETTINGS`. Note that the cell order list is generated whenever you start a new game, so toggling these settings will have no effect mid-game.

## Known Bugs

- You aren't prevented from the instant-collect for Scout Flies cells while on Zoomer/FlutFlut
