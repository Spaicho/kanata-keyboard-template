# Kanata Remapping — Quick README

## Overview
This layout adds home-row modifiers, a navigation layer on Caps / `'`, and convenient editing keys on Alt and Caps.

---

## Links
- **Using Kanata to remap any keyboard:**  
  https://shom.dev/start/using-kanata-to-remap-any-keyboard  
  Blog post explaining practical Kanata remapping techniques.

- **Kanata key reference (mod.rs):**  
  https://github.com/jtroo/kanata/blob/main/parser/src/keys/mod.rs  
  Full list of internal key codes supported by Kanata.

- **Keyviz** *(optional)*:  
  https://github.com/mulaRahul/keyviz  
  A live key-press visualizer — useful for seeing keystrokes in real time and memorizing your new layout.

- **QWERTY-FR keyboard layout** *(optional, for French users)*:  
  https://github.com/qwerty-fr/qwerty-fr  
  A QWERTY-based layout optimized for French typing.

---

## Main Changes

### Home-row modifiers
`asdf jkl;` → **hold = modifiers**
- **a** = Win  
- **s** = Alt  
- **d** = Shift  
- **f** = Ctrl  
- **j** = Ctrl  
- **k** = Shift  
- **l** = Alt  
- **;** = Win  

---

### Caps / Apostrophe navigation layer
Hold **Caps** or **'**:
- **i j k l** → Arrow keys  
- **t = Home**, **y = PgUp**  
- **g = End**, **h = PgDn**

---

### Editing keys
- **Caps tap = Return**  
- **Left Alt tap = Backspace** (hold = Alt)  
- **Right Alt tap = Delete** (hold = Right Alt)

---

## Notes
- Grave → Esc remap is disabled for now.  
- Modifier order matters:
