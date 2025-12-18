# Cart Based Parallelizer
<img alt="area_render_26_.png" src="images/area_render_26_.png?raw=1" height="300px">

**Authors:** *javierrubik33, Morbido, pebeye, wreg*

**Endorsed by:** *Andrews54757*

**Tags:** *Untested*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1388318282913943653)

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


### Andrews54757 (6/24/2025)
__Set:__
If cart has 2 items or more it goes to the set. The set is a 1x1x1 block were items are dropped and alligned via a dropper were carts can pass through to pick up the items being checked. 
Functioning: One item is taken out of the cart, renamed dummies are pushed into the cart, cart goes over the set (trying to pick the item it is checking) and then the item previously removed is dropped into the set.
That leaves us with two scenarios that will allow the system to tell if the cart should be accepted to the output or not, either the item was already in the set or it wasn't:

- It was: If the item was already in the set the cart will pick the item and then reset the exact same item back again, thus not changing the status of the set and leaving the cart with 2 of that item in the first slot [2 x x x 62]
- It was not: If the item was not in the set the cart will not pick any item and one will be added to the set, thus adding what was not already there and leaving the cart with the following arrangement [1 x x x 62]


### Andrews54757 (6/24/2025)
__Set Check:__
To decide if the cart should be accepted we use the information in hand, 2 items in the first slot or 1. This step starts by removing 1 item from the cart and trying to push another renamed item into it. The hopper that tries to push is completely full (giving ss15) if it succeds to push it will lower its signal strength to 14, which is used to redirect the cart. Same hopper that pushes will pull the same renamed item 8gt later from the same cart, returning back to ss15.
Depending on if the cart was accepted or not we do something with the item previously removed:

- Rejected: If the cart is rejected it is yeeted back to the input and the item previously removed is merged with its content.
- Accepted: If the cart is accepted it is yeeted into a 4d alligner that will send items to the output (a max of 62) and the single item is dropped into the unmapping queue which is simply a cobweb where items stay a precise amount of time, preserving order.
Note: In both cases the cart still had dummy items and that makes it so both outputs have to go over filters for dummies, and that's the reason why they are renamed and not unstackables.

__Unmapping:__
Unmapping is used to remove the key item from the set with a defined delay (enough for a hopper to process a full stack ~512gt) to allow for duplicate stacks of the same item to be accepted. It simply waits for the item previously sent to the queue line to arrive and spawns a cart that is used as a filter to go under the 1x1x1 and pick up the set item. Cart is yeeted directly into the output with 2 of that item being sent. Since those 2 items arrive to the filter before its full stack is completely filtered hopper cooldown won't be an issue. (This is one of the reasons why it is incompatible with push filters).

