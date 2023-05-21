# Changelog

> [!Info] Older Changelogs  
> Changelogs listed here are for the latest Biome Makeover version.   

## Versions
Changelogs for specific versions, for versions not listed here, see their respective release pages
- [1.19.4](notes/changelogs/1194.md)

## Latest Minor

> [!summary] 1.19.4-1.9.1
>### Bug Fixes
>- Badlands surface fossils not being correctly buried
>- Fix Peat Composters not dropping anything when broken
>- Fix Glowshroom and Mushroom Stem blocks not having a tool assigned
>- Fix Peat Composters not having a tool assigned
>- Fixed Budding Illunite and Illunite Buds not having a tool assigned


## Latest Major

> [!example] 1.19.4-1.9.0
> ### Bug Fixes
>- Fixed Cowboy Hat z-fighting
>- Fixed Saguaro Cactus z-fighting
>- Fixed an issue with Ghosts sometimes spawning in light areas
>- Fixed the Stone Golem base hitbox remaining on the client side after the golem's death
>- Fixed Crab Chowder using the Cooked Crab food stats
>- Fix the bottom of the Witch Quest UI missing a row of pixels
>- Fixed disabled items appearing in the creative menu
>- Fix an oopsy where Buttonbush and Marigolds & Wild Mushrooms were not generating
>- Fix mod incompatibility issues related to crop/farmland blocks
>- Fix mod icon not loading correctly
>- Fix signs being crashy
>- Fix Potted Glowshrooms not emitting light
>- Fix Glowshroom Stem blocks not removing faces correctly
>- Fixed some Barrels within Ghost Towns containing no loot
>- Fix a Minecraft bug where Bell blocks not rotating when loaded by Jigsaw Structures ([MC-253819](https://bugs.mojang.com/browse/MC-253819))
>- Fix Nocturnal Effect not applying correctly
>- Fix wooden blocks not necessarily playing the correct sound when toggled by a Ghost or Poltergeist block
>- General stability improvements
>
>### Generation
>- Changed Blighted Balsa generation
> 	- Now generate in groups
> 	- Improved leaf placement
>- Tweaked some Ghost Town buildings
> 	- Removed real world iconography
> 	- Fixed some buildings destroying the ground below them
>- Fixed a Ghost Town Water Tower variant not generating
>- Improved Ghost Town loot
>- Replaced Mesmerite Boulders with Illunite Fissures
>- Increase the amount of Wild Mushrooms generating in the Mushroom Fields
>- Added Mushroom House structure
>- Mansion structures have had their data pack support improved
>
>### Mobs
>- Scuttler AI has been tweaked to more consistently eat petals
>- Pink Petals dropped from Scuttler eating Barrel Cactus is now dropped from a loot table
>- Updated Witch Quests
> 	- Can now reward froglights
> 	- The "Swamp Jives" music disc is now more common
> 	- Can now request tadpole buckets & mangrove propagules
>- Stone Golems will now drop at least 2 Cladded Stone on death
>- Pillagers can now drop Cladded Armor
> 	- 50% chance for a patrol leader
> 	- 5% for a regular pillager
>- Pillagers can now drop Crude Cladding and Crude Fragments
> 	- Patrol Leaders have a 100% Chance to drop either:
> 		- 75% 1 - 4 Crude Fragments
> 		- 25% 1 Crude Cladding
> 	- Regular Pillagers have a 25% Chance to drop either:
> 		- 90% 1 - 4 Crude Fragments
> 		- 10% 1 Crude Cladding
>- Renamed Cowboys to Marauder Pillagers
> 	- IDs haven't changed (yet)
>- Updated Mushroom Trader trades
>- Mushroom Trader no longer spawns naturally and no longer despawns (spawn in Mushroom House Structure)
>- Improved mob path-finding around barrel cactus, saguaro cactus, smally lily pads, water lilies and Black Thistle
>- Moth AI has been improved
>- Rootling Petal drops are now controlled by loot tables
>- Helmit Crabs will no longer pick up helmets with the `biomemakeover:helmit_crab_exception` tag (empty by default)
>- Witches will allow any item with the `biomemakeover:witch_hats` tag to be used for Witch Quests
>- Stone Golems can be healed with items in the `biomemakeover:heals_stone_golem` tag
>- Adjusted the Evoker's chance of dropping an Illunite Shard, it is also now affected by looting
>
>### Blocks
>- Adjusted Paydirt loot table
>- Barrel Cactus will no longer destroy items with the `biomemakeover:barrel_cactus_immune` tag (pink petals)
>- Added `biomemakeover:barrel_cactus_plantable_on` tag
>- Added `biomemakeover:saguaro_cactus_plantable` tag
>- Added Particles when Flowered Barrel Cactus is eaten by Scuttlers 
>- Illunite Rework
>	- Generates in Illunite Fissures
>	- Grows on Budding Illunite, from bud to cluster
>	- Blocks of Illunite can no longer be crafted back into 9 Illunite Shards
>- Cladded Stone explosion resistance has been increased from 1.5 to 6
>- Added Block of Crude Cladding
>- Mossy Peat can now be cooked into Dried Peat
>- Peat and Mossy Peat now have the `minecraft:dirt` tag allowing plants to be placed upon them
>- Tall Red and Brown Mushrooms can no longer be bonemealed
>- Tall Red and Brown Mushrooms can now generate when bonemealing mycelium
>- Peat is now renewable by dripping water into a full composter with dripstone
>- Peat and Mossy Peat are now replaceable by moss
>- Improved Willowing Branches selection boxes
>- Willowing Branches can now grow past 3 long
>- Willowing Branch Tips can be shorn to stop further growth
>- Willowing Branches can be bonemealed
>- Reviewed/Adjusted the map color for every block
>- The Altar will not curse items with any curse that has the `biomemakeover:altar_curse_excluded` enchantment tag
>- The Altar will not upgrade any enchantment with the `biomemakeover:altar_cant_upgrade` enchantment tag
>-  Blocks will now give off correct game events (sculk sensor signals) when activated by a Ghost or Poltergeist block
>- Daylight Detectors can now be toggled by Ghosts and Poltergeist blocks
>- Added Game Events (Sculk Sensor signals) to various Biome Makeover Actions
>
>### Items  
>- Buffed Cladded Armor projectile resistance from 1 to 1.5
>- Buffed Cladded Armor defense to be at the same level as iron rather than chainmail
>- Added Crude Fragments
>	- 1 Crude Cladding can be crafted into 4 Crude Fragments
>	- 4 Crude Fragments can be crafted into 1 Crude Cladding
>	
>### Textures:
>- The following textures have been updated:
>	- Purple, Green and Orange Glowshroom Blocks
>	- Glowshroom Stem
>	- Purple, Green and Orange Glowshroom Bricks
>	- Glowshroom & Mushroom Stem Brick
>	- Brown & Red Mushroom Brick
>	- Paydirt
>	- Cladded Stone
>	- Crude Cladding
>	- Bighted Balsa Logs and Sapling
>	- Illunite Cluster
>	- Glowfish (Entity, Raw Glowfish, Cooked Glowfish, Glowfish Bucket)
>	- Mushroom Trader
>	- Glowshroom Stew
>	- Some spawn egg colours
>	
>### Other
>- Witch Quest Rewards are now data-driven
>- Mushroom Villager trades are now data-driven
>- Added uk_ua translation (Ukrainian), Thanks, Tema Hromosoma!
>- Sorted Translation files



