# I can't believe this is optimal: why Lithium makes hopperlocking unnecessary
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1451060467060707470)

You've probably noticed by now that a lot of storage devices have a feature called "hopperlocking." Hopperlocking is the practice of powering inactive hoppers with redstone in order to prevent it from doing anything and reducing lag. Because a locked hopper has no need to know if there are any items in it's input or output (it can't move anything anyways), it will skip many computationally expensive checks every tick and produce much less lag when locked. Thus, many (older) storage tech devices will contain wiring to lock its hoppers as an optimization.
## Lithium makes hopperlocking optional
[Lithium](https://github.com/CaffeineMC/lithium) is a mod that every technical minecraft server uses. The way this mod works is very complex, but in general it uses more intelligent algorithms to make the game run more efficiently while preserving vanilla behavior.

In the past, when most storage tech was being developed, Lithium did not contain much optimizations specifically for storage tech. At this point, you still had to micro-optimize your storage by locking hoppers to prevent lag.

Today, in 2025, it's a different story. Lithium now has an optimization which automatically manages inactive hoppers, so that they produce no lag. Simply put, it automatically locks your hoppers for you, without you having to wire it yourself! **So if you have Lithium, hopperlocking does nothing**

If you want to store a bunch of items, say for bulk farm storage, you can just slap together a bunch of chests and hoppers as in the thumbnail, and call it a day. It will be just as optimal, as the more complicated locked bulk systems made in the past.
## Nuances
Today, hopperlocking is practiced because people enjoy the challenge of locking every hopper as a vestigial habit from the old days. Remember that the game's point is to have fun, and so if you find locking hoppers to be fun, go for it! But also, you don't have to lock your hoppers if you don't want to, and that will not make your design bad.

There are also some [complexities](https://github.com/CaffeineMC/lithium/blob/develop/common/src/main/java/net/caffeinemc/mods/lithium/mixin/block/hopper/README.md) with the way the auto-locking optimization is implemented under the hood for Lithium. For example, a hopper under a hoppercart will never auto-lock. These nuances often present themselves in niche cases and will not be an issue for most storage technologies. Moreover, Lithium gets better as time goes on, so what is an issue today might not be an issue tomorrow!
## Tldr
If you have Lithium, you don't have to lock your hoppers
