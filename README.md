# Coffee Crawl fork

Crawl is won by lair. Therefor, coffee crawl is the first ten floors of crawl, then one floor of Zot.

The goal of this game is to make a 15-30 minute crawl.

## Upcoming changes

Core changes

- [x] remove lair, orc, vaults, depths
- [x] shorten dungeon to 10 levels
- [x] temple always appears on level 2
- [x] remove portal branches besides bazaar
- [x] actually remove depths
- [x] remove drop restrictions for D1 to D4 to avoid too many 'boring' floors
- [x] remove things like adders from D:10 since the game is almost over by D:10
- [x] map zot enemies to dungeon enemies in random gen (for now)
- [x] remove abyss access via banish
- [x] remove abyss access via distortion weapons
- [x] remove abyss access via starting role
- [x] remove abyss access via god abilty
- [x] remove abyss access via distortion unwielding, replace with maligned_gateway
- [x] remove abyss access via Zot trap, replace with maligned_gateway
- [x] remove abyss access via miscast, replace with maligned_gateway
- [ ] revert mapping zot enemies to dungeon enemies
- [ ] rebalance zot enemies for a 10 level crawl
- [ ] to make orb run easier, nerf or remove panlords
- [ ] to make orb run easier, nerf orb run enemies to easier ones
- [ ] end the game when the player exits the realm of zot with the orb. This is to avoid players spending 10 minutes predigging tunnels in a now 25 minute game.

## Extended changes

Changes I would like to try, ala hellcrawl.

- [ ] remove dexterity
- [ ] remove bows
- [ ] remove upstairs
- [ ] remove food
- [ ] remove strength and intelligence
- [ ] remove id minigame

## Bad ideas

Changes I would like to try which are probably bad ideas.

- [ ] give every enemy in the game the briar patch ability thorn hunters have to prevent luring
- [ ] either flat increase piety gain or decrease piety cap

## Monster changes

To make Zot easier, I am going to change the following monsters to be weaker.

| Done | Monster               | Monster Enum               | Proposesd Comparable  |
| ---- | --------------------- | -------------------------- | --------------------- |
| v2   | MOTH_OF_WRATH         | MONS_MOTH_OF_WRATH         | MONS_VAMPIRE_MOSQUITO |
| v2   | BLACK_DRACONIAN       | MONS_BLACK_DRACONIAN       | MONS_TENGU_WARRIOR    |
| v2   | YELLOW_DRACONIAN      | MONS_YELLOW_DRACONIAN      | MONS_ORC_WARRIOR      |
| v2   | GREEN_DRACONIAN       | MONS_GREEN_DRACONIAN       | MONS_ORC_WARRIOR      |
| v2   | PURPLE_DRACONIAN      | MONS_PURPLE_DRACONIAN      | MONS_ORC_WARRIOR      |
| v2   | RED_DRACONIAN         | MONS_RED_DRACONIAN         | MONS_ORC_WARRIOR      |
| v2   | WHITE_DRACONIAN       | MONS_WHITE_DRACONIAN       | MONS_ORC_WARRIOR      |
| v2   | DRACONIAN_STORMCALLER | MONS_DRACONIAN_STORMCALLER | MONS_DEATH_KNIGHT     |
| v2   | DRACONIAN_MONK        | MONS_DRACONIAN_MONK        | MONS_ORC_WARRIOR      |
| v2   | DRACONIAN_SHIFTER     | MONS_DRACONIAN_SHIFTER     | MONS_ORC_SORCERER     |
| v2   | DRACONIAN_ANNIHILATOR | MONS_DRACONIAN_ANNIHILATOR | MONS_DEEP_ELF_MAGE    |
| v2   | DRACONIAN_KNIGHT      | MONS_DRACONIAN_KNIGHT      | MONS_ORC_KNIGHT       |
| v2   | DRACONIAN_SCORCHER    | MONS_DRACONIAN_SCORCHER    | MONS_ORC_SORCERER     |
| v2   | KILLER_KLOWN          | MONS_KILLER_KLOWN          | MONS_RAKSHASA         |
| v2   | DEATH_COB             | MONS_DEATH_COB             | MONS_HUNGRY_GHOST     |
| v2   | CURSE_TOE             | MONS_CURSE_TOE             | MONS_EYE_OF_DRAINING  |
| v2   | TENTACLED_MONSTROSITY | MONS_TENTACLED_MONSTROSITY | MONS_UGLY_THING       |
| v2   | ELECTRIC_GOLEM        | MONS_ELECTRIC_GOLEM        | MONS_OGRE_MAGE        |
| v2   | ORB_OF_FIRE           | MONS_ORB_OF_FIRE           | MONS_EFREET           |
| v2   | QUICKSILVER_DRAGON    | MONS_QUICKSILVER_DRAGON    | MONS_SWAMP_DRAGON     |
| v2   | SHADOW_DRAGON         | MONS_SHADOW_DRAGON         | MONS_SWAMP_DRAGON     |
| v2   | STORM_DRAGON          | MONS_STORM_DRAGON          | MONS_SWAMP_DRAGON     |
| v2   | GOLDEN_DRAGON         | MONS_GOLDEN_DRAGON         | MONS_SWAMP_DRAGON     |
| v2   | ORB_GUARDIAN          | MONS_ORB_GUARDIAN          | None                  |

### v1 balancing results

After completing v1 balancing, I tested out zot in wizard mode. I ran through the dungeon and to zot with 27 in all skills, but no other adjustments. I picked up items as I went to get a sense of what an average run might have after running the previous floors.

Then, I entered zot and fought the enemies there. They were still much stronger than what I was prepared for. I also saw some enemies as part of vaults which were not rebalanced, so I will need to revisit that.

I set all my skills to 14, which is still likely much better than what people would have at that time, and tried fighting some enemies. Overall, everything was still too strong. Orb of Fire killed me almost a dozen times, and absorbed at least fifty hits before going down. Damage-wise, things might be okay, but enemies still feel way too bulky. I will divide AC, EV and HP of the above enemies by two and see how that feels. This will bring most enemies closer to the durability of the average orc warrior. I will revisit damage after the durability issues have been revisited.

### v2 balancing actions

Cut hp in half for most Zot monsters. Brought AC and EV down in some cases.

## References

[DCSS README](https://github.com/crawl/crawl)
[Dungeon Crawl Short Soup](https://github.com/dcandido/crawl)
