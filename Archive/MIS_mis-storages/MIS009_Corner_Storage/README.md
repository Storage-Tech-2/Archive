# Corner Storage
<img alt="area_render_1_.png" src="images/area_render_1_.png?raw=1" height="300px">

**Authors:** *bipim*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1464410091057975570)

A decently fast and low lag multi item sorting + bulk solution. Originarily made for 1.19, updated to 1.21.

Extra credits in wdl.
## Features
- 4x hopper speed sorting, multiple slices can work in parallel (expect between 6x and 13x in real sorting sessions).
- Multi item sorting for shulker boxes and loose items, 1x hopper speed, multiple slices can work in parallel.
- Regular bulk with direct input.
- Individual threshold for each MIS category to decide if sort as box or unload items.
- Temporary storage to sort a selection of items (~160, expandable) only in full boxes.
- Basic safety features that stop the input and force pause in case of errors in chunkloading, excessive backlog, running out of boxes or overflow overflowing.
- Compatible with /carpet MovableBlockEntities=true.
- All inventories that may need to be fixed if the system gets unloaded are accessible.
- Decently hopperlocked. All the hopper carts are killed when idle. Low active lag (max 4mspt with lithium in i5-4210U, old laptop cpu)
## Considerations
- destroys boxes to unload their content
- boxes assigned to temp may be buffered in the merging loop and so made temporarily inaccessible, this is intended
- some components used are very old (splitter i'm looking at you)
## Notes
download: https://www.mediafire.com/file/flzlc49n1e1tpa9/jasps_v4.0.1.zip/file
## Compatibility
Updated to 1.21 (originally for 1.19)

## Resources
- [MIS009_jasps_v4.0.1.url](https://www.mediafire.com/file/flzlc49n1e1tpa9/jasps_v4.0.1.zip/file): Mediafire link
  - download
- [MIS009_corner_storage_jasps_v4.0.1.litematic](attachments/MIS009_corner_storage_jasps_v4.0.1.litematic): MC 1.21.4, Size 71x41x67 blocks
- [MIS009_corner_storage_jasps_v4.0.1_nether.litematic](attachments/MIS009_corner_storage_jasps_v4.0.1_nether.litematic): MC 1.21.4, Size 9x6x12 blocks
