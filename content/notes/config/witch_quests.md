---
title: "🧹 Custom Witch Quests & Rewards"
tags:
- config
---

With [data packs](notes/config/datapack) you can modify both the requested items and the rewards from [Witch Quests](notes/mechanic/witch_quest).


# Requested Items
Items required for quests come from a "category". Each category is a collection of possible items for the Witch to request.  

Each category has a **weight**, the higher the weight, the more likely the category will be chosen.

When selection and item for a quest, a category is chosen, then an item is chosen at random from that category.  

Each item has a max count, being the maximum amount of that item the Witch will request.

Each item has a **point value**. The total amount of points for a single quest determines the difficulty of the quest, with higher being harder.

Harder quests have a higher chance of a better reward.

- [Biome Makeover's Categories](https://github.com/Lemonszz/Biome-Makeover/tree/HEAD/common/src/main/resources/data/biomemakeover/quest_category)

## New Category
Here is an example category file, we could call this file `my_cool_category.json`. It will go in the `data/[packname]/quest_category/` directory.  
```json
{
	"weight": 10,
	"requests": [{
			"item": "minecraft:apple",
			"max_count": 4,
			"points": 5
		},
		{
			"item": "minecraft:wheat",
			"max_count": 10,
			"points": 1
		},
		{
			"item": "minecraft:turtle_egg",
			"max_count": 1,
			"points": 10
		},
		{
			"item": "minecraft:tall_grass",
			"max_count": 4,
			"points": 2
		}
	]
}
```

In this category, we have a **weight** of 10, this is the likelihood that this category would be chosen.  

To change the rarity of this category, I could set this value to a lower number, `5` would make it twice as rare, while `20` would be twice as common.

Each item has it's own `points` value. This is the number that contributes to the rarity of the item. A higher `points` value item makes the reward more valuable.

## Overwriting a category
Say you want to remove all the Biome Makeover's default requested items.  You can not delete Biome Makeover's files, so you have to overwrite it. Here you have two options:

### Overwriting the file
Say we want to remove the `dark_forest.json` category.  

We create a new file at `data/biomemakeover/quest_category/dark_forest.json` within our data pack.  We then fill this file with our own data. 

This will fully replace Biome Makeover's `dark_forest.json` as they do not get merged.

### Overwrite and Empty
The other option is overwriting and emptying a category.  Again, say we want to remove the `dark_forest.json` category.  

We create a new file at `data/biomemakeover/quest_category/dark_forest.json`. 

This time we fill it with the following:

```json
{}
```

This is an empty JSON object. Biome Makeover will not attempt to load empty categories, effectively skipping it.

We would then create own own category in `data/[datapack name]/quest_category/my_cool_category.json` and fill it with our own data.

# Rewards
Rewards are the items received for completing a Witch Quest.

Rewards are split into "reward tables" that get selected based on the **points** of the completed quest.

## New Reward Table

A reward table contains two parts `weights` and `rewards`

### Weights  
Weights describe the rarity of this table being rolled for a specific quest rarity. A higher weight is more common.  

For example:
```json
"weights": { 
	"common": 110,
	"uncommon": 90, 
	"rare": 0, 
	"epic": 0 
	}
```

This describes a weights that are likely to be rolled for a common and uncommon quest, but has no chance for a rare or epic quest.

```json
"weights": { 
	"common": 1, 
	"uncommon": 10, 
	"rare": 50, 
	"epic": 100 
	}
```
This describes weights that have a very low chance on a common or uncommon quest, but a better chance on rare and epic quests.

### Rewards  

There are two types of rewards `biomemakeover:item` & `biomemakeover:potion`.

```json
{ 
	"type": "biomemakeover:item",
	"item": "minecraft:fermented_spider_eye",
	"min": 6,
	"max": 20
}
```
This describes an in item reward that will give `minecraft:fermented_spider_eye` with a minimum count of 6 and a max count of 20.

Items also have an optional `tag`, allowing you to give the item NBT:

```json
{
	"type": "biomemakeover:item",
	"item": "minecraft:diamond_sword",
	"tag": {
		"display": {
			"Name": "[{\"text\":\"Witchy Sword\",\"italic\":false}]",
			"Lore": ["[{\"text\":\"A sword once owned by a witch!\",\"italic\":false}]"]
		}
	},
	"min": 1,
	"max": 1
}
```
This describes a diamond sword with the name "Witchy Sword" and the lore "A sword once owned by a witch!"


```json
    {
      "type": "biomemakeover:potion",
      "potion": "minecraft:strong_leaping"
    }
```
This describes a reward that will give a leaping potion. All potion rewards have a chance to become splash or lingering potions.

### Full Example  
This is a cut down version and modified version of the file `data/biomemakeover/quest_reward/items.json`

```json
{
	"weights": {
		"common": 110,
		"uncommon": 90,
		"rare": 0,
		"epic": 0
	},
	"rewards": [{
			"type": "biomemakeover:item",
			"item": "minecraft:glass_bottle",
			"min": 1,
			"max": 10
		},
		{
			"type": "biomemakeover:item",
			"item": "minecraft:glowstone_dust",
			"min": 4,
			"max": 8
		},
		{
			"type": "biomemakeover:potion",
			"potion": "minecraft:strong_leaping"
		},
		{
			"type": "biomemakeover:potion",
			"potion": "minecraft:fire_resistance"
		},
		{
			"type": "biomemakeover:item",
			"item": "minecraft:spider_eye",
			"min": 5,
			"max": 10
		},
		{
			"type": "biomemakeover:potion",
			"potion": "biomemakeover:adrenaline"
		}
	]
}
```