# Simple 5x Parallel Unloader Using Carts
<img alt="area_render_110_.png" src="images/area_render_110_.png?raw=1" height="300px">

**Authors:** *Passionate Storage Techer 69, Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1406048074920493137)

A small device that takes in boxes and outputs items for filtered storage systems, ensuring no more than 1x hopperspeed per item type and capable of outputting up to 5 different item types simultaneously for up to 5x hopperspeed.
## Features
- Very small, only 11x11x12
- 4D aligned item output
- Separate unstackable and empty box output
## Considerations
- Slow and cannot be expanded beyond 5x hopperspeed
- Does not work with SS3 filters, items are output with a max stack size of 62/14
## Notes
Built on ST2 CMP (par unloader dev waypoint). Uses a modified version of the [OIP002 Hopperspeed Item Entity isStackable](https://discord.com/channels/1375556143186837695/1388317887462113373) item entity unstack separator ([OIP002 Hopperspeed Item Entity isStackable](https://discord.com/channels/1375556143186837695/1388317887462113373))
## Explanation
This device uses hoppercarts to ensure only a full stack of a single item type is output at a time. A single hoppercart is driven beneath 5 boxes, allowing it to pick up the first item type of those boxes. Then any remaining empty slots are filled with dummy items. The cart is driven under the boxes over and over again, for 512 gt to allow all slots to be filled completely if possible. The cart is then yeeted and the output is brought to an unstackable filter which removes unstackable items and separates 2 items from the stack to be sent separately 16gt later (so item stacks have max size of 62/14 and can be filtered).

## Resources
- [PU004_simple_5x_parallel_unloader.litematic](attachments/PU004_simple_5x_parallel_unloader.litematic): MC 1.21.4, Size 11x11x12 blocks
