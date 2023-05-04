---
title: "💰 Loot Tables"
tags:
- config
---

> [!Info] Relative Paths
> Unless stated otherewise, all paths to loot tables are relative to `data/biomemakeover/loot_tables`.
> For example `mansion/arrows.json` is located in `data/biomemakeover/loot_tables/mansion/arrows.json`

## Blocks and Entities

Like vanilla, every block and entity has their loot table located at `blocks/[block name].json` & `entities/[entity name].json`, unless stated otherwise.

### Witch
Alongside it's vanilla loot table, the witch will also drop from the `entities/witch_hat.json` loot table.

### Pillagers
Alongside their vanilla tables Pillagers will also drop from either the `entities/pillager_leader_additional.json`  (Patrol Leaders only) or the `entities/pillager_additional.json` table.

## Gameplay Loot Tables

### Scuttler Eating
When a [Scuttler](notes/mob/scuttler) eats a [Flowering Barrel Cactus](notes/block/barrel_cactus), the petals will drop from the `gameplay/scuttler_eating.json` loot table.

### Rootling Shearing
When shearing [Rootlings](notes/mob/rootling), the petals will drop from one of the following color appropriate tables:
- `gameplay/rootling/blue.json`
- `gameplay/rootling/brown.json`
- `gameplay/rootling/cyan.json`
- `gameplay/rootling/gray.json`
- `gameplay/rootling/light_blue.json`
- `gameplay/rootling/purple.json`

## Structure Loot

### Ghost Town
[Ghost Town](notes/structure/ghost_town) loot is located in:

- `ghost_town/loot_0.json`
- `ghost_town/loot_1.json`
- `ghost_town/loot_2.json`

### Woodland Mansion
[Woodland Mansion](notes/structure/mansion) loot is located in:
- `mansion/arrows.json`
- `mansion/dungeon`
- `mansion/dungeon_good`
- `mansion/dungeon_junk`
- `mansion/good`
- `mansion/junk`
- `mansion/standard`

### Sunken Ruins
[Sunken Ruins](notes/structure/sunken_ruins) loot is located in `sunken_ruin.json`

### Mushroom House
[Mushroom House](notes/structure/mushroom_house) loot is located in `mushroom_house.json`