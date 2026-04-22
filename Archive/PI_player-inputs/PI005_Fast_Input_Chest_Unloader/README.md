# Fast Input Chest Unloader
<img alt="Wall_UI.png" src="images/Wall_UI.png?raw=1" height="300px">

**Authors:** *Christone*

**Endorsed by:** *Christone*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1496373746594873515)

Simply unloads a double chest as fast as it can using hopper carts. No extra sorting features. Designed to be an input to a storage system where a player can simply put everything into one chest, whether items or boxes.
## Features
- Fast (about 30sec to unload a chest full of mixed items)
- Waits for user to close chest before unloading, (opening the chest also pauses unloading)
- Reliable for all stupid player input cases I can think of (unlike the past 10 versions)
- Will yeet carts when chest is empty or ran out of carts
- Clean Wall UI (no redstone-type blocks around the input chest)
- Clean Floor UI (the top redstone and water streams can be neatly covered with carpet)
- Great for use in sorting systems that want a lot of entities in a pile (like cart-based MIS, Entity-based splitters, cart-based splitters, variable stack-separation systems, cart-based input parallelizers, or 'dolphin' respawn-based parallelization)
## Considerations
- no pre-sorting of unstackables or boxes included (unlike other input systems)
- no separate chest for bulk input
## Notes
It can store and recycle up to 73 carts, 41 included, more carts means it can unload more of the chest before needing to yeet and recycle the carts, so 73 is a little faster because it only yeets once, but it's diminishing returns, 22 is a good number if you want less carts.
## Compatibility
Works in versions 1.19+ due to cart yeeting
Works in versions 1.16+ with the DropFullCarts mod.

## Other Images
<img src="images/Floor_UI.png?raw=1" height="300px">

## Resources
- [PI005_Fast_Input_Chest_Unloader_Wall_UI.litematic](attachments/PI005_Fast_Input_Chest_Unloader_Wall_UI.litematic): MC 1.20.1, Size 3x8x9 blocks
- [PI005_Fast_Input_Chest_Unloader_Floor_UI.litematic](attachments/PI005_Fast_Input_Chest_Unloader_Floor_UI.litematic): MC 1.20.1, Size 3x9x9 blocks
