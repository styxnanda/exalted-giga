<h1 align="center"><strong>Exalted Giga Crusader Kings III</strong></h1>
<p align="center">
  <img src="./exalted_giga/thumbnail.png" height="250"/>
</p>
<p align="center">
    Become a giga ruler by cheating your way through CK3 :sunglasses:
</p>

# WARNING

A NEW 2.0 VERSION IS THE LATEST RELEASE, BUT THE README ISN'T UP TO DATE YET!
As a heads up, this 2.0 version features an event that you can trigger from a decision called `Exalted Giga Menu`. Inside, you can choose from 4 cheats to use.
The old batch cheat (one button to add all stats) is still usable.

# What does this mod do?

This is a simple mod that adds the following to the player's ruler:

<center>

|   Item   |   Amount    |                        Icon                         |
| :------: | :---------: | :-------------------------------------------------: |
|   Gold   | `1,000,000` |   <img src="./images/icons/gold.png" width="40%">   |
|  Piety   | `1,000,000` |  <img src="./images/icons/piety.png" width="40%">   |
| Prestige | `1,000,000` | <img src="./images/icons/prestige.png" width="40%"> |
|  Renown  | `1,000,000` |  <img src="./images/icons/renown.png" width="40%">  |

</center>

# About Mod

This mod was tested on the 1.10.\* version of the game, but it should be compatible with any mods and should also be able to withstand future updates. I created this mod when I wanted to cruise my way through CK3 and dominate the world. It's pretty fun and way more convenient than having to type in the debug console per command.

There is a 30 days cooldown in-between the usage. If you want to change it, visit the section _[Changing modifier into custom values](#changing-modifier-into-custom-values)_.

# Installation

1. Move the `exalted_giga` folder and `exalted_giga.mod` file into your Crusader Kings 3 mods folder, usually located in `C:\Users\<your_name>\Documents\Paradox Interactive\Crusader Kings III\mod`

2. Load the mod into your playset via Paradox Launcher (when launching the game from Steam)

# Usage in-game

The cheat is accessible via the decision menu.

<p align="center">
    <img src="./images/Decision_Menu.png" width="50%"/>
</p>
<p align="center">
    <img src="./images/Choosing_Decision.png" width="40%"/>
</p>

# Changing modifier into custom values

To change the value from `1,000,000` to any custom values, edit the file `exalted_giga\common\decisions\my_decisions.txt` using any text editor (Notepad, Notepad++, VSCode, etc). Change the following numbers into any custom values.

```txt
effect = {
	add_gold = 1000000 # Change this value for gold modifier
	add_prestige = 1000000 # Change this value for prestige modifier
	add_piety = 1000000 # Change this value for piety modifier
	dynasty = {
		add_dynasty_prestige = 1000000 # Change this value for renown modifier
	}
}
```

You might want to do this if balancing is an issue. Furthermore, you can also change the cooldown duration (even disable it completely) by changing the following line in the same file:

```text
cooldown = { days = 30 }
```

If you want to disable cooldown, change it into:

```text
cooldown = { days = 0 }
```

Or you can also use months as counter:

```text
cooldown = { months = 6 }
```

Or year:

```text
cooldown = { year = 2 }
```
