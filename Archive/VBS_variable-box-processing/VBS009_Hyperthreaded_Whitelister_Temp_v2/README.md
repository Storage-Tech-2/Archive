# Hyperthreaded Whitelister Temp v2
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *TisUnfortunate, Lukeem*

**Endorsed by:** *TisUnfortunate*

**Tags:** *Functional, Recommended, Independently Tested*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1503402043581141154)

A temp which uses whitelisters to divide bulk items into smaller categories to significantly decrease search and output times, and hyperthreads search operations to increase throughput. Designed to function as a variable loops exclusive whitelister. Special thanks to ComfyBiha and Kurisu for help testing.
## Features
- Can store up to 400 unique partials (50 per slice)
- Hyperthreaded Box Retrieval (*next box begins processing while previous bucket is being returned*)
- Fast non-whitelisted Handling (52gt cycle)
- Outputs full whitelisted boxes separately (same as non-whitelisted cycle)
- Compact(6x11x19)
- Accessible Temp Chests
- Random Input Proof
- 43 hoppers(27 idle locked)
- No idle cart
## Considerations
- Does not handle empty boxes, mixed boxes, or non-box items.
- Distribute your assigned items evenly across the slices
- Number of items assigned to each category is linearly related to cycle time, temp will get slower as you saturate the slices more. (first box input to a slice is 118gt)

## Resources
- [VBS009_HT.WL.Temp.v2.0.litematic](attachments/VBS009_HT.WL.Temp.v2.0.litematic): MC 1.21.4, Size 21x13x8 blocks
