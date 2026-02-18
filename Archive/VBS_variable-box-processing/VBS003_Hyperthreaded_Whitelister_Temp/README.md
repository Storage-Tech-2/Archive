# Hyperthreaded Whitelister Temp
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *TisUnfortunate*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1473820723696107726)

A device that can store up to 400 unique partials, with a compact design and various features for efficient operation.
## Features
- Can store up to 400 unique partials (50 per slice)
- Compact(6x11x19)
- Hyperthreaded Box Retrieval
*next box begins processing while previous bucket is being returned*
- 38 hoppers
- Paired Partials output to water stream
- Accessible Temp Chests
- Random Input Proof
- Handles non-whitelisted inputs
- Whitelisting Cart yeeted after use
## Considerations
- the hopper on top of the grouper and the block of water before it must be in the same chunk
- No Empty Box or loose item input protection
- processing time is ~linearly related to # of boxes in bucket. The more items allocated to a slice, the slower it can be (207gt for no boxes in bucket to ~715gt for 49 boxes in bucket).

## Resources
- [VBS003_Hyper.Threaded.Whitelister.Tempv1.2.litematic](attachments/VBS003_Hyper.Threaded.Whitelister.Tempv1.2.litematic): MC 1.21, Size 19x11x8 blocks
