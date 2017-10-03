# The Radar Script

## About

> The Radar Script is a radar script, that looks, and feels like DOJ's. It doesn't have a menu, and it doesn't have anything complicated with it!

## How to use

* `G` to open and close the RADAR
* `X` to freeze the radar
* `PGUP` to change the fast speed up
* `PGDOWN` to change the fast speed down

## Uses

Uses for this script, is for roleplay reasons only. I made this script for roleplay in mind, and also for DOJ's radar script in mind. I think I made a great representation of DOJ's.

Used for spotting the speed on all passing cars, and then it reads it back to you with 2 decimal precision.

## Pros N Cons

### PROS

* Working fine without lag
* Easy to install and use
* Just works
* Comes with a built in whitelist
* Many settings to choose from

### CONS

* Doesn't inlude a menu like DOJ's
* Isn't exactly like DOJ's
* Takes up a lot of space on the screen

## Pictures

> Coming soon!

## Changing the Settings

Everything at the top of the file, before `THE LINE`, is considered a setting, and can be changed. The settings should look something like this:

```lua
local settings = {
	minSpeed = 2.0, -- will not count vehicle if under this speed
	drawDistance = 125.0, -- how far the radar will look for cars ahead of it
	speedInKmh = false, -- If enabled, then it will display speed in KMH, otherwise, MPH
	playSound = true, -- Plays a sound if the car in front go above the fast speed limit
	speedInterval = 5.0 -- Amount that the fast speed changed when you change it in game
}
local whitelist = {
	vehs = { -- make sure these are upper, and have quotes
		"POLICE",
		"POLICE2",
		"POLICE3",
		"POLICE4",
		"SHERIFF",
		"SHERIFF2",
		"FBI",
		"FBI2",
		"RIOT",
		"POLICEB",
	},
	enable = false -- if enabled, then will check if the vehicle that the player is driving is the same as one of above
}
```

Let's say that you want to change the minSpeed Variable, you would change it from this:

```lua
    minSpeed = 2.0
```

to 

```lua
    minSpeed = 5.0
```

### Keep in mind

Keep in mind that all of the variables that end with a `.0` have to always end with a `.0`, or else the script will not work and it will crash on ya!