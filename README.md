This is a set of scripts for use with the TinTin++ mud client on TorilMud.  Feel free to fork, copy or use any of this, or if you want to contribute, clone the project.  Currently these scripts are nothing but a framework to load appropriate files for your character, race, class, and class.

Functionality will be slowly introduced over time.

### Installation
* Either fork, download, or clone the scripts
* Edit the toril.tin file and your account name
```
#var my_account <your account>
```

To run, change directory to wherever you've installed the scripts and load the toril.tin file:
```
cd ~/mud/toril
tt++ toril.tin
```
The script will then connect to Torilmud, and enter the account name you supplied above.

After selecting a character to play the score command will be actioned and will attempt to load:
* a file in the characters folder matching the name of the character
* a file in the race folder matching the character's race
* a file in the class folder matching the character's class

As an example if you have a Bob, the Human Warrior the following files will attempt to be loaded:
```
./characters/Bob.tin
./races/Human.tin
./classes/Warrior.tin
```

Those files will in turn attempt to load a bunch of scripts specific to that character, race, and class, but the complexity of those files will be hidden.



