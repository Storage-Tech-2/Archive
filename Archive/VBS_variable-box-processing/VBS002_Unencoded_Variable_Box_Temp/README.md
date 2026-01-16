# Unencoded Variable Box Temp
<img alt="area_render_107_.png" src="images/area_render_107_.png?raw=1" height="300px">

**Authors:** *vincent, 77777777777777777777, insto*

**Endorsed by:** *Andrews54757*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1401376236223074426)

Stores a partial box until another partial box with the same item type is input, after which both are output for merging. Despite being an unencoded system, this device is capable of quick access using a CUD based integrated variable "encoder."
## Features
- Up to 312 item types, 26 types in 12 slices.
- Uses CUDs and a built in variable encoder-like device to quickly identify slices storing a specific type. Takes only 70gt to insert a box if no match is found.
- Even distribution of boxes across slices during initial filling. Afterwards, boxes are put in from furthest to closest slice to the input.
- Automatic ejection of overflow when there is no more capacity.
- Built-in item aligner for direct input into mergers
- Pauseable
## Considerations
- If a matching item type box is stored, the boxes in a matched slice are cycled through a variable box filter which can take up to 8*26 = 208 gt extra.
- Expanding the design to store more item types is not straightforward
## Notes
Press the wooden button to start processing input. Flip the lever on the yellow concrete block to pause the system. Can theoretically work in Minecraft 1.16+

## Acknowledgements:
- wreg: Original unencoded temp idea using CUDs
- 雨天: Original unencoded temp idea using CUDs

## Other Images
<img src="images/area_render_108_.png?raw=1" height="300px">

## Resources
- [VBS002_unencoded_variable_temp.litematic](attachments/VBS002_unencoded_variable_temp.litematic): MC 1.21, Size 8x11x31 blocks
