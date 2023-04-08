---
title: "Owl"
tags:
- mobs
- tameable
---

![[notes/images/owls.png]]
## About

The Owl is a mob added as part of the [Dark Forest](notes/makeover/dark_forest) makeover.   

Owls can be tamed with any raw meat and they will fight along side you.

## Behavior
Owls can spawn on grass or leaf blocks with a light level higher than 2.

Untamed Owls will wander around the dark forest, attacking their prey.

Tamed Owls will follow their owner, attacking anything the owner attacked.  If the owner interacts with the owl, it will sit down and stay in place.

## Stats
| Stat | Value |
| ---- | ------ |
| Health (Untamed) | 6.0 |
| Health (Tamed) | 20.0
| Movement Speed | 0.4 | 
| Attack Damage (Untamed) | 2.0 |
| Attack Damage (Tamed) | 4.0 |
| Follow Range | 16.0 |

## Configuration
Owls will attack any mob with the `biomemakeover:owl_targets` entity type tag.

By default these are:
```
"minecraft:rabbit",  
"minecraft:chicken",  
"minecraft:silverfish",  
"minecraft:endermite",  
"minecraft:bat",   
"biomemakeover:dragonfly",  
"biomemakeover:lightning_bug",  
"biomemakeover:lightning_bug_alternate"
```
