# Ghauntlet (web build)

A Halloween dungeon crawler in the spirit of Gauntlet Legends: 1-4 kids in
costumes that took, fighting through crypts full of ghouls. Candy is life and
it keeps running out. Five realms with a boss at the bottom of each, the
Endless Crypt, the Daily Descent, Horde Night, Candy Clash and Boss Rush;
solo with bot friends, couch co-op, or online rooms through the Wayside
relay. Made in Godot 4.6; this is the browser build, also a cart in the
Wayside Station arcade.

One page, two packs: phones and tablets load `index.mobile.pck` (lighter
graphics, fewer music tracks), desktop browsers `index.pck`.
`?pack=mobile|desktop` forces one; `?room=CODE` opens a friend's online room.
When an Endless Crypt run ends (out of souls, or quit after floor 1) the game
posts `{type: "PLAYER_DIED", score}` (the last floor's score) to the page
around it.

This repo holds only the exported files; the game's source lives elsewhere
and publishes here with its `tools/publish_web.sh`.
