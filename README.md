# nonSNES
An Open-Source HardWare (OSHW) recreation of the Super Nintendo Entertainment System (PAL)

The design tries to be a 1:1 recreation of the original SNSP-CPU-01 Rev5 board.

![SNES mainboard in blue](https://raw.githubusercontent.com/stonedDiscord/nonSNES/main/photo/snsp.jpeg)

## Some of the planned Changes and improvements
- [X] Replace the obsolete trimmer capcaitor with an in-stock one
- [X] Replace the reset button with a regular mechanical keyboard switch
- [X] Include an AV out connector board using mousebites
- [X] Replacefor the U11 regulator (the old mitsumi one had a nonstandard pinout for reset monitors)
- [ ] Include RGB bypass mod
- [ ] Remove the CIC/swapp it for a CIC replacement
- [ ] Region switch
- [ ] Replace the audio DAC
- [ ] Replace the audio RAM
- [ ] Replace the WRAM
- [ ] Replace the S-CLK clock generator
- [X] Include controller port board

## Tips if you decide to make this/get it made
I've compared prices using https://pcbshopper.com/ and last time I checked JLCPCB had the best prices and the board in the image was made by them.
This will vary depending on where it's shipped to. The dimensions are 188x159mm.

If you decide to get it assembled I suggest only getting the bottom side with all the SMD components done and doing the top yourself.
The bottom only has jellybean capacitors, resistors, diodes, transistors so it's not going to be very expensive.
I suggest going over the BOM with a text editor to replace all the 0805 component sizes with 0603 and all the SC-59 with SOT-23.
JLCPCB seems to be fading out 0805 resistors out of their "standard components", so this will save you some money.

For the top you will have to salvage the Nintendo components. The video RAM is still being made by S@Tech (HM62256).
The audio RAM can probably also be easily replaced, I haven't looked into this yet. Feel free to open an issue about it.

## Roadmap:
Get a 1CHIP version going, should be a lot easier to source and assemble

## Inspired by
https://github.com/Redherring32/OpenTendo

## Credits

ArcadeTV for the stripped scans:
https://circuit-board.de/forum/index.php/Thread/13913-STRIP-CLUB-PCB-Scans/

arzi84 for the schematic
