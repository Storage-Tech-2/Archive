# Borb-MIS
<img alt="508210971-e577d7af-4f02-4934-8dfc-e0bb319a8a74.png" src="images/508210971-e577d7af-4f02-4934-8dfc-e0bb319a8a74.png?raw=1" height="300px">

**Authors:** *borbarad13*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional, Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1461811417341624371)

A resilient multi item sorter with a compact frontend ("Borb-MIS").
## Features
- Sorts 64 & 16 stackables
- Flexible assignment: multiple item types per chest (no slot reservation)
- 42 categories in 16-wide chunk (2000+ item types)
- Highly unload resistant (tested 17000 gradual, 7000 instant, 1000 delayed reloads)
- Early survival buildable (first week)
- Reduced block palette (<27 types)
- Standalone or integrable
- Fault-tolerant to over/under/double assignments
- Minimal lag: +2 mspt on i7-6700 integrated server
- Rotatable. Orientation tested (90/180/270° rotations, no errors)
## Considerations
- Speed depends on input (~3K/hour)
- No shulker unloader, sorts only stackable items
## Notes
Credits: Fast detector rail by 2no2name (via Ilmango). All tests passed without errors.
## Compatibility
Designed & tested in 1.20. Likely works in 1.16+
## Instructions
1. Must be chunk aligned
2. Use Litematica recommended
3. Elevate floor before system by 1 block for chest access
4. Before category config changes: turn off system, await shutdown via maintenance hatch

## Resources
- [MIS007_B-MIS_-_Multi_item_sorter_by_B13_v9.zip](attachments/MIS007_B-MIS_-_Multi_item_sorter_by_B13_v9.zip): MC 1.20.1
- [MIS007_multi_item_sorter_b_mis_42_categories_one_chunk_by_borbarad13_2023_v9.litematic](attachments/MIS007_multi_item_sorter_b_mis_42_categories_one_chunk_by_borbarad13_2023_v9.litematic): MC 1.20.1, Size 16x18x13 blocks
