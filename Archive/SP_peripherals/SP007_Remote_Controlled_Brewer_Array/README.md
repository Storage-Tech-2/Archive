# Remote Controlled Brewer Array
<img alt="area_render_7_.png" src="images/area_render_7_.png?raw=1">

**Authors:** *bipim*

**Endorsed by:** *Andrews54757*

**Tags:** *Potion Brewer, Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1464409780700450867)

A 'remote' brewer using renamed tokens. To use, select the potion type (normal, splash, lingering) then press Q on the ticket(s) in the chest. Each ticket requests 3 potions. By choosing 9 tickets you can compose your own custom box.
## Features
- Makes every potion in 1.21 with the exception of drinkable water bottles.
- Parallelizes potion brewing using up to 9 brewing stands.
- The interface is separated from the actual brewer. Should be straightforward to link/make custom ones to fit in a storage hall.
- Initial distribution of fuel/water bottles.
- Protection from missing ingredients, fuel, bottles, dispenser dry firing.
- Hopper cart killed when idle.
- 'Speed' ranges from ~740 potions/h (6 ingredients) to ~940 potions/h (3 ingredients)
## Considerations
- requires some renaming
- not as fast as brewers doing multiple stages at once
## Notes
Tested with random input and varying number of ingredients for ~100k potions in all directions. Includes a schem and world download file with the interface wired to the brewer as an example.
## Compatibility
1.21+
## Instructions
1. Select the potion type (normal, splash, lingering)
2. Press Q on the ticket(s) in the chest to drop the token item to the collection hoppers below. Each ticket requests 3 potions.
3. By choosing 9 tickets you can compose your own custom box.

## Other Images
<img src="images/area_render_10_.png?raw=1">

<img src="images/image.png?raw=1" height="300px">

## Resources
- [SP007_brewer_array_v2_interface.litematic](attachments/SP007_brewer_array_v2_interface.litematic): MC 1.21, Size 10x7x9 blocks
- [SP007_brewer_array_v2.litematic](attachments/SP007_brewer_array_v2.litematic): MC 1.21, Size 10x15x25 blocks
- [SP007_Bipim_Remote_Brewer_Array_Wired.zip](attachments/SP007_Bipim_Remote_Brewer_Array_Wired.zip): MC 1.21.4
- [SP007_bipim_remote_brewer_wired_example.litematic](attachments/SP007_bipim_remote_brewer_wired_example.litematic): MC 1.21.4, Size 12x15x57 blocks
