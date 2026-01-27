# How to use Litematica
<img alt="25b5529d7a3b030ac136a6ce879d8ed2a1aa4a8d.png" src="images/25b5529d7a3b030ac136a6ce879d8ed2a1aa4a8d.png?raw=1">

**Authors:** *Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1464102124097900585)

You might have noticed that most of the things here in the ST2 archives have litematica schematics as downloadable attachments. Litematica is a mod that allows you to save and load schematics of designs in the game. It's very useful is a must if you want to use or developing any advanced Minecraft contraptions yourself.
## Install
1. Make sure you have fabric loader installed. See https://fabricmc.net/use/installer/ for installation instructions.
2. In your mods folder, install the [Litematica mod](https://modrinth.com/mod/litematica) by moving the jar file there.
3. Make sure [Malilib](https://modrinth.com/mod/malilib) is also installed. If not, install it too.
## Making schematics
1.  In-game, press `M` to open menu.
2. Go to area editor, set selection mode to "Simple"
3. Go back to previous menu, make sure tool mode is "Area Selection" (click it until it's that)
4. Exit menu, then grab a wooden stick. Press `M+R` to toggle rendering.
5. Set the boundaries of your build by left clicking in one corner, and right clicking in the opposite corner
6. Go to the area editor again. Set the selection name. Then, click "Save schematic"
7. Adjust filename as necessary, then click "Save schematic" again.
8. Your schematic is located in the `schematics` folder inside your `.minecraft` (on win) or `~/Library/Application Support/minecraft` (on macos) folder.
## Using schematics
1.  The schematic you want to use should be placed in the `schematics` folder already
2. In-game, press `M` to open menu.
3. Click "Load Schematics"
4. Select the schematic file you want, then click "Load Schematic"
5. Exit back to the main litematica menu. Now you can go to "Schematic Placements" to configure where you want it.
6. Alternativey, in the main litematica menu, set Tool Mode to "Schematic Placement". In the game, turn on rendering with `M+R`. You can then grab a stick item in your hotbar, and click in the world to place the schematic where you want it.
7. If you are building a schematic in survival, use the Render Layers configuration (in configuration menu) to restrict rendering to a certain layer range. after you build a layer, increase the layer amount and build the next one. Do this until you built the whole thing. Then verify that you built it correctly using the Schematic Verifier (Litematica menu > Schematic Placements > Configure your placement > Schematic verifier button).
8. If you want to paste a schematic in creative mode, set Tool Mode to "Paste Schematic in World." Then grab a stick, make sure rendering is on, and use the executeOperation hotkey (you need to set this yourself in the configuration menu) to paste it.
## Using the ST2-Downloader mod
The [ST2-Downloader mod](https://modrinth.com/mod/st2-downloader) integrates with Litematica to automatically download and load schematics from the ST2 archives here into the game. Simply click on a litematic attachment within a post, and it will auto load it into Litematica for you.
## Tips
- There are lots of YouTube tutorials out there, use them if you are confused.
- Set datafixerMode to Always to ensure that schematics from older versions are loaded with inventories correctly.
- Also set both entityDataSync and pasteUsingServux to true so that you can paste instantly with inventories on servers using the Servux mod.
