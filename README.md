# Tradrack LED stick

This is a mod for Annex Engineering's [TradRack][1] that enables the addition
of LED light indicators for each filament gate/lane.

![Rendered image of the v1 PCB](pcb/images/v1.png)

Since the lanes are spaced at a 17mm pitch, there are no regular LED strips
that would fit a Tradrack with a large number of lanes (I myself use ~35 lanes),
hence the need for this project.

This project is not an official Annex Engineering project and bears no
affiliation with the Annex Engineering organization.  The project is licensed
under the terms of GPL-3.

There are various software options available for controlling these LEDs,
for example by using the [Happy Hare][2] software to control the Tradrack.

For now there's only a PCB design in this repo.  I might eventually add
some 3D-printable parts that aid in mounting the LED boards.

## Fabrication

You can easily get the PCBs fabricated at various PCB shops.  I provide
easy-to-use files for fabrication using [JLCPCB][3] in the `pcb/fabrication-outputs` folder.
Simply upload the files to JLCPCB's assembly service and everything
should mostly just work.

## Mounting

The PCBs are designed with a 17mm pitch which should match the Tradrack lane
spacing.  You can join the PCB with a short piece of wire, a solder bridge,
or a JST-XH straight-through connector.  The PCBs are designed with a 1mm
gap between them to allow for some adjustment when aligning multiple PCBs,
in case the lanes or the PCBs themselves have some imperfections.

The PCBs are also designed to be easy to cut at an arbitrary point without
causing a short.  Cutting the PCB between any two LEDs should be easily done
with a hack saw/rotary cutter/...  Just make sure to use appropriate protective
equipment and maybe have a spare stick in case something goes wrong.

[1]: https://github.com/Annex-Engineering/TradRack
[2]: https://github.com/moggieuk/Happy-Hare/blob/main/doc/leds.md
[3]: https://jlcpcb.com/
