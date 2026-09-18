# Differences from Phira

Phira-Vrenxz is a fork of [Phira](https://github.com/TeamFlos/phira). The chart standard, judgement and core gameplay are unchanged; the work went into the UI and a set of things you can adjust yourself. The list below is grouped by area.

> The current release is 1.3.2 (2026-09-16). Anything marked **unreleased** exists only in the source tree (some of it is not even committed) and has **not shipped in any release**, so a downloaded build will not have it; build from source to use it, see the [build guide](../phira_build_guide/index.md).

## Interface

- UI scale: menus, fonts and touch areas scale together, the background does not
- Profile page restyled in a parallelogram style, shadows removed
- Card-based menus and lists
- Pause screen reworked
- New "Custom" section in settings: UI position, home UI offset, accent colour and more
- "Legacy home mode": switch back to the old home background and music
- Score display on by default, off on low resolution to save performance

These four are **unreleased**:

- A choice of built-in home backgrounds: `background.jpg`, `bg1.png`, `bg2.png`, `bg3.png` and `background_old.jpg` (the images are in the repo, the picker is not built yet)
- Full-screen adaptation: window ratios from 21:9 to 9:16 (16:10, 4:3 and portrait included) share one layout
- The loading screen was re-animated: the background slides in from the right, the panel fades in offset to the left, the cover fades in; pressing start fires a full-screen white flash that sits on top and fades out once the slide finishes
- The start button on the song select screen is now a white parallelogram, cut flat on the right and flush with the screen edge; its icon is scaled down proportionally and dims while held

## Multiplayer

This section describes the multiplayer flow in the source tree, which is **unreleased** and has to be built from source.

- A built-in Phira-MP client: room list and room codes, host chart picking, ready-up, in-room chat, and self-hosted servers
- No spectating and no results screen: a match ends straight back in the room, where you can queue another one
- The room-selection (lobby) page was rebuilt, its stat blocks following the parallelogram style of `ending.rs`
- The connect page keeps only two buttons: connect and back to home
- The pause / resume countdown is back to 3 seconds

### Room page

- The score cards lost their black-and-white gradient background
- The grade slot shows the real grade (F / C / B / A / S / V)
- The start button is greyed out and disabled instead of being hidden when the conditions are not met
- Picking a chart starts downloading / syncing it in the background right away
- The buttons at the end of the top bar are laid out by text width
- The bold black line on the right is gone, and the bright end of the bottom-right gradient is brighter

## Charts

- Export supports the .pez format
- Batch chart download
- Bundled charts
- Fixed a crash in the chart library

## Input and judgement

- Replaced the system input box with an in-game one
- Fixed copy and paste in the input box
- Fixed drag / flick keyboard judgement and stuck keys with IMEs

This one is **unreleased**:

- Flick matches Phira: it is no longer "pre-judged" into a free Perfect before you actually swipe, and the late-press protection was added

## First-run wizard

This section describes the first-run flow in the source tree, which is **unreleased** and has to be built from source.

- A new first-run wizard walks through language, sign-in, volume, other settings and a final confirmation before the game reaches the main screen; its layout sits to the right
- The last step asks whether to play the tutorial; every step can be skipped forward, and you can get into the game without an account
- Returning players do not see it again: if the data already has a chosen language (`has_chosen_language`), the wizard counts as done

## Other

- Fixed crashes with video playback and unlock animations
- Bundled XC-SIM (requires sign-in)
- Removed the console window on Windows
- Android packages are provided since v1.3.0

This one is **unreleased**:

- Legacy data sync: on startup the game looks for an old PhirLie / Phira-Vrenxz data folder and offers to sync it. The prompt only appears once; afterwards use **Settings → Storage → Sync legacy data**

## Release notes

What changed in each version: [Release notes](./changelog.md).
