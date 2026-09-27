# Castles Reforged

A browser remake of **Castles v1.5** (Crazy Mice, 2001), the turn-based artillery game where up to five castle lords try to knock each other's walls down.

It is one `index.html` with no build step and no dependencies beyond Google Fonts. The painted castle lives in `assets/castle.png`; if that file is missing, or the page is opened straight from disk (browsers will not let a page read image pixels from `file://`), the game falls back to a castle drawn in code. Serve the folder to see the painted one.

## Play locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

## Deploy on Render

This repo includes a `render.yaml` Blueprint for a free static site.

1. In the Render dashboard choose **New → Blueprint** and pick this repository.
2. Render reads `render.yaml`, creates the `castles-reforged` static site and publishes the repo root.
3. Every push to the main branch redeploys automatically.

## What's in the game

- 2 to 5 lords, each a player on this device or a computer opponent (Squire, Knight or Warlord).
- The original ten weapons: Arrow, Big Arrow, Grenade, Super Grenade, Direct Missile, Balloon, Defense, Ground Defense, Ball Grenade and Gimlet.
- Seven extras in the spirit of the registered edition: Cannonball, Fire Pot, Sapper Charge, Rock Rain, War Falcon, Earthquake and Storm Bolt.
- Castle upgrades, falling gift crates, wind, ground that gets blown away, and an armory between rounds.
- A battlefield twice the screen width, with panning and a minimap.

## Controls

| Action | Keys / mouse |
|---|---|
| Turn the sight | Tap or right-click the field to point at that spot, the angle slider and ◀ ▶ buttons, or `←` `→` (hold `Shift` for big steps) |
| Set power | The power slider and − + buttons, `↑` `↓`, or hold `Space` to charge and let go to fire |
| Fire at the set power | `Enter` or the Fire button |
| Slingshot aim | Drag back from your own castle and let go |
| Look around | Drag the field, use the scroll wheel, or click the minimap |
| Pick a weapon | `1`–`0` for the original ten, `Q` / `E` to cycle |
| Pause / mute | `P` or `Esc` / `M` |

There is no turn timer, so take your time.

There are also two secret weapons for human players. Old-school players know to try typing the name of one of them. On a phone, the pause menu has a box for codes.

## Credits

The original *Castles* was made by Crazy Mice in 2000–2001. This is a fan remake written from scratch. It contains none of the original game's code, graphics or sound.
