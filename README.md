# Installation

Download and unzip zip file. The game should be playable.

# Goal

This is generally an awesome game. Well balanced out of the box and quite replayable. However, there are still OP strategies and elements in the game those allow to finish it very quickly disregarding gradual growth. I like to reduce their effect to emphacise gradual hero evolution.

I just modified what I think is OP and what makes game playable for me. Played and won with Sourceress on impossilbe and had pretty good time balancing army and money. I am not saying these are ultimate perfect changes. Please try it out and let me know (file an issue) if they need to be tweaked or something else need to be changed.

# Analysis

## Units

General unit design is simply amazing. Each unit level has its use and more advanced unit is not always better. Plus morale mixing mini game.

Due to the army HP limit (= hero leadership), higher HP actually makes unit **worse**. For example, say you have 100 leadership and enough money to fill it with either 100 peasants or 20 zombies. Simple math shows that 20 zombies are _less_ combat effective even with their small skill level advantage! I call this HP efficiency metric. There is also a money efficiency: the kick for the buck metric. Money efficiency is usually a less of an issue due to general abundance of money.

```
hit point efficiency = damage / HP
money     efficiency = damage * HP / (cost ^ 2)
```

HP efficiency is about same for all units across the board, give or take. Money efficiency goes down a lot for higher tier units. However, as stated previously, money is rarely the issue.

Of course, lower tier units have their drawback. The most notable is that with leadership increased there is just not enough of them in dwelling to fill up leadership quota. They are also get gradually less effective against higher tier units and, naturally, has to be abandoned as player target tougher enemies.

## Combat related spells

Fireball and Lightning are well balanced. Fireball is more devastating but slightly more expensive. Resurrection and Clone are also balanced. Resurrection generates twice as more units but slightly more expensive and is limited with initial units count. Balance between these two groups (damaging enemy units and restoring own units) seems to be fine too. It is about four times more expensive to restore own units, which makes sense as they usually dying much slower.

# Mechanics.

I modified the mechanics years ago and do not remember all the bugs and things I fixed. The only one I recall is that enemy troops are moving toward the player, NOT toward where the player was. That disables the ability to dance around them. You either fight or go back. In some circumstances, like when you enter the town fleeing from wandering army, you cannot exit the town without a fight.

# Spoil of war

The spoil of war income becomes incredibly large mid game solely sufficient to maintain further army improvement and self fueling speedball conquest. Ignoring income restriction and cost of troops makes the rest of the game not interesting.

Reduced by factor 2.5.

# Spell mofifications

## Time stop

Second level sorcerer with 10 spell power can buy tons of these and move 100 steps per 200 gold. With huge mid game spoil of war income that effectivelly stops the time forever.

Spell cost is increased to **5000**.

## Castle Portal and Town Portal

Same can be said about instant teleportation. They are not that abusive as Time stop but nevertheless allow for huge time save including bypassing week of traveling to other continent.

Spell cost is increased to **5000**.

## Raise control

Too cheap for sorcerer with 10-20 spell power resulting in 1000-2000 lidership improvement per single spell.

Spell cost is increased to **5000**.

# Unit modifications

## Morale groups

### Group A

Peasants and Militas. No changes.

### Group B

Castle troops. Generally made slightly less efficent and much more expensive to compensate their unlimited supply.

### Group C

Good creatures. No bonuses or penalties. They have about same amount of good and bad effects: do not lower other creatures morale, can get high morale, and frightened by evil and undead creatures.

### Group D

Evil creatures. No bonuses or penalties. They have about same amount of good and bad effects: lower good creatures morale, can get high morale, do not lose their morale.

### Group E

Undeads. Slight bonus to damage due to difficulty mixing them with many other units.

## Units

| name  | HP | dmg min | dmg max | cost | modification explanation |
| ---- | ---: | ---: | ---: | ---: | ---- |
| Peasant | 1 | 1 | 1 | 10 |  |
| Sprite | 1 | 1 | 2 | 15 |  |
| Militia | 2 | 1 | 2 | 50 |  |
| Wolf | 3 | 1 | 3 | 40 |  |
| Skeleton | 3 | 1 | **3** | 40 | Match wolf efficiency. |
| Zombie | 5 | 2 | **4** | 50 | Increase appeal. |
| Gnome | 5 | 1 | **4** | 50 | Increase appeal. |
| Orc | 5 | 2 | 3 | 75 |  |
| Archer | 10 | 1 | 2 | 250 |  |
| Elf | 10 | 1 | 2 | **400** | Compensation for most powerful shooter. |
| Pikeman | 10 | 2 | 4 | 300 |  |
| Nomad | 15 | 2 | **6** | 300 | Match pikeman efficiency. |
| Dwarf | **15** | 2 | **8** | 350 | Rebalance for more efficiency. |
| Ghost | **15** | 3 | 4 | 800 | Rebalance for less efficiency. |
| Cavalry | 20 | 3 | 5 | **1500** | Expensive castle unit. |
| Ogre | **25** | 3 | **7** | 750 | Increase appeal. |
| Barbarian | **30** | 1 | **9** | 750 | Increase appeal. |
| Troll | 50 | 2 | 5 | 1000 |  |
| Druid | 25 | 2 | 3 | 1000 |  |
| Archmage | 25 | 2 | 3 | **1500** | Better than Druid. |
| Vampire | 30 | 3 | 6 | 1500 |  |
| Knight | **50** | 6 | 10 | **3000** | Expensive castle unit. |
| Giant | **100** | **5** | **15** | **6000** | Rebalance for less efficiency. |
| Demon | 50 | 5 | 7 | **6000** | More expensive for super ability. |
| Dragon | 200 | **10** | **30** | **20000** | Rebalance for less efficiency. |

