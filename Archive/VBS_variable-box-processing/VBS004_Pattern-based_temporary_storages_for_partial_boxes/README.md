# Pattern-based temporary storages for partial boxes
<img alt="area_render_11_.png" src="images/area_render_11_.png?raw=1" height="300px">

**Authors:** *bipim*

**Endorsed by:** *Andrews54757*

**Tags:** *Untested*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1464409896463106232)

Capable of retrieving multiple boxes cycling the chests content once. Instead of searching for box content or selecting a slot, it uses the pattern of key items and corresponding boxes in the chests, either replacing the key item with the corresponding box or leaving a gap, depending on the version used. If there's no match found, the chests won't be cycled. Suited for medium to high speed mergers and sorting sessions where you expect to merge a decent number of different item types.
## Features
- Speed:
  - Pair preserving: ~150gt/box (insertion) + ~900 gt (chest cycling and caching of pairs)
  - Ideal splitting: ~ 30 gt/box (check) + ~900 gt (chest cycling, pairs output) + ~24gt/box (non-matching boxes insertion)
- Capacity:
  - Pair preserving: **182** 64-stackables + **25** 16-stackables
  - Ideal splitting: **200** 64 or 16-stackables
## Considerations
- Can rarely produce empty or full boxes
## Notes
Comes in 2 versions: pair preserving (slow) and ideal splitting (fast). **Both versions can rarely produce empty or full boxes, just filter them out or use the add-on provided for the pair preserving version if your mergers can't handle that. **

The pair preserving version has two variants: one uses a simple fader to stop chest cycling until the current queue of boxes is done inserting, while the other one uses a dropper counter to count the matches and doesn't allow chest cycling until a user-defined number of pairs is found.  I recommend using the fader version.
## Compatibility
1.19+
## Instructions
- Pair preserving: input previously whitelisted partials. If merger can accept new pairs, clock the pair request line at 24gt or higher. Set the threshold of pairs found to a reasonable number depending on your system and expected input (if using the dropper counter version). If there's "overflow", cycle it back to the input immediately or use an intermediate buffer.
- Ideal splitting: Input a batch of previously whitelisted partials **that you know for sure don't have any duplicate item type**. Dump all the output back into the splitter/cycvar/whatever device you're using.

## Other Images
<img src="images/area_render_32_.png?raw=1" height="300px">

## Resources
- [VBS004_pattern_matching_temp_ideal_splitting_v1.0.1.litematic](attachments/VBS004_pattern_matching_temp_ideal_splitting_v1.0.1.litematic): MC 1.21, Size 6x12x25 blocks
- [VBS004_fill_level_restorer.litematic](attachments/VBS004_fill_level_restorer.litematic): MC 1.20.2, Size 5x5x4 blocks
- [VBS004_pattern_matching_temp_pair_preserving_v1_fader_version.litematic](attachments/VBS004_pattern_matching_temp_pair_preserving_v1_fader_version.litematic): MC 1.21, Size 26x11x7 blocks
- [VBS004_pattern_matching_temp_pair_preserving_counter_versionv1.litematic](attachments/VBS004_pattern_matching_temp_pair_preserving_counter_versionv1.litematic): MC 1.21, Size 26x11x7 blocks
