# SpaceQix

A free, original neon territory-capture game with a head nod to the classic 80s arcade line-drawing game. You steer a marker along the edge of a glowing field, cut lines across it to claim ground, and reveal a hidden picture as you go, while a chaotic prowler hunts your unfinished line and crawlers patrol the edges.

**Play it in your browser:** https://nbwillcox.github.io/SpaceQix/

Everything is generated in code: the eight hidden pictures, the prowlers and all the sound effects are drawn and synthesized on the fly. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpacePac](https://github.com/nbwillcox/SpacePac), [SpaceTube](https://github.com/nbwillcox/SpaceTube) and the rest of the series.

## Controls

| Action | Keys |
| --- | --- |
| Move | `←` `↑` `↓` `→` or `W` `A` `S` `D` (or a gamepad d-pad / stick) |
| Slow draw (hold as you leave the edge) | `Shift` or `Space` |
| Pause | `P` or `Esc` |

You move while a direction is held. Pushing into the open field starts a line, and the line ends when you reach an edge again.

### On a phone or tablet

Play in portrait. A floating stick on the lower left moves the marker (it moves while the stick is pushed), and holding **SLOW** as you leave the edge draws a slower line worth double. The pause button opens the menu. The on-screen controls appear on touch devices automatically; Settings has size, opacity and a left-handed layout. Use your browser's *Add to Home Screen* to install it as a full-screen app.

## Gameplay

- **Claim the field:** draw a line from one edge to another. The piece of the field **without the prowler** in it becomes yours and reveals part of that level's hidden picture. Claim the level's target percentage (65% on level 1, rising to 80%) to clear it.
- **The prowler** is a chaotic line that roams the open field. If it touches your unfinished line, you lose a life and the line is wiped.
- **Crawlers** patrol the edges and chase you along them. Enclose one in claimed ground and it is destroyed.
- **The fuse:** if you stop in the middle of a line for too long, a fuse lights at the start of your line and burns toward you. Keep moving, or finish the line.
- **Slow draw:** hold SLOW as you leave the edge to draw at half speed for **double points**, and the ground you claim is revealed in full brightness. The prowler can strike a slow line more easily, so choose your moments.
- **Power-ups** sit in the open field and are collected when you claim the ground they are on: **F** freezes every enemy, **H** is a shield, **S** is a speed boost, **B** is a bomb that destroys the crawlers, and **1UP**.
- **Bosses** appear on every fifth level: The Weaver, The Prism and The Hydra. The boss prowler is bigger, has three lines and fires bolts that hunt your unfinished line. You need 75% to beat it.
- **Lives and score:** 3 lives, an extra life every 20,000 points. Big claims earn a bonus. Local top-10 high scores are kept in your browser.

## Run it locally

Open `index.html` in a browser, or serve the folder with any static server, for example `python -m http.server`. Test flags: `?level=N` starts on level N, `?god=1` makes you immune, `?touch=1` forces the touch controls on a desktop.

## License

[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix for non-commercial use, with a link back to https://github.com/nbwillcox/SpaceQix. SpaceQix is an original game inspired by the arcade golden age; it uses no art, sounds or code from any commercial game.
