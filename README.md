# manubank
Remake of Westbank (sinclair spectrum 1987) v0.91

Play me in http://www.quercusdata.com/manubank/

## Run locally

The game uses ES modules, so it must be served over HTTP (opening `index.html` directly from disk does not work):

```
npm start
```

## Project structure

```
js/
  main.js              Entry point
  config.js            Timing (doors and characters reaction times) and gameplay rules
  constants.js         Enums (game modes, door states, indicator states...)
  layout.js            Canvas size and screen positions
  assets.js            Images and sounds
  engine/              Game loop, input and renderer
  game/Game.js         Screens, score, lives, levels and pauses
  game/DoorSlot.js     Door state machine
  game/actors/         Lady, SlowBandit, Hatter and TallCustomer
```
