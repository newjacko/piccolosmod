# Piccolo’s Agario Modded 3.2 🕹️  
_Agar.io, re‑imagined by **𝓝𝑒ⓦ 𝓙ⓐ¢K** after 10 years_

![Banner](https://i.ibb.co/zWcCmyf/pm3.gif)

> **Piccolo’s Mod** is an all‑in‑one Tampermonkey userscript that turbo‑charges Agar.io with advanced controls, automation, a full UI overlay, custom/ enemy skins, quality‑of‑life patches, ad‑blocking and much more — no external servers, no pay‑walls, 100 % open‑source.

---

## Table of Contents
1. [Features](#features)
2. [Quick Install](#quick-install)
3. [Controls & Hotkeys](#controls--hotkeys)
4. [UI Guide](#ui-guide)
5. [Configuration File](#configuration-file)
6. [FAQ](#faq)
7. [Contributing](#contributing)
8. [License](#license)
9. [Credits & Thanks](#credits--thanks)

---

## Features
| Category | Highlights |
|----------|------------|
| **Gameplay** | • Macro feed<br>• Double/Triple/Quad & Vertical quad split<br>• Hybrid Pause/Freeze (locks view _and_ blocks packets)<br>• Straight‑line mode for precision sniping |
| **Automation** | • Auto‑respawn (skip stats)<br>• Auto coin collector (polling + timer decode)<br>• Automatic potion opener & runner |
| **Visuals** | • Acid mode toggle<br>• Dark/Light theme switch<br>• Minimap with optional enemy dots<br>• Built‑in FPS counter & unlimited FPS option |
| **Skins** | • Drag‑n‑drop skin uploader (works in editor)<br>• Saved skin gallery (21 slots)<br>• Enemy‑skin mapping + “Apply all”<br>• One‑click named‑skin & emoji clipboard |
| **UI Overlay** | • Floating “Show Controls” widget<br>• Modular settings window (hotkeys, options, skins, player data)<br>• Player‑data manager with leaderboard, cell‑names & score export |
| **QoL Patches** | • 50‑character nickname limit restored<br>• Russia→Ukraine easter‑egg<br>• Promo banner replacer + ad/TOS scrubber |
| **Dev Goodies** | • Fully persisted config via `localStorage`<br>• Function‑index header for easy navigation (see `NEW NOTES` block) |

---

## Quick Install
1. **Browser**: Chrome / Opera (pause‑freeze may misbehave on Edge).  
2. **Extension**: [Tampermonkey](https://www.tampermonkey.net/) 4.19 +.  
3. **Script**:  
   *Click the link — Tampermonkey will prompt you to install/upgrade:*

```text
https://update.greasyfork.org/scripts/531449/Piccolo%27s%20Agario%20Mod.user.js
The script auto‑updates thanks to the @downloadURL / @updateURL headers.
To disable updates, open Tampermonkey ▸ ⚙ Config ▸ “Check for updates”.

Controls & Hotkeys

Action	Default
Toggle UI Overlay	H
Macro Feed	M (hold) / Left‑Mouse<sup>★</sup>
Single Feed	W / configurable
2× / 3× / 4× Split	D / T / Q
Vertical Quad Split	U
Vertical Line Aim	V
Pause / Freeze	P
Skin Switcher popup	S
<sup>★ Mouse bindings (left/ middle/ right) are fully remappable inside the overlay.</sup>

UI Guide
Controls Button ‑ fixed top‑left. Opens or hides the main overlay.

Main Overlay

Mouse Actions & Skins – remap clicks, copy named skins or emojis.

Hotkeys – click any key‑cell, then tap a new key.

Game Options – sliders: Acid‑mode, FPS‑cap, Minimap, Theme, etc.

Player Data & Skins – jump into the data/skin manager.

Player Data Manager
Tabs: Leaderboard, Cell Names, Your Score.
Right pane: “Your Skin” uploader and Enemy Skins mapper.

Skin Sites Popup – extra tabs: current/OG skins, Ur Skins gallery.

(Screenshots live in /docs folder of this repo.)

Configuration File
All settings persist in localStorage under the key piccolosmod.
Feel free to export/import that blob between browsers or tweak defaults in‑code (see defaultConfig{…}).

FAQ
<details> <summary>Why does pause/freeze sometimes drift?</summary>
Edge/Vivaldi throttle requestAnimationFrame when the tab is unfocused.
Use Chrome/Opera or disable Packet Freeze in NEW NOTES → PAUSE SYSTEM.

</details> <details> <summary>Custom skin isn’t loading!</summary>
Make sure the host URL supports CORS or use an image CDN (e.g. ibB.co).

Check that the image is ≤ 1 MB and square-ish (512 × 512 works great).

</details> <details> <summary>How do I restore my original Agar.io skin?</summary>
Open Your Skin tab → click Clear → Reload page.
captureOriginalSkin() stores it on first run.

</details>
Contributing
Pull‑requests are welcome!
If you add a new module, please:

Append the function(s) to the NEW NOTES – FUNCTION INDEX block.

Keep UI colours from COLORS{} or config.agarioColors{} for consistency.

Stick to ES 2019 syntax (no top‑level await, optional‑chaining is OK).

Test on Chrome 124+ and Tampermonkey 4.19.

License
MIT – do whatever, just leave the header comments intact.

Credits & Thanks
imsolo.pro/web – UI inspiration & helper snippets.

legendmod.ml – original chat/private‑server tricks.

@BeeChasnyAgario – first code drop that started it all.

@maroooc – promo art & endless ideas.

The entire Agar.io community – keep the arena alive!

💬 Questions or new ideas? Find me on Discord: new_jack_9999
