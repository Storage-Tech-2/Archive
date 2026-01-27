# Unbreakable custom-duration pulsed clock
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Andrews54757*

**Endorsed by:** *Andrews54757*

**Tags:** *Functional, Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1450290815661244497)

This demonstration shows how one can make a custom-duration pulsed clock that is unbreakable to random on/off input.
## Features
- Adjust delay by adding more/removing repeaters, or any other delay block.
- Lever turns clock on/off
- Robust against random lever input. the clocked delay line will never have more than one pulse, and the controls will never fail to start the clock when enabled.
## Instructions
1. The trapdoor-pane latch ensures a pulse is sent every time the latch moves to the on position no matter how fast it is triggered.
2. The piston to reset the latch must be powered 2gt before the trapdoor is, so that double pulsing isn't possible and clock always turns off when desired.
3. The powered rail updates the other piston after reset piston is so that it can't be BUD-ed off permanently: the clock will always turn on with the lever on.

## Resources
- [CC005_unbreakable_custom_clock_demo.litematic](attachments/CC005_unbreakable_custom_clock_demo.litematic): MC 1.21.4, Size 6x3x9 blocks
