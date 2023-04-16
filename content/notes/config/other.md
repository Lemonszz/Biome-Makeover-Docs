---
title: "🦦 Other"
tags:
- config
---


These data pack features are too small to have their own dedicated pages.


## Custom Compostable Items
Our base library allows you to add compostable items via data pack:

Your .json files should be inserted in the `compostable` folder. E.g. `data/[your pack]/compostable/custom_compostables.json`

### Format  
You have two options when creating a compostable .json file, Single and Multiple.

#### Single
```json
{
	"item": "minecraft:gold_nugget",
	"chance": 0.3
}
```
This will allow gold nuggets to be inserted into a composter, with a 30% chance of adding a compost layer.

#### Multiple

```json
[
	{
		"item": "minecraft:gold_nugget",
		"chance": 0.3
	},
	{
		"item": "minecraft:iron_nugget",
		"chance": 0.4
	},
	{
		"item": "minecraft:raw_gold",
		"chance": 0.7
	},
	{
		"item": "minecraft:raw_iron",
		"chance": 0.4
	}
]
```
This adds gold nugget, iron nugget, raw gold and raw iron items as compostable entries with 30%, 40%, 70% and 40% changes of adding a compost layer.


## Brewing Fuel  
Our library allows you to add custom brewing stand fuel, we use this in Biome Makeover for [Soul Embers](notes/item/soul_embers). 

```json
{  
  "item": {  
    "item": "biomemakeover:soul_embers"  
  },  
  "fuel": 20  
}
```

One item per .json file.  You can use an empty json object `{}` to override a file.