# 16gt Parallelized Cart MIS Storage
<img alt="render.png" src="images/render.png?raw=1" height="300px">

**Authors:** *Wes*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1477856882214310001)

A small but powerful multi-item sorting storage system with up to 32x hopperspeed parallelization using hoppercarts.
## Features
- 32x HS parallel (16gt/full stack)
- 32x HS box unloader
- 1 wide tileable slice
- Sorts up to 50 items per slice, 32 slices on each side. (up to 3200 item types)
- Filter chests accessible
- All in one item entity input: dump entire inventory regardless of what it is (64, 16, and unstackable items, mixed boxes, bulk boxes).
- Multi-item box sorting: Full boxes are input into slice without unloading
- Full boxes with unstackable item get sorted to unstackables slice.
- Overflow protection
## Considerations
- Noisy
- Chunkloader not included
- Sometimes items will go in topmost chest in slices even when theres space below.
## Notes
Chunkloader excluded in schem but redstone connection for one included. Recommended to build it deep below storage to prevent linking troubles. Lever present to ignore box sorting capability and unload all boxes regardless of fill level. Note that you can use any set of unique items for the in-slice code items.
## Compatibility
1.21.10+, broken in older 1.21 versions because of bubble column changes. Tested in 1.21.10-1.21.11
## Instructions
1. **To build:** build the schematic using Litematica, make sure to fill inventories accordingly. Press "I" on container to see inventories. https://modrinth.com/mod/techutils highly recommended to verify. Inventories filled in the storage:
    - 2x double chest and a chain of hoppers at unloader containing __hopper minecarts__
    - 11x hoppers containing __6 different unique renamed blockers__
    - 1x dropper containing __shears (unstackables)__
    - 1x dispenser containing __water bucket__
    - 64x hopper (for each slice) and 1x dropper containing __65x different random item stacks__. Any set of random items can be used, be it renamed or not, as long as they are all different.
    - 64x accessible filter chests (for each slice) configured with __renamed blockers__ for non-CUD version.
  Clear items from inventories that should be empty.
2. Build chunkloader(s), loading the whole storage system. Recommended to build deep below storage. Redstone connection for chunkloader is included in storage system.
3. Add light sources around the storage system to make sure no mobs or animals can spawn closely.
4. **To use:** Set up MIS filter chests below the trapdoors with the categories you want. You can only change these anytime the storage isn't running. Burn the blockers you don't use. _Make sure to never add the same item to multiple slices._
5. Make sure that no rail in the back is broken by piston from setting categories, and those rail pistons are in __down__ position.
6. Dump items into the input (white stained glass column).

## Other Images
<img src="images/hallway.png?raw=1" height="300px">

<img src="images/Slice.png?raw=1" height="300px">

## Resources
- [MIS012_1.21.10_16gt_Cart_MIS_Storage_-_Categories_Included.litematic](attachments/MIS012_1.21.10_16gt_Cart_MIS_Storage_-_Categories_Included.litematic): MC 1.21.10, Size 19x14x45 blocks
- [MIS012_16gt-Cart-MIS-Storage-Categories.zip](attachments/MIS012_16gt-Cart-MIS-Storage-Categories.zip): discord
  - Contains JSON configuration for the item layout tool website
