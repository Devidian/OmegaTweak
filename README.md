# OmegaTweak v16.1.2
## 7 Days to die Tweaks by Devidian

### Changes to blocks.xml
* new Drop-Fall event paths (no magic disappearance of material)
  + Stone->destroyedStone->Gravel->sandStone->sand->sand
  + (type)Ore->(type)Ore 
  + grass -> dirt
  + dirt -> dirt
  + fertileFarmland -> fertileDirt
  + sod -> sod
  + clay -> clay
  + keystone -> keystone
* added repair items (wood) for pew segments

### Changes to recipes.xml
* added book recipe for 64 paper + 1 leather (caseing)
* added paper recipe from book (1 book = 64 paper)
* added crushedSand recipe (18 sand from 1 destroyed stone)
* added machete repair recipe (1 machete 2 repair kit 5 forgedSteel)
* added commercialDoor1, 2 & 4 recipe (workbench)
* added emberpile1 & 2 recipe
* added pew segments recipes
* added miningHelmet recipe with footballHelmetZU

### Changes to entityclasses.xml
* Backpack lifetime raised from 20 Minutes to 60 Minutes
* (UMA)Zombie corpse lifetime raised from 30(45) to 60 seconds
  + Note: corpse still exist after rotting, no time to set(change) there currently
* Dog & Animal corpse lifetime raised from 300 to 900 seconds (15 Minutes)

### Changes to progression.xml
* Raised player level from 200 to 1000
* recalculated level progression, now cumulative xp is 5 times more (11MXP->55MPX) for 5 times more level.
* level 200 vanilla means level 530 now, rest to 1000 will progress slower.
* Skillpoints per level lowered to 3, means vanilla skill points (1200) is reached at level 400 which is faster than level 200 before.
* New Action Skill: Fistfight
  + Bonus 1: StaminaDegradation down to 0.66 (Level 100)
  + Bonus 2: EntityDamage up to 1.28
* New Action Skill: Machetes Training
  + Merged perks "Knife Guy" and "The Decapitator" into "Machetes Training", those wont have any further effect on machetes now
  + EntityDamage from "Knife Guy" recalculated with "Machetes Training" origin values - may be rebalanced in future
* New Perk: Geologist with 2 level each 20 Skillpoints
  + Requirements: Player Level 50, Miner 69er Level 5, Mining Tools Level 100
  + Level 1: 10% Block Damage,  5% harvest count
  + Level 2: 20% Block Damage, 10% harvest count (With this one you can one-hit stone again)
* New Perk: Crafting-Perfectionist with 5 level each 20*1.15 Skillpoints
  + Requirements: Player level 140,150,165,180,200 all craftSkill* level 2,4, 6,8,10
  + Level 1-5: 20-100 Quality points added

### Changes to items.xml
* added Fistfight as Action0 group for player hand (id 70)
  + added actionXp (5)
  + added buffs to player hand
    - 5% chance to buff bleeding
    - 30% chance to stun
* uncommented book, changed stack to 100, fuel and weight to 64
* Added "Machetes Training" as ActionSkillGroup for machete
* ~~changed machete repairMaterial to forgedSteel~~ (since A16e.b129 machete is steel)
* Adjusted stack numbers:
  + scrapIron 6000 -> 30000 (what fits in forge)
  + scrapBrass 6000 -> 30000
  + scrapLead 6000 -> 30000
  + ironFragment 1200 -> 3000 (->15000 Scrap iron,2 of it fit in forge)
  + crushedSand 6000 -> 15000 (reduced weight from 5 to 2)
  + forgeCrucible 1 -> 3
  + toolAndDieSet 1 -> 5
  + cobblestones 1000 -> 5000
  + concreteMix 1000 -> 5000
  + cement 1000 -> 3000
* added Admin-Hazmat-Suit with full protection

### Changes to Localisation.txt
* Localisation for Geologist perk
* Localisation for fistfight (german & english only yet)
* Localisation for perfectionist perk (german & english only yet)
* Admin-Hazmat-Suit localisation added

### Changes to entitygroups.xml
* added new group with all +special zombies (ToDo: Balancing)

### Changes to spawning.xml
* changed last entry for screamer horde to spawn zombies from special zombies group too

## Installation & Update Information
The current master is ONLY for Alpha 16, dont try to use with a lower Alpha version.
Lower versions are tagged

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
