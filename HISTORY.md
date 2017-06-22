## v16.0.e (merge version, experimental)
* restored changes to blocks.xml made in previous versions
  * drop fall events
  * pew segmet repair values
* restored entitygroups zombie group
  * removed deleted zombie types
  * need to add A16 zombies (done!)
* restored entityclasses.xml changes
  * all timer changes
* restored all changes from spawning.xml
* restored all Omega recipes in recipes.xml
  * note: jail door is now vanilla recipe
* restored OmegaTweak perks
  * due to changes, there is now only one crafting-perfectionist perk but requieres all craftSkill* on a certain level and player level 140+
* restored Localisation.txt changes
* restored items.xml changes
### Changes to items.xml
* schematicMaster.Stacknumber changed from 1 to 10 (schematics are books, why can't we stack those?)
### Changes to blocks.xml
* keystoneBlock.Fall changed to keystoneBlock (from destroyed stone)
  * Note: Would be better if the owner could pick it up instead, but that seems not to work, there is aldready a TakeDelay(30) defined

## v15.2.1
* merged A15.2 experimental changes

## v15.1.2

### Changes to items.xml
* Adjusted stack numbers of build materials according to others:
  * cobblestones 1000 -> 5000
  * concreteMix 1000 -> 5000
  * cement 1000 -> 3000

## v15.1.1
* changed versioning
* merged A15.1 experimental changes

## v15.0.3

### Changes to blocks.xml
* new Drop-Fall event paths (no magic disappearance of material)
  * Stone->destroyedStone->Gravel->sandStone->sand->sand
  * (type)Ore->(type)Ore 
  * grass -> dirt
  * dirt -> dirt
  * fertileFarmland -> fertileDirt
  * sod -> sod
* added repair items (wood) for pew segments

### Changes to entitygroups.xml
* added new group with all +special zombies

### Changes to spawning.xml
* changed last entry for screamer horde (*) to spawn zombies from special zombies group

### Changes to recipes.xml
* changed book recipe to use 1 leather instead of 1 wood
* changed book stack to 100, fuel and weight to 64
* added jailDoor recipe (workbench)
* added commercialDoor1, 2 & 4 recipe (workbench)
* added emberpile1 & 2 recipe
* added pew segments recipes
* added miningHelmet recipe with footballHelmetZU

### Changes to items.xml
* uncommented book
* added buffs to player hand (id 70)
  * 5% chance to buff bleeding
  * 30% chance to stun
* added actionXp (5) to player hand action0 (Fistfight ActionGroup)
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


### Changes to progression.xml
* New Action Skill: Machetes Training
  * Bonus 2: EntityDamage up to 1.28 (Level 100) and 1.40 (level 200)
* Added Machetes Training as requirement for knife guy and decapitator until we have something similar
* Changed xp of fistfight and machete training to 125 (from 100) to rebalance

## v15.0.2

### Changes to recipes.xml
* added book recipe for 64 paper + 1 wood (caseing)
* added paper recipe from book (1 book = 64 paper)
* added crushedSand recipe (18 sand from 1 destroyed stone)
* added machete repair recipe (1 machete 2 repair kit 5 forgedSteel)

### Changes to progression.xml
* Raised player level from 200 to 1000
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

### Changes to Localisation.txt
* Localisation for all perfectionist perks (german & english only yet)

## v15.0.1

### Changes to entityclasses.xml

* Map Icon for Minibikes activated
* Backpack lifetime raised from 20 Minutes to 60 Minutes
* (UMA)Zombie/Hornet corpse lifetime raised from 30(45) to 60 seconds
  * Note: corpse still exist after rotting, no time to set(change) there currently
* Dog & Animal corpse lifetime raised from 300 to 900 seconds (15 Minutes)


### Changes to progression.xml
* New Perk: Geologist with 2 level each 20 Skillpoints
  * Requirements: Player level 50, Miner 69er level 5, Mining Tools level 100
  * Level 1: 10% Block Damage,  5% harvest count
  * Level 2: 20% Block Damage, 10% harvest count (With this one you can one-hit stone again)
* New Action Skill: Fistfight
  * Bonus 1: StaminaDegradation down to 0.66 (level 100)
  * Bonus 2: EntityDamage up to 1.28

### Changes to items.xml
* Added Fistfight as Action0 group for player hand

### Changes to Localisation.txt
* Localisation for Geologist Perk
* Localisation for fistfight (german & english only yet)