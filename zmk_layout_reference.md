# Stenomi Keyboard Layout Reference

## Table of Contents
- [Quick Start](#quick-start)
- [Layer Overview](#layer-overview)
- [Key Position Map](#key-position-map)
- [Layer 0: Plover/Steno](#layer-0-ploversteno)
- [Layer 1: QWERTY](#layer-1-qwerty)
- [Layer 2: Symbol](#layer-2-symbol)
- [Layer 3: Number](#layer-3-number)
- [Layer 4: Function](#layer-4-function)
- [Combos Reference](#combos-reference)
- [Differences from QMK](#differences-from-qmk)
- [Tips and Tricks](#tips-and-tricks)

---

## Quick Start

### Default Mode
- **Boot into**: PLOVER layer (stenography mode)
- **Switch to typing**: Press top-left key to enter QWERTY mode
- **Switch back**: Press top-left key again

### Basic Navigation
```
PLOVER  ──► Press top-left key ──► QWERTY
QWERTY  ──► Press top-left key ──► PLOVER
```

---

## Layer Overview

| Layer | Name | Purpose | Access |
|-------|------|---------|--------|
| 0 | PLOVER | Stenography with Plover software | Default layer |
| 1 | QWERTY | Standard typing | Toggle from PLOVER |
| 2 | SYMBOL | Special characters & symbols | Hold bottom-left in any layer |
| 3 | NUMBER | Numbers & navigation | Hold left thumb in QWERTY |
| 4 | FUNCTION | F-keys & media controls | Hold right thumb in QWERTY |

---

## Key Position Map

Use this reference when creating combos or understanding key positions:

```
Physical Layout:
┌────┬────┬────┬────┬────┬────┐     ┌────┬────┬────┬────┬────┬────┐
│  0 │  1 │  2 │  3 │  4 │  5 │     │  6 │  7 │  8 │  9 │ 10 │ 11 │
├────┼────┼────┼────┼────┼────┤     ├────┼────┼────┼────┼────┼────┤
│ 12 │ 13 │ 14 │ 15 │ 16 │ 17 │     │ 18 │ 19 │ 20 │ 21 │ 22 │ 23 │
└────┴────┴────┼────┼────┼────┤     ├────┼────┼────┼────┴────┴────┘
               │ 24 │ 25 │ 26 │     │ 27 │ 28 │ 29 │
               └────┴────┴────┘     └────┴────┴────┘
```

---

## Layer 0: PLOVER/STENO

**Purpose**: Primary stenography layer for use with Plover software

```
┌──────────┬─────┬─────┬─────┬─────┬──────┐     ┌──────┬─────┬─────┬─────┬─────┬─────┐
│ ->QWERTY │  S  │  T  │  P  │  H  │ ST1  │     │ ST3  │  F  │  P  │  L  │  T  │  D  │
├──────────┼─────┼─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┼─────┼─────┤
│  SYMBOL  │  S  │  K  │  W  │  R  │ ST2  │     │ ST4  │  R  │  B  │  G  │  S  │  Z  │
└──────────┴─────┴─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┴─────┴─────┘
                        │  #  │  A  │  O   │     │  E   │  U  │  #  │
                        └─────┴─────┴──────┘     └──────┴─────┴─────┘
```

### Keys Explained

**Left Hand:**
- `S` - Left S key (two positions available)
- `T`, `P`, `H` - Left consonants
- `K`, `W`, `R` - Left consonants
- `ST1/ST2` - Star keys
- `#` - Number key (both sides)
- `A`, `O` - Left vowels

**Right Hand:**
- `F`, `P`, `L`, `T`, `D` - Right consonants (first row)
- `R`, `B`, `G`, `S`, `Z` - Right consonants (second row)
- `ST3/ST4` - Star keys
- `E`, `U` - Right vowels

### Usage
1. Ensure Plover is running with HID mode enabled
2. Press multiple keys simultaneously to form chords
3. Plover translates chords to words/commands
4. Bottom-left key (SYMBOL) provides momentary symbol layer access

---

## Layer 1: QWERTY

**Purpose**: Standard typing for when stenography isn't needed

```
┌──────────┬─────┬─────┬─────┬─────┬──────┐     ┌──────┬─────┬─────┬─────┬─────┬──────┐
│ ->PLOVER │  Q  │  W  │  E  │  R  │  T   │     │  Y   │  U  │  I  │  O  │  P  │ BSPC │
├──────────┼─────┼─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┼─────┼──────┤
│  SYMBOL  │  A  │  S  │  D  │  F  │  G   │     │  H   │  J  │  K  │  L  │  ;  │  '   │
└──────────┴─────┴─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┴─────┴──────┘
                        │ NUM │ SPC │SHIFT │     │ ENT  │ SPC │ FN  │
                        └─────┴─────┴──────┘     └──────┴─────┴─────┘
```

### Special Keys

**Top Row:**
- Standard QWERTY letters Q-P
- `BSPC` - Backspace (top-right)

**Home Row:**
- Standard home row A-L
- `;` - Semicolon
- `'` - Single quote

**Thumb Keys:**
- `NUM` - Hold for NUMBER layer
- `SPC` - Space (appears twice for convenience)
- `SHIFT` - Shift modifier
- `ENT` - Enter
- `FN` - Hold for FUNCTION layer

### Available Combos
See [QWERTY Combos](#qwerty-layer-combos) section for all combinations

---

## Layer 2: SYMBOL

**Purpose**: Access to all special characters and symbols (replaces QMK's PWR key combinations)

```
┌──────────┬─────┬─────┬─────┬─────┬──────┐     ┌──────┬─────┬─────┬─────┬─────┬──────┐
│          │  !  │  @  │  {  │  }  │  |   │     │  '   │  +  │  -  │  /  │  *  │ TAB  │
├──────────┼─────┼─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┼─────┼──────┤
│  -----   │  #  │  $  │  (  │  )  │  `   │     │  "   │  &  │  =  │  ,  │  .  │ ESC  │
└──────────┴─────┴─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┴─────┴──────┘
                        │     │     │      │     │  ;   │  \  │     │
                        └─────┴─────┴──────┘     └──────┴─────┴─────┘
```

### Symbol Map

**Top Row (Left to Right):**
- `!` - Exclamation
- `@` - At sign
- `{` - Left brace
- `}` - Right brace
- `|` - Pipe
- `'` - Single quote
- `+` - Plus
- `-` - Minus
- `/` - Forward slash
- `*` - Asterisk
- `TAB` - Tab key

**Home Row (Left to Right):**
- `#` - Hash/Pound
- `$` - Dollar sign
- `(` - Left parenthesis
- `)` - Right parenthesis
- `` ` `` - Backtick/Grave
- `"` - Double quote
- `&` - Ampersand
- `=` - Equals
- `,` - Comma
- `.` - Period
- `ESC` - Escape key

**Thumbs:**
- `;` - Semicolon
- `\` - Backslash

### QMK Equivalents
This layer replaces the QMK PWR key combinations:
- QMK: `PWR + LSU` = `!`  →  ZMK: Hold SYMBOL, press position 1
- QMK: `PWR + LP` = `{`   →  ZMK: Hold SYMBOL, press position 3
- QMK: `PWR + RF` = `+`   →  ZMK: Hold SYMBOL, press position 7

---

## Layer 3: NUMBER

**Purpose**: Quick access to numbers and navigation arrows

```
┌──────────┬─────┬─────┬─────┬─────┬──────┐     ┌──────┬─────┬─────┬─────┬─────┬──────┐
│          │  1  │  2  │  3  │  4  │  5   │     │  6   │  7  │  8  │  9  │  0  │ BSPC │
├──────────┼─────┼─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┼─────┼──────┤
│          │  [  │  ]  │  {  │  }  │  `   │     │  ←   │  ↓  │  ↑  │  →  │  ~  │ ESC  │
└──────────┴─────┴─────┼─────┼─────┼──────┤     ├──────┼─────┼─────┼─────┴─────┴──────┘
                        │ --- │     │      │     │ ENT  │ TAB │     │
                        └─────┴─────┴──────┘     └──────┴─────┴─────┘
```

### Number Row
- Left hand: `1 2 3 4 5`
- Right hand: `6 7 8 9 0`
- Far right: `BSPC` (Backspace)

### Home Row
**Left Hand (Brackets):**
- `[` - Left square bracket
- `]` - Right square bracket
- `{` - Left curly brace
- `}` - Right curly brace
- `` ` `` - Backtick

**Right Hand (Navigation):**
- `←` - Left arrow
- `↓` - Down arrow
- `↑` - Up arrow
- `→` - Right arrow
- `~` - Tilde
- `ESC` - Escape

### Thumb Keys
- Left: Hold to activate this layer
- Right: `ENT` (Enter), `TAB`

### Usage Tips
- Hold left thumb (NUM) to access this layer
- Perfect for entering numbers while typing
- Arrow keys are positioned for vim-style navigation (HJKL pattern)

---

## Layer 4: FUNCTION

**Purpose**: Function keys, media controls, and navigation

```
┌──────────┬──────┬──────┬──────┬──────┬──────┐     ┌──────┬──────┬──────┬──────┬──────┬──────┐
│          │  F1  │  F2  │  F3  │  F4  │  F5  │     │  F6  │  F7  │  F8  │  F9  │ F10  │ F11  │
├──────────┼──────┼──────┼──────┼──────┼──────┤     ├──────┼──────┼──────┼──────┼──────┼──────┤
│          │ PREV │ PLAY │ NEXT │ VOL- │ VOL+ │     │ PGUP │ PGDN │ HOME │ END  │ MUTE │ F12  │
└──────────┴──────┴──────┼──────┼──────┼──────┤     ├──────┼──────┼──────┼──────┴──────┴──────┘
                          │      │      │      │     │      │      │ ---  │
                          └──────┴──────┴──────┘     └──────┴──────┴──────┘
```

### Function Keys
**Top Row:**
- F1 through F11 across the top
- F12 on bottom right

### Media Controls
**Bottom Left:**
- `PREV` - Previous track
- `PLAY` - Play/Pause
- `NEXT` - Next track
- `VOL-` - Volume down
- `VOL+` - Volume up

### Navigation
**Bottom Right:**
- `PGUP` - Page up
- `PGDN` - Page down
- `HOME` - Home key
- `END` - End key
- `MUTE` - Mute audio

### Access
- Hold right thumb key (FN) from QWERTY layer
- Combines the QMK FUNCT and MEDIA layers

---

## Combos Reference

### What Are Combos?
Combos let you press multiple keys simultaneously to trigger special actions. They work like chords in stenography but for standard keys.

### System Combos (All Layers)

| Keys | Position | Action | Purpose |
|------|----------|--------|---------|
| Top-left + Top-right | `0 + 11` | `BT CLR` | Clear Bluetooth pairing |
| Second corners | `1 + 10` | `OUT TOGGLE` | Switch between USB/Bluetooth |

**Usage Example:**
```
Press both top corner keys simultaneously → Clears Bluetooth
Press both second-from-corner keys → Toggles USB/BT output
```

---

### QWERTY Layer Combos

#### Thumb Combos (Modifiers)

| Keys | Position | Output | QMK Equivalent |
|------|----------|--------|----------------|
| Left two thumbs | `24 + 25` | `Ctrl` | `P( LNO | LA, SEND(KC_LCTL))` |
| Middle two thumbs | `25 + 26` | `Alt` | `P( LA | LO, SEND(KC_LALT))` |
| Right middle thumbs | `26 + 27` | `GUI/Win` | `P( RT | RD | RS | RZ, SEND(KC_LGUI))` |
| Outer thumbs | `24 + 27` | `Esc` | `P( LA | RU, SEND(KC_ESC))` |
| All four thumbs | `24+25+26+27` | `Caps Lock` | `P( LA | LO | RE | RU, SEND(KC_CAPS))` |

**Visual Guide:**
```
Thumbs:  [24] [25] [26]     [27] [28] [29]
         NUM  SPC  SHFT     ENT  SPC   FN

24+25 = Ctrl
25+26 = Alt
26+27 = GUI
24+27 = Esc
All 4 = Caps
```

#### Home Row Combos

| Keys | Position | Output | Purpose |
|------|----------|--------|---------|
| A + S | `13 + 14` | `Tab` | Quick tab access |
| J + K | `19 + 20` | `Backspace` | Quick delete |

#### Navigation Combos

| Keys | Position | Output | QMK Equivalent |
|------|----------|--------|----------------|
| H + J | `18 + 19` | `←` Left | `P( MOVE | RF, SEND(KC_LEFT))` |
| J + K | `19 + 20` | `↓` Down | `P( MOVE | RP, SEND(KC_DOWN))` |
| K + L | `20 + 21` | `↑` Up | `P( MOVE | RL, SEND(KC_UP))` |
| L + ; | `21 + 22` | `→` Right | `P( MOVE | RT, SEND(KC_RIGHT))` |

**Visual Guide:**
```
Home Row Right Hand:
[H] [J] [K] [L] [;]
 18  19  20  21  22

H+J = ←
J+K = ↓
K+L = ↑
L+; = →
```

#### Page Navigation

| Keys | Position | Output |
|------|----------|--------|
| Top right corners | `10 + 11` | `Page Up` |
| Bottom right corners | `22 + 23` | `Page Down` |

---

### Symbol Layer Combos

| Keys | Position | Output | Purpose |
|------|----------|--------|---------|
| { + } keys | `3 + 4` | `[` | Left square bracket |
| } + \| keys | `4 + 5` | `]` | Right square bracket |
| - + / keys | `8 + 9` | `_` | Underscore |

---

## Differences from QMK

### What Changed

| Feature | QMK Georgi | ZMK Stenomi |
|---------|------------|-------------|
| **Chord Processing** | Native with `P()` macros | Combos only (max ~4 keys) |
| **PWR Key** | Modifier for symbols | Replaced with SYMBOL layer |
| **Layer Count** | 3 (Steno, Gaming, Gaming_2) | 5 (Plover, QWERTY, Symbol, Number, Function) |
| **Mouse Keys** | Supported | Not available (placeholders added) |
| **Repeat Function** | `REPEAT()` | Not available |
| **Steno Mode** | Built-in firmware | Requires Plover software (HID mode) |

### What You Lose

1. **Complex Multi-key Chords**: QMK allowed unlimited key combinations like `P( LSU | LSD | LFT | LK, ...)`. ZMK combos are limited to ~4 keys maximum.

2. **PWR Key Magic**: In QMK, holding PWR + any key gave you symbols. In ZMK, you switch to the SYMBOL layer instead.

3. **Mouse Control**: QMK's `CLICK_MOUSE()` and mouse movement aren't available in ZMK.

4. **Dynamic Logic**: QMK's `processQwerty()` function allowed complex conditional behavior. ZMK is more static.

### What You Gain

1. **Wireless Support**: Native Bluetooth with easy pairing
2. **Better Power Management**: ZMK is optimized for battery life
3. **Display Support**: Nice!View and other displays work out of box
4. **Active Development**: ZMK is actively maintained and growing

---

## Tips and Tricks

### Getting Started

**Day 1-3: Muscle Memory**
- Start in QWERTY mode
- Practice thumb combos (Ctrl, Alt, Esc)
- Don't try to learn everything at once

**Week 1: Layer Switching**
- Practice switching between layers
- Learn NUMBER layer for digits
- Memorize SYMBOL layer positions

**Week 2: Combos**
- Add navigation combos (H+J, J+K, etc.)
- Practice page up/down combos
- Build speed with modifier combos

**Month 1: Stenography**
- If interested, start learning Plover
- Begin with the Learn Plover! book
- Practice in PLOVER layer for 15min/day

### Common Workflows

#### Programming
```
1. QWERTY for variable names
2. Hold SYMBOL for brackets/operators
3. Hold NUMBER for quick digits
4. Use combos for navigation
```

#### Writing
```
1. QWERTY for typing
2. Navigation combos for editing
3. FUNCTION layer for media control
4. PLOVER layer for speed (advanced)
```

#### Gaming
QWERTY layer works well for most games:
- Left hand on WASD
- Right hand on mouse
- Thumb combos for modifiers

### Customization Ideas

**Add Your Own Combos:**
1. Find positions using the key map
2. Edit the `.keymap` file
3. Add combo definition:
```c
combo_your_name {
    timeout-ms = <30>;
    layers = <QWERTY>;
    key-positions = <X Y>;
    bindings = <&kp KEY>;
};
```

**Popular Combo Ideas:**
- `Q + W` = Escape (top-left chord)
- `Z + X` = Undo (bottom-left)
- `M + ,` = Screenshot
- `P + ;` = Delete word

### Troubleshooting

**Combo Not Working?**
- Check `timeout-ms` (increase to 50-100ms)
- Verify key positions are correct
- Ensure you're on the right layer
- Press keys simultaneously, not in sequence

**Layer Stuck?**
- Press layer toggle key again
- Momentary layers auto-release
- Check for stuck key hardware issue

**Bluetooth Issues?**
- Use `0 + 11` combo to clear pairing
- Re-pair in computer's Bluetooth settings
- Toggle output with `1 + 10` combo

**Steno Not Working?**
- Ensure Plover is running
- Set Plover to "HID" mode (not serial)
- Check Plover recognizes your keyboard
- Verify you're in PLOVER layer (Layer 0)

---

## Keyboard Shortcuts Cheat Sheet

### Quick Reference Card

Print this out and keep it nearby:

```
╔══════════════════════════════════════════════════════════╗
║            STENOMI KEYBOARD QUICK REFERENCE              ║
╠══════════════════════════════════════════════════════════╣
║ LAYER SWITCHING                                          ║
║  • Top-left key ............ Toggle PLOVER ↔ QWERTY     ║
║  • Bottom-left (hold) ...... Access SYMBOL layer        ║
║  • Left thumb (hold) ....... Access NUMBER layer        ║
║  • Right thumb (hold) ...... Access FUNCTION layer      ║
╠══════════════════════════════════════════════════════════╣
║ THUMB COMBOS (QWERTY)                                    ║
║  • Left two thumbs ......... Ctrl                        ║
║  • Middle thumbs ........... Alt                         ║
║  • Right middle thumbs ..... GUI/Win                     ║
║  • Outer thumbs ............ Esc                         ║
║  • All four thumbs ......... Caps Lock                   ║
╠══════════════════════════════════════════════════════════╣
║ NAVIGATION COMBOS                                        ║
║  • H + J ................... ←  Left                     ║
║  • J + K ................... ↓  Down                     ║
║  • K + L ................... ↑  Up                       ║
║  • L + ; ................... →  Right                    ║
║  • A + S ................... Tab                         ║
║  • J + K ................... Backspace                   ║
╠══════════════════════════════════════════════════════════╣
║ SYSTEM COMBOS                                            ║
║  • Top corners (0+11) ...... Clear Bluetooth            ║
║  • Second corners (1+10) ... Toggle USB/BT              ║
╚══════════════════════════════════════════════════════════╝
```

---

## Resources

### Learning Stenography
- **Learn Plover!**: Free online book at [https://www.openstenoproject.org/](https://www.openstenoproject.org/)
- **Plover Discord**: Active community for help
- **QWERTYSteno**: Practice steno on QWERTY layout first

### ZMK Documentation
- **Official Docs**: [https://zmk.dev/docs](https://zmk.dev/docs)
- **Keycodes**: Full list of available keys
- **Combos Guide**: Advanced combo configuration
- **Behaviors**: Learn about tap-dance, mod-tap, etc.

### Communities
- **r/stenography** - Reddit community
- **r/ErgoMechKeyboards** - For hardware questions
- **Plover Discord** - Best place for steno help
- **ZMK Discord** - Firmware questions and support

---

## Appendix: Complete Keycode Reference

### Standard Keys
```
Letters:  A-Z (KC_A through KC_Z)
Numbers:  0-9 (KC_0 through KC_9, or N0-N9)
F-Keys:   F1-F12 (KC_F1 through KC_F12)
```

### Modifiers
```
LSHIFT, RSHIFT  - Shift keys
LCTRL, RCTRL    - Control keys
LALT, RALT      - Alt keys
LGUI, RGUI      - Windows/Command keys
```

### Navigation
```
UP, DOWN, LEFT, RIGHT  - Arrow keys
HOME, END             - Home/End
PG_UP, PG_DN         - Page Up/Down
```

### Special Characters
```
EXCL  !     AT     @    HASH   #    DLLR   $
PRCNT %     CARET  ^    AMPS   &    STAR   *
LPAR  (     RPAR   )    LBKT   [    RBKT   ]
LBRC  {     RBRC   }    PIPE   |    BSLH   \
FSLH  /     MINUS  -    UNDER  _    PLUS   +
EQUAL =     GRAVE  `    TILDE  ~    SEMI   ;
COLON :     SQT    '    DQT    "    COMMA  ,
DOT   .     LT     <    GT     >    QUES   ?
```

### Media Keys
```
C_PP        - Play/Pause
C_NEXT      - Next track
C_PREV      - Previous track
C_VOL_UP    - Volume up
C_VOL_DN    - Volume down
C_MUTE      - Mute
```

### Plover HID Keys
```
PLV_SL  - Left S       PLV_TL  - Left T
PLV_KL  - Left K       PLV_PL  - Left P
PLV_WL  - Left W       PLV_HL  - Left H
PLV_RL  - Left R       PLV_ST  - Star
PLV_A   - A vowel      PLV_O   - O vowel
PLV_E   - E vowel      PLV_U   - U vowel
PLV_FR  - Right F      PLV_PR  - Right P
PLV_LR  - Right L      PLV_TR  - Right T
PLV_DR  - Right D      PLV_RR  - Right R
PLV_BR  - Right B      PLV_GR  - Right G
PLV_SR  - Right S      PLV_ZR  - Right Z
PLV_NM  - Number (#)
```

---

**Version**: 1.0  
**Last Updated**: 2026-01-14  
**Firmware**: ZMK with Plover HID support  
**Hardware**: Stenomi (30-key split keyboard)

---

*Happy typing! Remember: it takes time to build muscle memory. Be patient with yourself and practice consistently.*