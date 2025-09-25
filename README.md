# GL\_TGD\_Test\_Framing\_Game

A tiny farming game demo with simple loop: plow a tile -> plant a selected seed -> the crop progresses through timed growth stages -> harvest when ready -> sell for profit -> buy new fields. Tools (shovel / sickle) are physical pickups; equipping a tool gates which actions are allowed. 

\*\*Unity Version:\*\* 6000.2.2f1  

\*\*Packages:\*\* Visual Scripting (built-in), plus assets listed below.


## Quick Start

1. Clone the repository.
2. Open with Unity.
3. Open the scene: `Assets/Scenes/SampleScene`.
4. Play.


## Controls
- WASD — move
- 1 - Shovel, 2 - Sickle, 4 - Seeds, 5 - Cycle through seeds, 0 - None/Unequip tool
- E — interact (plow/plant/harvest/buy/sell/pick up)


## Features
- Tile lifecycle: Green → Plowed → Planted → Harvestable → Green (plowed auto-reverts on a cooldown)
- Crops growth: 4 stares; per-stage durations; `HarvestReady` flag on completion
- Tools: equips via hotkeys
- Seeds: seed cycling skips empty stacks; shops to buy seeds
- Inventory: `SeedStacks`, `ProduceStacks`, money; chest to sell produced crops
- Field progression: buy Field2/Field3 gates to unlock new seed stands
- HUD & prompts: money, equipped tool, current seed, and contextual prompts (`PromptShow/PromptClear`, `HUDRefresh`)
- Animation: chest open/close on Player proximity


## Data (Balance)
- Seed prices: `[9, 12, 14, 16, 18, 24]`
- Produce prices: `[15, 21, 26, 31, 36, 48]`
- Stage durations (s):
  - Carrot `[10,10,9,1]`, Broccoli `[15,15,14,1]`, Cauliflower `[20,20,19,1]`
  - Sunflower `[25,25,24,1]`, Corn `[30,30,29,1]`, Mushroom `[40,40,39,1]`
- Starting Money: `150`
- Field2 Price: `400`, Field3 Price: `2000`


## Assets Used

- GameDev Starter Kit – Farming (Free) - https://assetstore.unity.com/packages/3d/environments/gamedev-starter-kit-farming-free-edition-243035

- Character Pack: Free Animal People Sample - https://assetstore.unity.com/packages/3d/characters/humanoids/character-pack-free-animal-people-sample-204568

- Skybox Series Free - https://assetstore.unity.com/packages/2d/textures-materials/sky/skybox-series-free-103633


## Notes

- Gameplay is built with Visual Scripting.

- Graphs live in `Assets/Scripts/`.





