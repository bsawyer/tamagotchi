# Tamagotchi

An html game inspired by [Tamagotchi](https://en.wikipedia.org/wiki/Tamagotchi) the handheld digital pet

## Development

### Setup

Install dev dependencies

```
~ npm i
```

### Figma

The [figma designs](https://www.figma.com/file/l7scjUYTK6q8G982lRL8ct/tamagotchi-clone?type=design&mode=design&t=KqeiXNbpnqQO5XIt-1) are consolidated into a single page called "Rig"

Within the page, groups follow a naming convention to encapsulate what svg shapes will be animated with css e.g.

> with the group name
`rigHands:armatures:rotate`
all the child shapes of this group can be targeted for animating with the css selector `.armature-right-hand.armature-rotate`

The page is exported from Figma to `assets/rigFull.svg` and then converted to `docs/svg.js` by running

```
~ node ./scripts/pack.js
```

### Game

The game script is in `docs/script.js` and can played by opening `docs/index.html` in a browser

To see live stats append `?debug` to the url