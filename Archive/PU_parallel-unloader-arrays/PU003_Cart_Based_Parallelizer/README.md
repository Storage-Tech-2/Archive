# Cart Based Parallelizer
<img alt="area_render_26_.png" src="images/area_render_26_.png?raw=1" height="300px">

**Authors:** *_javierrubik33, morb1d0, pebeye, wreg_*

**Endorsed by:** *Andrews54757*

**Tags:** *Untested*

This system aims to accelerate the sorting speed of your main storage by unloading multiple items simultaneously whilst ensuring every item type isn't unloaded faster than what a single filter can handle. Hopper carts are used as a way to quickly pick up full stacks of items and unloading them via cart yeeting. To use drop any items on the input pressure plate and connect your filters to the output. Due to the nature of the system, filters that are compatible with it are: ss2 ssi filters (excluding push filters) and overstacked filters.

## Features
- Up to x64 hopper speed (576k items/hour)
- Small footprint (12x12x12 blocks)
- 3 separate outputs for stackables, unstackables and boxes
- Can handle any input (but stacked unstackables)
- Bufferless (any single item will be instantly dropped into the output, same for unmapped items)
- 4d aligned output
- ~88% hopper locked (30/33 hoppers)

## Considerations
- Entity lag
- Can't be rotated (curved rail redirection is used)
- Any stacked unstackables (StackableShulkerBoxes included) inputted will not be sorted correctly and one item of every stack would despawn.

## Notes
Use the north direction sub schem, the others might be forked. Explanation of device in thread.

## Resources
- [PU003_Cart_Based_Paralleliser_Javi.litematic](attachments/PU003_Cart_Based_Paralleliser_Javi.litematic): MC 1.20.2, Size 26x12x26 blocks
