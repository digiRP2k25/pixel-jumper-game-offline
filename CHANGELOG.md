# Changelog

All notable changes to Pixel Jumper.

## [v1.4] – 2026-11-02 · Mobile full-screen edition

First public release. It includes everything built since the v2.0 prototype.

### Mobile and full screen
- The game fills the whole screen in any orientation, and wider screens show more of the track.
- On Android, the first tap switches to full screen and landscape. The ⛶ button (or `F` key) turns full screen on and off.
- The score, buttons, and ball stay clear of phone notches and rounded corners.
- Swipe down to drop fast (the touch version of the `↓` key).
- Multi-touch is handled, so lifting one finger doesn't cut a held jump short.
- Pinch-zoom, double-tap zoom, and pull-to-refresh are blocked during play.
- The screen stays awake while playing, and the phone gives a short vibration on crash (where supported).
- The game pauses when you rotate the phone mid-run.
- The start and game-over screens show your best and last 5 scores.

### Gameplay
- **Hold to jump higher:** a tap gives a small hop (~50 px) and a hold gives a big jump (~140 px).
- **Jump buffering:** a jump pressed just before landing still counts.
- **New obstacles:** tall, double, triple, and flying obstacles, added gradually as your score rises.
- **Fair spacing:** obstacles are always spaced so they can be cleared.
- **Smoother speed-up:** speed rises smoothly from 5 to 12.
- **Forgiving hitbox:** the collision area is slightly smaller than the ball.

### Look and sound
- **Day/night cycle** every 2,000 points, with stars and a moon.
- **Scenery:** moving hills, clouds, and road markings.
- **Ball animation:** the ball rolls, squashes on landing, and casts a shadow.
- **Effects:** dust puffs, a crash burst, a screen shake, and a flashing score every 500 points.
- **Sound effects** generated in code (no audio files), with a mute toggle.
- **Sharp graphics** on high-resolution screens.

### Offline and fixes
- Removed the Google Fonts dependency, so the game works fully offline.
- Best score, last 5 scores, and mute setting are saved between visits.
- Fixed: the game ran faster on 120/144 Hz screens (it now uses a fixed timestep).
- Fixed: one crash could record the score twice.
- Fixed: an accidental tap could restart the game instantly after Game Over.
- Auto-pause when switching tabs or apps; added pause and mute buttons.

## Development history (pre-release prototypes)

- **v2.0:** split-block obstacles, last 5 scores list, max speed 12.
- **v1.2:** red ball player with a 3D shine, obstacle colors that match the player, speed cap.
- **v1.0:** first playable version: blue block player, red obstacles, Space/tap to jump.
