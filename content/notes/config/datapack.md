---
title: "⚙️ Data Packs"
tags:
- config
---

> [!quote] [From the Minecraft Wiki](https://minecraft.fandom.com/wiki/Data_pack)
The data pack system provides a way for players to further customize their Minecraft experience. 
Data packs can be used to override or add new advancements, dimensions, functions, loot tables, predicates, item modifiers, recipes, structures, tags, damage types, world generation settings, and biomes without any code modification.


Biome Makeover is primarily configured via Data Packs.  While this does add some complexity, it also allows for more customization and decreased development time. 

Biome Makeover does have a small configuration file, but it will only be used when there is no other solution for configuration.  

## Getting Started

### Prerequisite Information
As overview will not cover:
- Creating or Moving files
- Installing Data Packs
- JSON formatting

We suggest reading through the following information provided by the Minecraft Wiki:
- [Data Pack](https://minecraft.fandom.com/wiki/Data_pack) - An overview of Data Packs
- [Creating a Data Pack](https://minecraft.fandom.com/wiki/Tutorials/Creating_a_data_pack) - Information of making your own data packs
- [JSON](https://minecraft.fandom.com/wiki/JSON) - Information about JSON syntax

### Base Data Pack
This is a starting point for your Biome Makeover Data Pack. It contains no configuration files, just the files required for a data pack and the folder structure to customize anything in Biome Makeover.  

You may delete any of the subfolders you do not use. Please rename the data pack file and information inside the `pack.mcmeta` file.

This data pack was last updated for Biome Makeover version `1.19.4-1.9.0`, but should still work on future versions.

[Download the Base Pack Here](notes/config/biomemakeover_example-datapack.zip)

### Biome Makeover's Data
If you wish to overwrite or modify Biome Makeover's data, you must know what each data file is.  

These can either be found within the mod .jar or [on the mod's Github Repository](https://github.com/Lemonszz/Biome-Makeover/tree/HEAD/common/src/main/resources/data).

### Getting Help  
We're happy to help, [Join our Discord](https://discord.gg/D5bNnw7) and make a thread in the `#configuration` channel. Please only do this after you have attempted for yourself.

## KubeJS
[KubeJS](https://www.curseforge.com/minecraft/mc-mods/kubejs) is a powerful Fabric/Forge mod that allows you to make scripts to modify the game, this is a very good alternative to Data Packs.

It also features a "Global Data Pack" feature that will load a data pack for any level. This is usually what you will want for modpacks.

Check out the [KubeJS website](https://kubejs.com/) for more information.

## Helpful Links
- [Biome Makeover's Data](https://github.com/Lemonszz/Biome-Makeover/tree/HEAD/common/src/main/resources/data).
- [KubeJS website](https://kubejs.com/)
- [Data Pack (MC Wiki)](https://minecraft.fandom.com/wiki/Data_pack)
- [Creating a Data Pack  (MC Wiki)](https://minecraft.fandom.com/wiki/Tutorials/Creating_a_data_pack)
- [JSON (MC Wiki)](https://minecraft.fandom.com/wiki/JSON)

## Biome Makeover Configuration
- 🧹[Custom Witch Quests and Rewards](notes/config/witch_quests)
- 🏷️[Tags](notes/config/tags)
- 🦦[Other](notes/config/other)