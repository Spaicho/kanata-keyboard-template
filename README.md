# Kanata Remapping - Quick README

## Overview
This layout adds home-row modifiers, two navigation layers (Caps and Tab), and editing shortcuts while keeping QWERTY-fr compatibility on Windows.

## Links
- Using Kanata to remap any keyboard: https://shom.dev/start/using-kanata-to-remap-any-keyboard
- Kanata key reference (mod.rs): https://github.com/jtroo/kanata/blob/main/parser/src/keys/mod.rs
- Keyviz (optional): https://github.com/mulaRahul/keyviz
- QWERTY-fr layout (optional): https://github.com/qwerty-fr/qwerty-fr

## Main Changes

### Home-row modifiers
`asdf jkl;` -> hold = modifiers
- `a` = Win
- `s` = Alt
- `d` = Shift
- `f` = Ctrl
- `j` = Ctrl
- `k` = Shift
- `l` = Alt
- `;` = Win

### Layer keys
- `Caps` tap = `Enter`, hold = `cap-mod`
- `'` tap = `'`, hold = `cap-mod`
- `Tab` tap = `Tab`, hold = `tab-mod`

### cap-mod (right-hand nav + history)
Hold `Caps` or `'`:
- `i j k l` -> `Up Left Down Right`
- `t` = `Home`, `y` = `PgUp`
- `g` = `End`, `h` = `PgDn`
- `e` = Back (`Alt+Left`)
- `r` = Forward (`Alt+Right`)
- `Space` = `Backspace`

### tab-mod (left-hand one-hand nav)
Hold `Tab`:
- `s d f e` -> `Left Down Right Up`

### Editing and modifier taps
- `Left Alt` tap = `Backspace`, hold = `Alt`
- `Right Alt` tap = `Delete`, hold = `Right Alt` (`AltGr`)
- `Left Shift` tap = `Esc`, hold = `Shift`

## Windows + QWERTY-fr note
`windows-altgr add-lctl-release` is enabled to avoid stuck `Left Ctrl` when using `AltGr` with QWERTY-fr on Windows.

## Strict training mode (`kanata-strict.kbd`)
Disables the original keys that have a remapped equivalent, to build the new habits.
Active at startup and after every reload (it is the first layer).

Disabled in strict mode, and what to use instead:
- Arrows -> hold `Caps` (or `'`) + `i j k l`, or hold `Tab` + `e s d f`
- `Home` / `End` -> hold `Caps` + `t` / `g`
- `PgUp` / `PgDn` -> hold `Caps` + `y` / `h`
- `Enter` -> tap `Caps`
- `Backspace` -> tap `Left Alt` (or hold `Caps` + `Space`)
- `Delete` -> tap `Right Alt`
- `Esc` -> tap `Left Shift`

Toggle strict / normal: hold `Caps`, tap `Esc`.

Tray icon (Windows GUI build, files in `icons/`):
- red `S` = strict, green `N` = normal, blue arrow = `cap-mod` / `tab-mod` held

Notes:
- Emergency exit: hold `Left Ctrl` + `Space` + `Esc` (kanata checks this before any remap).
- Kanata does not run on the sign-in / lock screen, in UAC prompts or in elevated (admin) windows: the original keys work there, the remaps do not.
- Software-typed input (e.g. KeePass auto-type) is not blocked: kanata ignores injected events.
- `strict` repeats the `default` remaps by alias name: keep both in sync when `default` changes.

## Notes
- Grave -> Esc remap is disabled.
- For arrow chords, press modifier before layer key if you hit ordering issues.
