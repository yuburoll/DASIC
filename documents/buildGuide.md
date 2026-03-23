# Build Guide

This is the build guide for DASIC.

This documents is translated by generative AI, so there can be some misleading texts.

**Images of the build guide are based on V1. I'm currently working on V2. read direction first, carefully.**

### Additional Resources

[**Soldering Tips**](solderingTip.md)

### Estimated Fabrication BOM

for only one set of DASIC:

![fabPCB](../images/dasicBOMpcb.png)

![fabCase](../images/dasicBOMcase.png)

for five set of DASIC:

![fab10PCB](../images/dasicBOM5piecesPCB.png)

![fab5Case](../images/dasicBOM5piecesCase.png)

The lowest per-unit cost comes from building five sets (approximately $45 each), but even building just two sets can bring the per-unit manufacturing cost down to around $55.

## Flashing Firmware onto the Controller Board

This guide assumes the use of an rp2040 board.

Hold the Boot button on the controller board while connecting the USB cable, and a removable drive will appear. (This is called DFU mode.)

Drag and drop the .uf2 file from the [uf2examples folder](../firmware/nologoRP2040qmk/examples) into the removable drive to flash the firmware. I recommend flashing the Vial firmware.

The firmware uses [QMK](https://qmk.fm/). If you want to build your own firmware, copy the "modubu" folder from the "firmware/qmk" directory into the "qmk_firmware\keyboards" directory and build it using QMK MSYS.

Once fully assembled, the Boot button becomes inaccessible, which causes issues. Therefore, **I recommend flashing the firmware before soldering the controller board**.

To enter DFU mode after flashing the firmware, hold the bottommost outermost switch (Left Ctrl or Fn position) while connecting the keyboard.

## Soldering the Controller Board

![headerPin0](../images/dasicBuildHeaderPin0.jpg)

![headerPin1](../images/dasicBuildHeaderPin1.jpg)

First, detach one row from the header pins included with the controller board. This is because the header pin closest to the USB port will not be soldered.

![processorSolder0](../images/dasicBuildProcessorSolder0.jpg)

![processorSolder1](../images/dasicBuildProcessorSolder1.jpg)

Insert and solder the header pins **with the processor components facing downward, and with the pin closest to the USB port left empty**.

If you have a breadboard, seating the header pins on it as shown above makes soldering easier.

![processorSolder2](../images/dasicBuildProcessorSolder2.jpg)

Solder the processor board you just prepared onto the PCB.

**The side where the processor board is mounted becomes the BACK of the PCB, and the opposite side becomes the FRONT. Flip the PCB according to whether it is for the left or right hand, then mount the processor board.**

![processorSolder4](../images/dasicBuildProcessorSolder4.jpg)

**NOTICE: The photo avove is for V1, V2 have different header footprint.**

Looking at the front of the PCB, solder all the header pins to pads.

The actual V2 footprint looks like the following. There is no THT hole in the center, and pads are positioned above and below. Please apply a generous amount of solder to connect the pads and pins.

![v2pad](../images/dasicV2Pad.png)

## Soldering the Connector & Jumping

![componentPositioning](../images/dasicBuildComponentPositioning.jpg)

![jackSolder0](../images/dasicBuildJackSolder0.jpg)

![jackSolder1](../images/dasicBuildJackSolder1.jpg)

![jackSolder2](../images/dasicBuildJackSolder2.jpg)

Position the TRRS connector so that it sits on the back side of each hand, and solder from the front side. Using masking tape or similar to hold it in place while soldering is recommended.

While looking at back side, bridge the three jumper pads near the text "JUMP when BACK SIDE" with solder. Do not do this on the opposite side (= the front side where the connector isn't mounted).

When soldering jumpers, first coat the soldering iron tip generously with solder paste, then melt a bead of solder onto it. In this state, bring the bead to the jumper pads and pull away once the two pads are bridged.

- If the pads are bridged but the solder forms a sharp, pointy peak, apply more solder paste to the tip.

- If the pads are not bridging and the solder just beads up on one pad, add more solder to the tip.

- Success is when the pads are bridged with a smooth, dome-shaped bead. Move on to the next jumper.

If it is not working, let the jumper area cool for a moment, apply a generous amount of flux to both the tip and the jumper, and try again.

Do not hesitate; wait patiently and check lead shape.

## Soldering the Diodes

![diodeTip](../images/diodeTip.jpg)

If using THT diodes, pre-bend the diode legs into a U-shape as shown in the photo above.

Start by soldering the diodes on the column with the greater number first. It does not matter whether you solder from the front or the back, but **all diodes must face outward.**

![DiodeSolder0](../images/dasicBuildDiodes0.jpg)

![DiodeSolder1](../images/dasicBuildDiodes1.jpg)

![DiodeSolder2](../images/dasicBuildDiodes2.jpg)

![DiodeSolder3](../images/dasicBuildDiodes3.jpg)

After soldering, clip all the protruding diode legs with flush cutters. Cut them as close as possible so they do not touch neighboring pads. Always hold the leg with your fingers while cutting to prevent it from flying away.

![DiodeSolder4](../images/dasicBuildDiodes4.jpg)

![DiodeSolder5](../images/dasicBuildDiodes5.jpg)

![DiodeSolder6](../images/dasicBuildDiodes6.jpg)

After finishing the first column, solder the next column in the same order. **Be careful not to let the diode legs touch each other.**

When using SMD diodes, pre-tin one pad at the diode position, then reheat that pad.

When the solder on the pad melts, place one leg of the SMD diode to align it, then solder the other leg.

## (Optional) Soldering the SMD Switch

The SMD switch is connected to the reset pin. For processor boards other than the rp2040, this switch is used to enter DFU mode. solder this switch on the back side.

The method is the same as for SMD diodes. Pre-tin one pad at the switch position, then reheat that pad.

When the solder on the pad melts, place one leg of the switch to align it, then solder the remaining legs.

## (Optional) Soldering Mill-Max Sockets

![millmax0](../images/dasicBuildMillmax0.jpg)

![millmax1](../images/dasicBuildMillmax1.jpg)

As shown in the photos above, insert the Mill-Max sockets from the front side, secure them with masking tape or similar, and then solder.

The correct position for inserting the Mill-Max sockets is the hole where no pad is visible from the front, and is centered on the pad visible from the back.

![millmax2](../images/dasicBuildMillmax2.jpg)

Pay special attention when securing the Mill-Max sockets for the Caps & Enter keys, referring to the photo.

When viewed from the front, they should be aligned to the off-center position; when viewed from the back, they should be centered on the pad shape.

## Assembling the Stabilizers

![stabilizers](../images/dasicBuildStabilizers.jpg)

Install stabilizers on all positions where keycaps of 2u or larger will be placed.

By default, stabilizers are installed in four locations: left Shift, two Spacebar positions, and Enter.

## Checking the Assembly

Inspect the solder joints and their positions to verify that the assembly is correct. The side where the diodes are mounted does not matter as long as the orientation is correct.

## Assembling Switches and the Plate

![plates1](../images/dasicBuildKeyboardPlates1.jpg)

![plates2](../images/dasicBuildKeyboardPlates2.jpg)

Pre-install the switches and blockers onto the keyboard plate. The photo also shows keycaps installed, but you do not need to install keycaps at this stage.

![plates0](../images/dasicBuildKeyboardPlates0.jpg)

To install the blockers, tighten the screws as shown in the photo above. If using the halfScrew version, hook one protruding end over the plate, then secure the other end with a screw.

![plates3](../images/dasicBuildKeyboardPlates3.jpg)

**NOTICE: The photo avove is for V1, you must position dev board and jack on back side (opposite side).**

Place the assembled board on top as shown in the photo, and solder the switches.


## Assembling the Case

![case0](../images/dasicBuildCaseAssemble0.jpg)

**NOTICE: The photo avove is for V1, you must position dev board and jack on back side (opposite side).**

Insert the plate and PCB assembly into the case.

As shown in the photo, tilt the assembly and insert the TRRS socket end first to position it correctly.

![case1](../images/dasicBuildCaseAssemble1.jpg)

**NOTICE: The photo avove is for V1, you must position dev board and jack on back side (opposite side).**

Once the assembly is inserted into the case, it will look like this.

- Securing only the plate with screws gives a softer typing feel. There are 5 screw points per keyboard half.

- Securing the PCB as well gives a firmer typing feel. There are 4 additional screw points per keyboard half.

After securing the screws, attach the back plate to the case. There are 7 fastening points per keyboard half.

Finally, attach the 4 bumpon pieces at the bumpon positions on the each back plate, and you are done.
