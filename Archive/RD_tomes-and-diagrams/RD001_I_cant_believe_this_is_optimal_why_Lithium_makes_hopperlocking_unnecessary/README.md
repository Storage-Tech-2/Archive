# I can't believe this is optimal: why Lithium makes hopperlocking unnecessary
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1451060467060707470)

You’ve probably noticed that many storage devices use a feature called **hopper locking**. Hopper locking powers inactive hoppers with redstone to prevent them from doing anything, reducing lag. Because a locked hopper can’t move items, it can skip several expensive checks each tick and generate far less lag. As a result, many older storage-tech builds include wiring to lock hoppers as an optimization.
## Lithium makes hopper locking optional
[Lithium](https://github.com/CaffeineMC/lithium) is a mod used on most technical Minecraft servers. Its internals are complex, but the goal is simple: improve performance while preserving vanilla behavior.

When much of today’s storage tech was developed, Lithium didn’t include many storage-specific optimizations, so locking hoppers was still a key micro-optimization.

Currently in 2025, that's changed. Lithium now includes an optimization that automatically manages inactive hoppers so they produce essentially no lag, effectively "locking" them without any extra wiring. **If you have Lithium, manual hopper locking won't improve performance.**

So for bulk storage (for example, farm outputs), you can often just stack chests and hoppers and call it done (like in the thumbnail). It'll be as efficient as older, more complex locked bulk systems.
## Nuances
People still hopper-lock because it's a fun challenge and a lingering habit from older designs. If you enjoy it, go for it, but you don't *need* to lock hoppers for your design to be "good."

There are also some [implementation details](https://github.com/CaffeineMC/lithium/blob/develop/common/src/main/java/net/caffeinemc/mods/lithium/mixin/block/hopper/README.md) in Lithium's auto-locking. For example, a hopper under a hopper cart won't auto-lock. These edge cases are usually niche and won't matter for most storage builds. And because Lithium improves over time, an issue today may be fixed tomorrow.
## Tl;dr
If you have Lithium, you don’t have to lock your hoppers.
