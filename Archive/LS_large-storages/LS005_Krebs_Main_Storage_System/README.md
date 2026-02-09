# Krebs’ Main Storage System
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Krebs*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1461831633719267508)

A highly efficient, fully locked storage system with advanced features including chest halls, bulk storage, unstackable sorting, parallel unloading, peripherals, and comprehensive status monitoring. Designed for high-capacity item management with low MSPT usage.
## Features
- 98% hopper locking
- 1mspt idle, 5mspt active (i5-9300h with lithium 1.17.1)
- 544 chest hall items, two double chest capacity per item (~7k items)
- 90 bulk items, 1.5 million capacity per item
- 10 multi item categories
- Unstackable sorter
- Parallel unloader, which allows for sorting items in parallel
- Some chest hall items have a assigned bulk slice for when they overflow
- Multiple peripherals (furnace array, crafting station, nano farms, etc.)
- Full system status output panel
- Basic error checking, which can pause the input if there is a problem
## Considerations
- Originally designed to fit Ingenium SMP’s needs, so you may need to change the item layouts
- Requires manual refilling of storage chest with stacked boxes for empty box distribution
- Only 8 slices of the set-based parallel unloader array used to limit client lag
- Additional red locking lines on chest halls are optional and need position adjustment
- No direct bulk input to limit user error (can be extended if needed)
- Unstackable sorter despawns water buckets in 1.19.3+
- Wooden decoration requires lightning protection to prevent fires
## Notes
All inventories that need to be filled (aside from empty box distribution) are marked with signs. Align the black/yellow square above the status panel to a single chunk unless repositioning chunkloaders manually. Nether side schematic attached for reference.
## Compatibility
Optimized for 1.17.1. For 1.16: replace 2 dispensers with powdered snow with waterlogged blocks and add pressure plate before rail to hopper. Issues in 1.19.3+ with unstackable sorter water buckets.
## Instructions
1. Align black/yellow square above status panel to single chunk (reposition chunkloaders if needed)
2. Manually refill storage chest with stacked boxes for empty box distribution
3. Adjust item layouts for your specific needs
4. Optional: Add/adjust red locking lines on chest hall outsides for full hopper locking
5. Use signs to identify inventories needing filling
## Credits
- Set-based parallel unloader array 2.4 – 8 slices, SS3 full version (*TheGlotzerify, Raffq, RaPsCaLLioN1138, Boyenn*)
- Fully locked input system, chest halls – 2 doublechest per item, and bulk – 1.5mil per item (*Krebs*)
- MIS 4.2 (*DatNerd et al.*)
- Unstackable sorter (CommandLeo) with accessible box loaders (vktec/squirl)
- Full clearance 6x mixed box loaders for overflow (*CommandLeo*)
- Precision 1x box loaders for bulk items (*CommandLeo & Walter*)
- Chunkloaders (*Kahyxen*)
- Crafting station (*acaciachan*)
- Long-duration pulse extender (*ilmango*)
- Pufferfish player detector (*Methodzz*)
- Overflow protection, automatic startup/shutdown with additional manual switch, full system status panel, automatic pausing/emergency stop (*Krebs*)
- Fully locked empty box distribution system. Requires manual refilling of storage chest with stacked boxes (*Krebs*)
- Fully locked 64-furnace array and miscellaneous peripherals (*Krebs*)
- Decoration (*Krebs and KingMoshe*)
- Additional locking for the MIS, unstackable sorter, and mixed box loaders (*Krebs*)

## Resources
- [LS005_Krebs_Main_Storage_System_Nether_Chunkloaders.litematic](attachments/LS005_Krebs_Main_Storage_System_Nether_Chunkloaders.litematic): MC 1.17.1, Size 21x9x21 blocks
- [LS005_Krebs_Main_Storage_System.litematic](attachments/LS005_Krebs_Main_Storage_System.litematic): MC 1.17.1, Size 114x101x109 blocks
- [LS005_Krebs_Main_Storage_System.zip](attachments/LS005_Krebs_Main_Storage_System.zip): MC 1.17.1
- [LS005_Krebs_Main_Storage_System_-_Inventories.zip](attachments/LS005_Krebs_Main_Storage_System_-_Inventories.zip): MC 1.17.1
