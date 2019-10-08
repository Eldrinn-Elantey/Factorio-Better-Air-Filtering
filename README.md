# Better Air Filtering
#### A mod for Factorio that provides complex air filtering steps to remove pollution.


## Overview
![overview]()

This mod features three tiers of air filtering machines. These machines remove pollution from the air in their region by using air filters. Each consecutive tier has a larger radius and stronger filtering effect. Keep in mind that you will still need filters spread around your base at strategic locations to effectively counteract the spread of pollution.  

#### Air filter machine 1
You start with a basic passive air filter machine that cleans the air in its own [chunk](https://wiki.factorio.com/Map_structure#Chunk). It should help keep biter attacks at bay through the early game.

#### Air filter machine 2
The upgraded version has a stronger filtering effect. In addition, by using a moderate amount of electricity this machine is able to pull in pollution from neighboring chunks in the shape of a diamond. This version has a radius of two chunks (in [manhattan distance](https://en.wikipedia.org/wiki/Taxicab_geometry)). Note that a continuous amount of energy is consumed for this suction effect in addition to the cost of filtering the air.

![range_mark_2](res/radius_mk2.png)

#### Air filter machine 3
The third and final upgrade of the air filtering machine features a larger radius of three chunks along with more air filtering per second.

#### Filter Types
There are currently two types of filters: __expendable filters__ and __recyclable filters__. The first ones are easier to craft, but filter out less pollution and are destroyed upon use. __Recyclable filters__ are more expensive but can be refreshed with a bit of coal to be used again.

## Technical Details
Some things to keep in mind when using this mod:
 - The [evolution](https://wiki.factorio.com/Enemies#Evolution) factor of enemies is based on the total amount of produced pollution. Cleaning it back up does not reverse this effect. This means that biters will still get stronger, no matter how proficient you are at cleaning pollution. You can prevent attacks caused by pollution reaching the biter nests however.
 - Pollution from other chunks is sucked toward air filters at an exponentially decreasing rate depending on the distance. The formula is `suction = base_suction * (1/4)^distance`. This means that filters only pull in approximately as much pollution as they can filter.

## Changes
Refer to the Factorio mod page for the complete [changelog](https://mods.factorio.com/mod/better-air-filtering/changelog).


## Future Features
 - A third and more efficient air filtering production chain based on first "dissolving" pollution in water and then treating it in chemical plants.


## Bugs / Crashes / Suggestions
> Important! This mod is in it's early stages of development and has not yet been extensively tested and balanced.

If you experience issues, please notify me on the [forum](https://mods.factorio.com/mod/better-air-filtering/discussion). Suggestions for future releases are also welcome.
