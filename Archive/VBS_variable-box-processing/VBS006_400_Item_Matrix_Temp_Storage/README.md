# 400 Item Matrix Temp Storage
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *TisUnfortunate, Ragdoll Willy, XP_Bot, giannis__, DNator, Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional, Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1480308116716257483)

Uses two whitelisters in a grid layout to store up to 400 partial boxes in 40 individually addressable droppers. Only 10 partials are stored in each dropper+hopper, making retrieval very fast (170gt) compared to disk drive temps. When you put in a box it will empty entire dropper with item, and put the boxes through a grouper. If there is matching box, both are output as pair, otherwise it stores the box in the dropper for later matching.
## Features
- Up to 400 item types
- 170gt fixed throughput for whitelisted input.
- 60gt fixed throughput for unwhitelisted input.
- Outputs unwhitelisted boxes separately.
- Fits in one chunk: 16x11x15
## Notes
Because of how fast the unwhitelisted input throughput is (60gt), this device can be used as your main whitelister for bulk/chest hall, provided that you are okay with full boxes being in the temp. This is very rare anyways, so it may be an acceptable compromise.

Designed on [Soontech CMP](https://soontech.org)
## Compatibility
1.21+
## Instructions
1. Set up whitelister chests with the item types you want to have in the temp
2. Put in partial boxes (each with a single type) into the input (barrel)
3. If unwhitelisted box, then it will be output out on one side. If whitelisted, it will output pairs on the other side.

## Resources
- [VBS006_matrix_temp_storage-r2.litematic](attachments/VBS006_matrix_temp_storage-r2.litematic): MC 1.21.4, Size 19x15x15 blocks
