# Dactyl wireless by filoxo

- 4 rows
- 6 columns
- Encoder

## Pinout



https://nicekeyboards.com/docs/nice-nano/pinout-schematic

## Notes

- I opted to make the right side primary because encoders on the secondary side are not supported ([yet](https://github.com/zmkfirmware/zmk/pull/728))
- I'd recommend that you [create your own zmk-config repo](https://zmk.dev/docs/user-setup#user-config-setup-script) to put these files into
- The keymap can be changed by updating the .keymap file, pushing to your config repo, and then following the steps here: https://zmk.dev/docs/user-setup#download-the-archive
- Unfortunately, there wasn't a good or sensible place to put a hardware reset button. If you need to reset the controller, take off the bottom plate, and short the two pins for GND and RST. The controller will then show up on your computer.
- The dot on the outside of the toggle switches denotes the ON position.
- The batteries used are 480mAh, which should last a long while. Unfortunately, ZMK does not currently have a way to signal low battery without a display. There is a current PR to add this as an underglow configuration that could be interesting to try to implement: https://github.com/zmkfirmware/zmk/pull/935
