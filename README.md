# The Beast v1 Improvements

This repository serves to log and record improvements I have made to my friend's Beast 3D printer.

Improvements:

* [self-contained span](#suspension-span) to suspend the signal/data cables & Bowden tubes
* [bltouch upgrade](#BLTouch-Upgrade)
* [z-axis stability upgrade](#Z-Axis-Stability-Upgrade)

## Suspension Span

See [here](./docs/suspension-span.md).

## BLTouch Upgrade

Follow the directions on [3d Beast Builders forum](http://3dbeastbuilders.boards.net/thread/231/bltouch-auto-leveling-distortion-correction).

Additionally, I moved and re-purposed the Z-min end-stop as a Z-max end-stop.

Configured firmware can be found [here](./firmware-repetier-1-x-y/README.md).

**Note that Thermistor 4 must be connected to the 'THB' pin in this updated firmware.**

## Z Axis Stability Upgrade

Follow directions in this [3d Beast Builders post](http://3dbeastbuilders.boards.net/thread/233/beast-v2-system-upgrade-v1). I followed the latter recommendation to leave all three Z motors in place and wired up.
