# Vaiduoklio Iškraustymas

First-person browser game: take your house back from a ghost with your fists.
Single file, `index.html` (Three.js from CDN).

**Play:** https://raugykla.github.io/vaiduoklis/

- Desktop: WASD move, mouse look, left click punch (hold to charge), Shift run, Q turn around, E use power-up, M mute
- Mobile: left side move, right side look, 👊 punch, ↻ turn around, item button to use power-up

All sound effects and the soundtrack are synthesized at runtime with the Web Audio API (no audio files). The music gets faster and adds instruments every level.

## Upgrades (meta progression)

Hurting the ghost earns 🟢 ectoplasm, which is kept after death and spent in the
upgrade tree (start / game-over screen → "Upgrade'ai"): 4 branches × 4 tiers
(10 / 25 / 50 / 90) plus Grandpa's Winchester (200, needs any 2 branches maxed).
Every upgrade has a visible in-game effect. Extra keys: F salt / holy water, R rifle.

Testing: open the game with `?ecto=500` to add ectoplasm, `?reset=1` to wipe upgrades.

## Versioning

Semantic versioning, one tag per commit: new features bump the minor version
(v1.1.0 → v1.2.0), bug fixes bump the patch (v1.2.0 → v1.2.1).
The version is shown in the bottom-right corner of the game — update
`<div id="version">` in `index.html` together with the tag.
