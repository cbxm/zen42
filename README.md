# Zen42 — A somewhat sane keymap for the Corne-ish Zen V2

![Corne-ish Zen Logo](img/Zen_R3_sticker.png)

This repository contains my personal keymap configuration for the Corne-ish Zen V2 low profile wireless mechanical keyboard. It's based on the official configuration but customized to suit my specific needs and preferences.

## Keymap Overview

The keymap is designed with multiple layers to provide easy access to a wide range of functions while maintaining a compact 42-key layout. Here's a brief overview of the layers:

1. **Base Layer**: Standard QWERTY layout with some modifications for improved ergonomics and efficiency.
2. **F-Numbers Layer**: Function keys and numpad layout.
3. **Symbols Layer**: Easy access to symbols and special characters.
4. **Navigation Layer**: Arrow keys, page navigation, and media controls.
5. **Board Layer**: Bluetooth controls and additional function keys.

### Key Features

- **Consistent Modifiers**: All modifier keys (Shift, Ctrl, Alt, GUI) are accessible from every layer, ensuring consistent keyboard behavior across layers.
- **Custom Modifiers**: The base layer includes custom modifiers like `mt RALT DELETE` for the top-right key, combining Alt and Delete functions.
- **Layer Switching**: Utilizes the `lt` (layer-tap) function for easy layer switching, e.g., `lt 3 SPACE` for accessing the navigation layer.
- **Bluetooth Functionality**: The board layer includes Bluetooth clear, previous, and next functions for easy device switching.
- **Conditional Layers**: Implements a conditional layer that activates the board layer when both layer 2 and 1 are active.

## Keymap Details

### Base Layer

```txt
|  TAB  |  Q  |  W  |  E  |  R  |  T  |   |  Y  |  U   |  I   |  O  |  P  | ALT/DEL |
| BKSP  |  A  |  S  |  D  |  F  |  G  |   |  H  |  J   |  K   |  L  |  ;  |    '    |
| SHIFT |  Z  |  X  |  C  |  V  |  B  |   |  N  |  M   |  ,   |  .  |  /  |  SHIFT  |
                   | GUI | ENTER | CTRL/ESC | ALT/ENTER | SPACE/NAV | MENU/FN |
```

The base layer is designed for efficient typing with easy access to common modifiers and layer switches.

### Function and Numpad Layer

```txt
| trans | F10 | F7 | F8 | F9 |     |   |   +   |   7   |   8   |   9   |   *   | trans |
| trans | F11 | F4 | F5 | F6 |     |   |   -   |   4   |   5   |   6   |   /   |   =   |
| trans | F12 | F1 | F2 | F3 |     |   |   0   |   1   |   2   |   3   |   ,   | trans |
                    |    |    |    |   | trans | trans |       |
```

This layer provides access to function keys and a numpad layout for quick number entry.

### Symbols Layer

```txt
| trans |  !  |  @  |  #  |  $  |  %  |   |  ^  |  &  |  *  |  (  |  )  |    \   |
| trans |  `  |  {  |  [  |  (  |  =  |   |  -  |     |     |     |  "  |        |
| trans |  ~  |  }  |  ]  |  )  |  +  |   |  _  |     |     |     |     | trans  |
                    |     |     |     |   |     |     |     |
```

The symbols layer provides easy access to commonly used symbols and brackets.

### Navigation Layer

```txt
| trans |     |     |     |     |      |   |       |       |       |       | trans | trans |
| trans |     |     |     |     | PgUp |   | Left  | Down  |  Up   | Right | Mute  |       |
| trans |     |     | Home| End | PgDn |   | Play  | Prev  | Next  | Vol-  | Vol+  | trans |
                    |     |     |      |   | trans | trans |       |
```

This layer focuses on navigation and media controls for improved workflow.

### Board Layer

```txt
|      |     |     | BT_CLR | BT_PRV | BT_NXT |   |     |     |     |     |     |      |
|      |     |     |        |        |        |   |     |     |     |     |     |      |
|      |     |     |        |        |        |   |     |     |     |     |     |      |
                    |        |        |        |   |     |     |     |
```

The board layer provides Bluetooth controls for easy device management.

## Customization

Feel free to fork this repository and customize the keymap to suit your needs. The main keymap file is located at `config/corneish_zen.keymap`. You can modify the layers, key bindings, and behaviors to create your perfect layout.

## Flashing Instructions

To flash this firmware to your Corne-ish Zen V2 keyboard:

1. Fork this repository to your GitHub account.
2. Make any desired changes to the keymap file (`config/corneish_zen.keymap`).
3. Commit and push your changes to your forked repository.
4. GitHub Actions will automatically build the firmware for you.
5. Download the firmware zip file from the Actions tab in your GitHub repository.
6. Extract the `.uf2` files and flash them to your keyboard using the standard flashing procedure.

For detailed flashing instructions, please refer to the official Corne-ish Zen documentation.

## Resources

- [Official ZMK Firmware GitHub](https://github.com/zmkfirmware/zmk)
- [ZMK Documentation](https://zmk.dev/docs)
- [ZMK Discord Server](https://zmk.dev/community/discord/invite)

## License

This configuration is released under the MIT License. Feel free to use, modify, and distribute it as you see fit.
