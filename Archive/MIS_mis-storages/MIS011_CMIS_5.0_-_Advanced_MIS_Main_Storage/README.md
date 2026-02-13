# CMIS 5.0 - Advanced MIS Main Storage
<img alt="area_render_165_.png" src="images/area_render_165_.png?raw=1" height="300px">

**Authors:** *Civic Dude*

**Endorsed by:** *Andrews54757*

**Tags:** *Untested*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1469384785846599845)

CMIS 5.0 is a complete storage system designed for single player or small server use in Minecraft 1.21+, utilizing Variable Sorting, Encoded Storage, Whitelisting, TempStorage, and Box Sorters to sort and store almost every item in a compact UI with local bulk storage for up to 62 item types, auto/manual restocking from Encoded Remote Bulk, and 62 parallelized cartMIS sorting slices.
## Features
- Processes up to 55,000 items/hr
- Local Box Sorter Bulk Storage with overflow to Encoded Remote Bulk
- Built-in auto and manual restocking
- Simple user interface
- Custom cartMIS slice with box unloaders and automatic box bypass based on fill level
- Includes 5 built-in peripherals: mini furnace array, simple crafting system, restock station, potion brewer, and firework rocket autocrafter
## Considerations
- No first box placement for bulk items (use dummy box during build)
- Ideal Splitter may be intimidating to build, but can be done. It also uses many item entities which is bad for lag.
## Sourced Components
- Ideal Splitter v3 by Andrews54757 ([VIP003 32X and 64X Compact Ideal Splitter](https://discord.com/channels/1375556143186837695/1388318356377043076))
- Whitelister, HyperThreaded TempStorage, and Compactor by TisUnfortunate 
- Remote Bulk Storage assembled by jayroi (Others' components, but assembled for me by jayroi)
- cartMIS Whitelister by Inspector Talon
- cartMIS Slice inspired by Luxar , modified Civic Dude 
- Shulker Box Sorter by 金合欢酱喵~ (acaciachan) , HeadUnit modified by Civic Dude 
- Cart yeeting unloaders by Christone 
- Unstackable Sorter by 77777777777777777777 
- Shulker Based Chunk Loader by: kahyxen
- Too many more to fully list out here.
## Notes
Don't put in a full cache of empty boxes in input or input system will get bricked.
## Compatibility
Minecraft 1.21+
## Instructions
1. Make sure that the chunkloader portals are linked (see nether schematic). See WDL file for portal alignment example.
2. Put mixed boxes or loose items in the input on the bottom of the wall. Put bulk boxes (full boxes of one type) in the bulk input embedded in the floor of the input area.
3. It will automatically begin sorting once cache/queue is full. you can also press a stone button to start sorting immediately.

## Other Images
<img src="images/2024-02-08_20.30.59.png?raw=1" height="300px">

<img src="images/2024-02-08_20.44.43.png?raw=1" height="300px">

<img src="images/2026-01-21_15.39.45.png?raw=1" height="300px">

## Resources
- [MIS011_CMIS_V5_nether.litematic](attachments/MIS011_CMIS_V5_nether.litematic): MC 1.21.4, Size 12x6x25 blocks
- [[NEW] CMIS 5.0 - A Minecraft Main Storage](https://youtu.be/bvo-P9Nj71Y): by [Civic Dude](https://www.youtube.com/@CivicDudeGaming)
  - System Demo Video
- [MIS011_CMIS_V5_Demo_2.zip](attachments/MIS011_CMIS_V5_Demo_2.zip): MC 1.21
- [MIS011_CMIS-V5.0.litematic](attachments/MIS011_CMIS-V5.0.litematic): MC 1.21, Size 75x44x94 blocks
