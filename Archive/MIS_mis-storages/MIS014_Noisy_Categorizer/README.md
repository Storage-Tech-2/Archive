# Noisy Categorizer
<img alt="render.png" src="images/render.png?raw=1" height="300px">

**Authors:** *Саня, (っ◔◡◔)っ ♥ Naijuunitengo ♥*

**Endorsed by:** *Moonyinspired 🇧🇷*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1511482219334729758)

Cheap and compact early game 1wt multi item sorter similar to [MIS001 Compact Categorizer](https://discord.com/channels/1375556143186837695/1388318067247026286).
## Features
- trapped chest input for everything
- unloads boxes
- <=1x hs (close to 1x with batches of ~23+ items)
- pausable
- 48 categories (including 3 empty) up to 50 items in default version
- size: 15x15x31
- overflow protection
- accessible whitelisters
## Considerations
- 2 stationary carts
- noisy due to powered droppers
## Notes
- Schematic has output signal to add chunk loading
- White glass in schematic represents solid block or glass
- All signs are optional
- Easily expandable in both axis
## Compatibility
1.20.4+
## How it works differently
While the overall principles of operation are similar to [MIS001 Compact Categorizer](https://discord.com/channels/1375556143186837695/1388318067247026286), this storage uses droppers to move items into slices instead of item entities. This allows it to move variable amounts of items (instead of fixed amounts), until that item type stops being sorted. This allows it to not use extra sorting cycles to insert large batches of the same item type.
## Instructions
1. Make sure to setup MIS filters first (top chests), a basic 1.21.9 layout is included separately, but the schematics do not have preset MIS chests.
2. Hook up chunkloading. There is a sign next to an observer which you may use as the clock source for your chunkloader.
3. Put either items or boxes into the input to start sorting

## Acknowledgements:
- (っ◔◡◔)っ ♥ Naijuunitengo ♥: Made decoration

## Other Images
<img src="images/slice.png?raw=1" height="300px">

<img src="images/image.png?raw=1" height="300px">

## Resources
- [MIS014_noisy_categorizer_1.20.4.litematic](attachments/MIS014_noisy_categorizer_1.20.4.litematic): MC 1.20.4, Size 15x15x31 blocks
  - Litematic of storage system
- [MIS014_noisy_categorizer_1.20.4_subregions.litematic](attachments/MIS014_noisy_categorizer_1.20.4_subregions.litematic): MC 1.20.4, Size 15x15x31 blocks
  - Litematic of storage system with subregions for digging out area in survival
- [MIS014_noisy_categorizer_decorated_1.21.9.litematic](attachments/MIS014_noisy_categorizer_decorated_1.21.9.litematic): MC 1.21.11, Size 15x15x32 blocks
  - Fully decorated version (deco by @adrian05584)
- [MIS014_MIS_layout_1.21.9.litematic](attachments/MIS014_MIS_layout_1.21.9.litematic): MC 1.21.11, Size 9x8x24 blocks
  - Preconfigured MIS chests for a basic 1.21.9 item layout. Only has MIS chests, does not include the storage system.
