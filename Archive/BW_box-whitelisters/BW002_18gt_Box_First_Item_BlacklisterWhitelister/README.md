# 18gt Box First Item Blacklister/Whitelister
<img alt="b.png" src="images/b.png?raw=1" height="300px">

**Authors:** *DrakePHOSE*

**Endorsed by:** *Andrews54757*

**Tags:** *Recommended, Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1472348054794408108)

Separates boxes based on if the first item of the input box matches an item set.
## Features
- Output can be adjusted. For example: moving the gate to a different distance, replacing the gate with a piston setup (the gate cannot be replaced by a trapdoor at the distance shown), or by locking or unlocking a hopper to separate the box.
- Can be expanded or made smaller, however the 8 slice version presented is the only one I tested. If hopper separation is used, additional testing should be minimal.
- 50-53 items per slice can be sorted, depending on how many 16 stackables there are in the chest.
## Considerations
- If an item or empty box is input, the output will spit out a hopper minecart. If enough hopper carts are spit out, it will break.
## Notes
- The chest should be configured to have 55 dummy 64 stackables and 3 unstackables. To add an item to the black/whitelist, remove 1 stackable item, or 4 if the item being added is a 16 stackable, then add ***only*** 1 of the listed item into the chest.
- Add an item ***only*** to 1 chest.
- The signal strength of the comparators reading from the chests should be 2 then change to 1 when one item is removed from the chest.
- Don't place a hopper on the rejected box output on the level right below the fence gate, the item can randomly hit the edge of the block and end up in the whitelisted output. Place it 1 block further below.

## Other Images
<img src="images/w.png?raw=1" height="300px">

## Resources
- [BW002_DrakePHOSE_18gt_Box_Blacklister.litematic](): MC 1.21.1, Size 17x10x6 blocks
- [BW002_DrakePHOSE_18gt_Box_Whitelister.litematic](): MC 1.21.1, Size 17x10x6 blocks
