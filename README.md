# ErgoDox Extended

In a world where everyone is removing keys from their ErgoDox, I wanted more.

![split keyboard](https://i.imgur.com/GKVULLC.png)
![split keyboard from the side](https://i.imgur.com/Z4m2mXL.png)

My goals for this keyboard were to take my existing design from 2018 and remove the Teensy,
while making it more compact, a little more stylish, and with several options for cases in
mind.

![pcb closeup](https://i.imgur.com/xBKXy66.png)

I used an ATMega32u4-au for the mcu because I wanted to be able to solder it by hand if I
needed. Same for the MCP23018-e/ss. I stuck with Micro-USB because, again, hand soldering.

There are options for SMD or through-hole diodes.

Cherry keyswitches, I've never used Gaterons or any others so I can't say whether they
would be compatible with the pcb.

This board works just like the original ErgoDox board; the same board can be used for
either half of the keyboard. Solder the logic components on the front, and diodes on the
front or back of the board. The silkscreen for diode direction is set up for `Row2Col` in
the firmware.

![pcb render](https://i.imgur.com/7y7QCEE.png)

Everything should be included in the kicad project aside from the firmware. Make sure
to clone recursively so that it pulls the submodule(s).

Firmware is [here](https://github.com/Gephorian/qmk_firmware/tree/ergodox-extended) until
I get a PR merged into QMK.

## Manufacturing

I've used JLCPCB and Elecrow. Both are great. Go for 1.6mm, whatever color you want is
fine. I was able to generate a BOM using JLCPCB's plugin and get it partially assembled,
so that takes a lot of guesswork out of the soldering and debugging if you go that route.

## Contributing

Feel free to submit PRs and issues for fixes.
