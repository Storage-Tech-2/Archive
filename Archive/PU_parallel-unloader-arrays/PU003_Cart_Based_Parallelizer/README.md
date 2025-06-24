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

## Comments

### Andrews54757 (6/24/2025)
**Cart Based Paralleliser Explanation**
By: _javierrubik33
Logic:

__Input:__
System starts by spawning a cart that has its first 4 slots filled with unstackables to then pass it under the input item pile, thus allowing the cart to pick up a single stack  whether it is a regular item, an unstackable or a shulker box. After that, 4 unstackables are removed from the cart.

__2 Item Check:__
Later a 2 item check (that will be necessary for later steps) is performed, it works by removing 1 item with a hopper, and then detect the cart with detector rail + comparator. That pulse is later used to redirect the cart to one way or another. After the detection is done the item previously removed is returned to the cart.**1** If cart had only a single item it is rerouted to a presorter, which will separate boxes, unstackables and single items, each to its respective output.**2**

__Note 1:__ In between that step one item is taken from the cart and put right back, with the objective to get the cart performed the following way [2 0 0 0 62] to allow later processing.
__Note 2:__ Since input is being taken with full carts it means that if a single item has been found it is the last of its type, thus allowing direct output without danger of overflow.

