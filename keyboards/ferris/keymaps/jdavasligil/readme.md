J's Keymap for the Ferris Keyboard
==================================

This keymap is optimized for programming.

What do all these layers do?
----------------------------

### Layer 0: Base layer

![Layer 0](https://i.imgur.com/HjNHUPL.png)

On tapping the keys, our base layer is qwerty with space on the right homing thumb and backspace on the left homing thumb.

Right thumb is used for one shot hits to Layer 1. Double tapping toggles Layer 4.

Left thumb is the SUPER key.

The behaviour of some keys differ when held:
* Right homing thumb enables Layer 2.
* Left homing thumb enables Layer 3.
* Both homing pinkies behave as shift.
* Both bottom-row ring fingers behave as ctrl.
* Both bottom-row middle fingers behave as alt.

### Layer 1: One Shot Macros

Layer 1 has some commonly used programming macros on the bottom row, and common
symbols laid out symmetrically on the home and top rows.

### Layer 2: Numbers and Functions

This layer is simple. It provides access to numbers on the home row.

### Layer 3: Numpad

The right side is a Numpad, and the left side provides some common arithmetic
symbols including period and underscore.

### Layer 4: Navigation / Media

This layer provides the arrow keys on the right home row, page navigation on the
left home row, mouse control top left, media control for space, volume control on
the bottom right, etc.

## How to Flash / Update

Switch to python virtual environment.

```
workon ipy
```

Then, compile and flash.

```
qmk compile && qmk flash
```

Wait until prompted to reset.

Open a new tab and then give the VENV permission to write. Type the following
immediately after resetting:

```
sudo chmod o+rw /dev/ttyACM0
```

Fin.
