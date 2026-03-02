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
- If you put in too many regular items (not boxes) into the input they may despawn. Unlikely to occur.
- Sometimes items will go in topmost chest in slices even when theres space below.
## Notes
Chunkloader excluded in schem but redstone connection for one included. Recommended to build it deep below storage to prevent linking troubles. Lever present to ignore box sorting capability and unload all boxes regardless of fill level. Nondirectional, nonlocational.
## Compatibility
1.21.10+, broken in older 1.21 versions because of bubble column changes. Tested in 1.21.10-1.21.11
## Instructions
1. Set up MIS filter chests below the trapdoors with the categories you want
2. Make sure that no rail in the back is broken by piston from setting categories
3. Dump items into the input (whit stained glass column)

## Other Images
<img src="images/hallway.png?raw=1" height="300px">

<img src="images/Slice.png?raw=1" height="300px">

## Resources
- [MIS012_1.21.10_16gt_Cart_MIS_Storage_-_Test_Categories_Included.litematic](attachments/MIS012_1.21.10_16gt_Cart_MIS_Storage_-_Test_Categories_Included.litematic): MC 1.21.10, Size 19x14x43 blocks
