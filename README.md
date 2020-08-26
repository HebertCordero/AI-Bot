# Vindinium-Bot

Vindinium is a multi-player turn based dungeon crawling game. Each player has one hero that can move across a map. The objective is for players to amass the maximum quantity of gold during a predetermined number of turns.

Four legendary heroes were fighting for the land of Vindinium

Making their way in the dangerous woods

Slashing goblins and stealing gold mines

And looking for a tavern where to drink their gold

![alt text](http://rwdc2.com/files/forest.png)

As of today the main Arena site is down so i will be working on making a local arena to test the bot.

Each player sends comands via POSTS to the site and each bot executes the commands as turns, GETs can also be used to receive the current state of the game.
Map layout, Gold, Player Positions, Health, ACTION [ATTACK, WAIT, MOVE [N,S,E,W][UP,DOWN,LEFT,RIGHT] ]

## The Code
This code uses Node.js to make the AI Logic, The bot should focus on finding the mines and aquiring GoldPerTurn, while staying away from other bots specially if the health is slow.

## Installation

1. Download the project.
2. cd js folder.
3. npm install to install dependencies.
```node
npm install
```

## Usage

| Command | Name | Explanation |
|:---:|:---:|:---:|
| -a | ARENA MODE | This will enlist you in a PVP match against other real bots. |
| -t | TRAINING MODE | This will queue your bot in a TRAINING MODE battle against basic bots. |
| num games | Number of games to play | min 1 |
| config | config.json | This loads your api key that will be used to play. |

```node
node bot.js <-a|-t> <num games> <config>
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
