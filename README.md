> [!NOTE]
> You can read the original README for the OpenGOAL project [here](https://github.com/open-goal/jak-project/blob/master/README.md).

# OpenGOAL Random Cell Order

Jak 1 but you must collect Power Cells in some specific order, randomly determined when you start a new game! If you try to collect the incorrect cell, you won't be able to. Once you collect the specified cell, the next in the list is revealed. [Original idea and version](https://teamrun.web.app/rco) by SixRock and Dexz.

<img src="https://github.com/OpenGOAL-Mods/OG-RCO/assets/2515356/f6c5bbcf-627d-43af-9571-654042cf19f2" width="50%"/>

## Settings (preventing softlocks / required speedrun tech)

Some cell orderings would be impossible, like if the very first cell chosen was from Lava Tube. To avoid these cases, there are a handful of restrictions enforced when randomly choosing cells. Additionally, depending on which speedrun tricks you are comfortable with, you can toggle other restrictions on/off. (shoutout to Six & Dexz again for originally working out most of these)

Restrictions:
- Unless all 4 Geyser Rock cells have been chosen, cells outside Geyser Rock cannot be chosen (the first 4 cells are always from Geyser Rock)
- For each hub level, Oracle cell #2 cannot be chosen before Oracle cell #1
- Similarly, the Volcanic Crater miners' cells cannot be chosen out of order
- Unless Purple Rings cell has been chosen, Blue Rings cell cannot be chosen
- Unless Fish Game cell has been chosen, Misty Island cells cannot be chosen
- Unless End of Fire Canyon cell has been chosen, cells beyond Fire Canyon cannot be chosen
- Unless End of Mountain Pass cell has been chosen, cells beyond Mountain Pass cannot be chosen (see below, this is used to prevent Snowy gondola softlock)
- Unless End of Mountain Pass cell has been chosen, and 2 more cells have been chosen since then, Snowy Mountain cells cannot be chosen (the +2 cells check for gondola now counts from End of MP instead of on pressing the warp gate switch in Red Sage hut)
- Unless FlutFlut Egg or Yellow Eco Switch cell has been chosen, the frozen crate cell in Snowy cannot be chosen
- If any Forbidden Jungle cells have been chosen, the Mayor's 90 orbs cell cannot be chosen before his cell from Forbidden Jungle Mirrors
- If any Precursor Basin cells have been chosen, the Geologist's 90 orbs cell cannot be chosen before her cell for the Lightning Moles
- If any Precursor Basin cells have been chosen, the Gambler's 90 orbs cell cannot be chosen before his cell for Dead Man's Gorge

Toggle-able restrictions:
| Option | When On... | When Off... |
|-|-|-|
| **No early Forbidden Temple** | Unless Top of FJ Tower cell has been chosen, Blue Eco Switch and Plant Boss cells cannot be chosen | You may need to break into Temple via Idle Deload |
| **No early Plant Boss** | Unless Blue Eco Switch cell has been chosen, Plant Boss cell cannot be chosen | You may need to do the boosted -> infinite jump -> extended uppercut in Temple to get to Plant Boss early |
| **No early Beach Tower** | Unless Blue Eco Switch cell has been chosen, Sentinel Beach Cannon Tower cell cannot be chosen | You may need to do the Tower climb from below |
| **No Fire Canyon Skip** | Unless 20 cells have been chosen, cells from Fire Canyon (or beyond, by earlier restriction) cannot be chosen | You may need to do FCS |
| **No Boulder Skip** | Unless 45 cells have been chosen, cells from Mountain Pass (or beyond, by earlier restriction) cannot be chosen | You may need to do Boulder Skip |
| **No Klaww Skips** | Unless Klaww cell has been chosen, other cells from Mountain Pass (or beyond) cannot be chosen | You may need to do Lava Walk or Idle Deload past Klaww |
| **No early MP secret cell** | Unless Yellow Eco Switch cell has been chosen, Mountain Pass secret cell cannot be chosen | You may need to do "backwards cell" on-foot, or tree/rock/stalag hops |
| **No Tree/Rock/Stalag Hops** | Unless End of Mountain Pass cell has been chosen, Mountain Pass secret cell cannot be chosen (you may need to do "backwards cell" on-foot) | You may need to do tree/rock/stalag hops |
| **No Snowy Fort w/o FlutFlut** | Unless Sentinel Beach FlutFlut cell has been chosen, the Snowy Fort Gate cell cannot be chosen | You may need to get to the Fort Gate Switch without FlutFlut |
| **No Snowy Fort break-in** | Unless Snowy Fort Gate cell has been chosen, the cell inside Snowy Fort and Snowy Scout Flies cell cannot be chosen | You may need to break into the Fort on-foot or with FlutFlut (if available) |
| **No Lava Tube Skip** | Unless 72 cells have been chosen, cells from Lava Tube or beyond cannot be chosen | You may need to do LTS |
| **No Citadel Hops** | Unless End of Lava Tube has been chosen, cells in Citadel cannot be chosen | You may need to do Citadel Hops |
| **No Citadel Skip** | Unless Blue, Red, and Yellow Sage cells have been chosen, neither Green Sage nor Citadel Flies cells can be chosen | You may need to do Citadel Skip. If you don't get the top Scout Fly after doing Citadel Skip, you might also end up having to do "V2" to get back up |

You can toggle these from the in-game pause menu: `OPTIONS` > `GAME OPTIONS` > `RANDOM CELL ORDER SETTINGS`. Note that the cell order list is generated whenever you start a new game, so toggling these settings mid-game will have no effect.
