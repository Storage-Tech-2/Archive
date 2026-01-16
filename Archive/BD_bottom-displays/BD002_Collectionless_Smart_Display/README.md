# Collectionless Smart Display
<img alt="collectionless_smart_display.png" src="images/collectionless_smart_display.png?raw=1" height="300px">

**Authors:** *catniped*

**Endorsed by:** *Andrews54757*

**Tags:** *Closed Box Detection, Auto Replacement, Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1388317191060979833)

A small smart display without empty box collection that breaks the box only when empty and closed.
## Features
- Small (6x6)
- Smart box breaking, only breaks it when empty and closed
- Global first box placement
- Minimum hoppers, fully locked
## Considerations
- When triggering while the display is replacing a box, the global first box placement can cause it to break a newly dispensed full box
- No empty box collection
- When emptying adjacent slices in very quick succession, one of them may fail to replace its box
- Buffers a box

## Resources
- [BD002_collectionless_smart_display.litematic](attachments/BD002_collectionless_smart_display.litematic): MC 1.14.4, Size 6x6x2 blocks
