# Variable Item Entity Parallel Unloader Array
<img alt="32b.png" src="images/32b.png?raw=1" height="300px">

**Authors:** *白Unique_Clock, ichika, Gufen*

**Endorsed by:** *Andrews54757*

**Tags:** *Untested*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1505654187365503068)

A parallel unloader array like device that directly processes item entity stacks instead of boxes. It makes sure that not more than 1x hopperspeed per type is being unloaded. Uses variable item entity filters to gather same-type items into groups for unloading, and unloads different types of items in parallel.
## Features
- Number of slices is customizable, more slices correspond to potentially higher speeds
- Precise 96gt clock can achieve full hopper efficiency (9000/h) for a single item type
- Outputs 12 items for 16-stack size and 60 items for 64-stack size respectively
- Final aligner output is timed perfectly so it is compatible with push filters
## Considerations
- Variable Item Entity Filter performs a global reset, waiting for the slowest unit in the PEIS to finish unloading. Recommended not to go below 16 times hopper speed
- Beyond parallel upper limit of item types, performance depends on specific input, and is relatively weak due to global reset constraint
## Notes
- Schematic includes two versions, with 32 units and 16 units respectively.
-  Fun fact: The term “rectification” (整流) in the Chinese TMC community refers to the generic idea of parallelization by types (with 1x per type), while parallel unloading refers to a specific method.

## Resources
- [PU006_1wtv2_B_32.litematic](attachments/PU006_1wtv2_B_32.litematic): MC 1.21.4, Size 10x15x44 blocks
- [PU006_1wtv2_B_16.litematic](attachments/PU006_1wtv2_B_16.litematic): MC 1.21.4, Size 10x15x28 blocks
