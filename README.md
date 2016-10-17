# OmegaTweak
## 7 Days to die Tweaks by Devidian

### Changes to entityclasses.xml

* Map Icon for Minibikes activated
* Backpack lifetime raised from 20 Minutes to 60 Minutes

### Changes to progression.xml
* New Perk: Geologist with 2 level each 20 Skillpoints
 * Requirements: Player Level 50, Miner 69er Level 5, Mining Tools Level 100
 * Level 1: 10% Block Damage,  5% harvest count
 * Level 2: 20% Block Damage, 10% harvest count (With this one you can one-hit stone again)

### Changes to Localisation.txt
* Localisation for Geologist Perk (Desc for french/spanish missing)

## Installation & Update Information
The current master is ONLY for Alpha 15, dont try to use with a lower Alpha version.
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
