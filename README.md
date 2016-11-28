# OmegaTweak v15.3
## 7 Days to die Tweaks by Devidian

### Changes to blocks.xml
* new Drop-Fall event paths (no magic disappearance of material)
 * Stone->destroyedStone->Gravel->sandStone->sand->sand
 * (type)Ore->(type)Ore 
 * added repair items (wood) for pew segments

### Changes to recipes.xml
* added book recipe for 64 paper + 1 leather (caseing)
* added paper recipe from book (1 book = 64 paper)
* added crushedSand recipe (18 sand from 1 destroyed stone)
* added machete repair recipe (1 machete 2 repair kit 5 forgedSteel)
* added jailDoor recipe (workbench)
* added commercialDoor1, 2 & 4 recipe (workbench)
* added emberpile1 & 2 recipe
* added pew segments recipes
* added miningHelmet recipe with footballHelmetZU

### Changes to entityclasses.xml

* Map Icon for Minibikes activated
* Backpack lifetime raised from 20 Minutes to 60 Minutes
* (UMA)Zombie/Hornet corpse lifetime raised from 30(45) to 60 seconds
 * Note: corpse still exist after rotting, no time to set(change) there currently
* Dog & Animal corpse lifetime raised from 300 to 900 seconds (15 Minutes)

### Changes to progression.xml
* Raised player level from 200 to 1000
* New Action Skill: Fistfight
 * Bonus 1: StaminaDegradation down to 0.66 (Level 100)
 * Bonus 2: EntityDamage up to 1.28
* New Action Skill: Machetes Training
 * Bonus 2: EntityDamage up to 1.28 (Level 100) and 1.40 (level 200)
* Added Machetes Training as requirement for knife guy and decapitator until we have something similar
* New Perk: Geologist with 2 level each 20 Skillpoints
 * Requirements: Player Level 50, Miner 69er Level 5, Mining Tools Level 100
 * Level 1: 10% Block Damage,  5% harvest count
 * Level 2: 20% Block Damage, 10% harvest count (With this one you can one-hit stone again)
* New Perk: Tools-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Tool smithing level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Weapon-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Weapon smithing level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Crafting-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Miscellaneous Crafting level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Gun perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Gun Smithing level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Science-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Science level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Tailoring-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Tailoring level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Leatherworking-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Leatherworking level 100
 * Level 1-5: 20-100 Quality points added
* New Perk: Armor-Perfectionist with 5 level each 20 Skillpoints
 * Requirements: Player level 200, Armor smithing level 100
 * Level 1-5: 20-100 Quality points added
* Changed xp of fistfight and machete training to 125 (from 100) to rebalance

### Changes to items.xml
* added Fistfight as Action0 group for player hand (id 70)
 * added actionXp (5)
 * added buffs to player hand
  * 5% chance to buff bleeding
  * 30% chance to stun
* uncommented book, changed stack to 100, fuel and weight to 64
* Added "Machetes Training" as ActionSkillGroup for machete
* changed machete repairMaterial to forgedSteel
* Adjusted stack numbers:
 * scrapIron 5000 -> 30000 (what fits in forge)
 * scrapBrass 5000 -> 30000
 * scrapLead 5000 -> 30000
 * ironFragment 1000 -> 3000 (->15000 Scrap iron,2 of it fit in forge)
 * crushedSand 1000 -> 3000
 * rockSmall 1000 -> 3000
 * yuccaFibers 1000 -> 5000
 * clayLump 1000 -> 3000
 * calipers 1 -> 10
 * toolAndDieSet 1 -> 5

### Changes to Localisation.txt
* Localisation for Geologist perk
* Localisation for fistfight (german & english only yet)
* Localisation for all perfectionist perks (german & english only yet)

### Changes to entitygroups.xml
* added new group with all +special zombies

### Changes to spawning.xml
* changed last entry for screamer horde to spawn zombies from special zombies group too

## Installation & Update Information
The current master is ONLY for Alpha 15, dont try to use with a lower Alpha version.

### Localisation 
Due to the fact that Localisation.txt is not pushed by the server, all players should be install the mod to have full Localisation feature (english & german).

### Linux Dedicated Server
Connect to your server via ssh and go to your Data folder. This for example is when you use allocs fixes:

```
cd /home/sdtd/engine/Data/
```

Now clone the repository, switch to the repository and pull for current master

```
git clone https://github.com/Devidian/OmegaTweak.git OmegaTweak
cd OmegaTweak
git pull
```

Last step is to copy all files to your Config dir with (-R to override existing files)

```
cp -R ./* ../Config/
```

To update, just pull the repository again and copy all files over to the Config directory.

### Windows DS or Client (All OS)
just download the files from github and copy them to your Config folder
