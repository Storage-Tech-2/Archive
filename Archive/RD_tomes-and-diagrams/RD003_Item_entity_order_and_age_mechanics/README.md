# Item entity order and age mechanics
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1456724032819957984)

Item entities have different properties which the technical minecraft community confusingly all call "age" for some reason. but make no mistake, it's not that simple.
## `ItemEntity.age`: Despawn counter
Starts at 0 when the item is spawned, then increments by 1 every gt inside entity tick. if passes 6000 (5 minutes), then the item is deleted. When merging, the merged entity's age is set to the minimum of the two merging entities. in effect, the lifetime of the item entity is set to the longest of the two merging entities.
## `ItemEntity.tickCount`: Tick counter
Starts at 0 when the item is spawned, then increments by 1 every gt. Every entity has this. increment happens before entity tick call in [`ServerLevel.tickNonPassenger`](https://mcsrc.dev/#1/1.21.11_unobfuscated/net/minecraft/server/level/ServerLevel#L817-829).
## `ItemEntity.id`: ID counter
Is fixed for an entity. Each entity is given an id that is one plus the previous id given to the previous entity.
## Ticking Order
This is the order inside the [`ServerLevel.entityTickList`](https://mcsrc.dev/#1/1.21.11_unobfuscated/net/minecraft/server/level/ServerLevel#L419-441) which defines which entity is ticked first. Order is set by order of spawning.
## Iteration Order
This is the order inside the [`EntitySectionStorage`](https://mcsrc.dev/#1/1.21.11_unobfuscated/net/minecraft/world/level/entity/EntitySectionStorage) which is based per subchunk. If you want to find entities in a certain area (eg for picking up item entities with a player or hopper), you will get a list with the order defined here. Crossing subchunks will change the order.
## Modulo 4
When ticked, entity uses the sum [`ItemEntity.tickCount + ItemEntity.id`](https://mcsrc.dev/#1/1.21.11_unobfuscated/net/minecraft/world/entity/item/ItemEntity#L146) and checks if it is divisible by 4 to begin self-movement. Essentially makes it so items spawned at same tick drop at different ticks from rest, one of 4. Combined with the fact that the entity id is incremented with a global counter, you can use this mechanic to do wireless redstone.
## Item entity merging
When ticked (so obeys ticking order), entity checks if [`ItemEntity.tickCount`](https://mcsrc.dev/#1/1.21.11_unobfuscated/net/minecraft/world/entity/item/ItemEntity#L163-169) is divisible by 2 if the item has crossed a block pos boundary, or 40 otherwise. Then it will check if it can merge with other entities in the same area (obeys iteration order). merging will reuse the entity with larger count, and discard the smaller count entity.
