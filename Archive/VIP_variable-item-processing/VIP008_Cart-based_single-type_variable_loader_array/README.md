# Cart-based single-type variable loader array
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Caribous*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional, Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1466911125688946759)

Given an item entity stream input, this device will load them into single-type boxes at high speeds. It uses variable cart filters to ensure each box contains only a single type.

The filter is based on the first item type that comes through. When that item stops coming through, the filter will automatically de-assign and the loaders will be reset, so it can assign to a new item type.
## Features
- Can handle up to 576k items/hr, but is expandable to higher speeds (add more loaders).
- Uses variable cart filters to filter items to match the first item type that comes through
- Automatically de-assigns filter, and resets loaders when it can't find the filtered item anymore.
## Considerations
- Can only load one item type at a time
- Directional, do not rotate or it will break
## Notes
Especially useful for loading boxes for concrete/tree farm output.

## Resources
- [VIP008_8gt_Cart_Var_v1.0.5.litematic](attachments/VIP008_8gt_Cart_Var_v1.0.5.litematic): MC 1.21, Size 9x10x33 blocks
