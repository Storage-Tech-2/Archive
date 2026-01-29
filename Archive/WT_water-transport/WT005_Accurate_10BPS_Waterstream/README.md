# Accurate 10BPS Waterstream
<img alt="image.png" src="images/image.png?raw=1">

**Authors:** *willymc*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1456717348068134943)

A waterstream that moves items at a rate of 10 blocks per second, allows for timing redstone signals with item movement. This design is closer to 10BPS than [WT003 10BPS Waterstream](https://discord.com/channels/1375556143186837695/1440940601724899448), for longer streams.
## Features
- Moves items at 10 blocks per second
- Allows for timing redstone signals with item movement
- Uses slime/piston pusher to shoot items at 10BPS starting at the first water block
- Average motion is 0.50003142 blocks per gt
- Tested for 2984 blocks (any longer items will despawn), the maximum error is 0.15625 blocks
## Notes
Item should be aligned against the slime block.

## Resources
- [WT005_accurate_10bps_stream.litematic](attachments/WT005_accurate_10bps_stream.litematic): MC 1.21.4, Size 2989x2x3 blocks
