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

## Notes
- Grave -> Esc remap is disabled.
- For arrow chords, press modifier before layer key if you hit ordering issues.
