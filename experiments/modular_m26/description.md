# Goals

- [x] Implement M26 as a fully-modular accessory:
  - [x] Usable as an underbarrel gun attachment
  - [x] Equally usable as an underbarrel attachment to its own standalone stock assembly

## Optional goals

- [ ] Implement the stock assembly as a gunmod for the `GUN`-implemented M26, making the M26 usable as both a gun and an underbarrel gun

# Results

The resulting gunmod operates successfully in both situations.

Because it's technically a separate gun when attached, the host (whether a gun or the stock assembly, if implemented as a firearm) cannot display the shotgun's ammo count in the inventory by default. This could be circumvented of, much like an AR-15 upper receiver, the M26 turns the stock assembly into a gun by supplanting its properties onto it. This does not disable the installed M26 from being considered a gun by the game, thus the M26 can still be chosen as a firing mode. (This may be countered by no longer rendering the M26 as partly a gun. That, however, will render it useless or item-breaking when installed on a regular firearm.)

Using the shotgun with the stock assembly requires the player to manually switch over to the shotgun's fire mode, even if the stock assembly "gun" has no legitimate way of firing on its own. This, though within the parameters of the experiment, precludes it from making it into the mod proper because it's inconvenient to the player, as well as unintuitive. (This would also apply to similar gunmod configurations, like the M320 with its standalone stock applied.)

Using the stock assembly as a gunmod on the M26 doesn't work because the M26 is hardcoded to not be able to fire independently, due to being an underbarrel-hosted gun. The M26, then, has to be installed on a different gun, which negates the entire point of the stock assembly being modular to the M26.

# Notes

- Stock assembly was modelled before Loadout changes to the ID, weight, and dimensions
