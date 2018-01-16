---
layout: default
title: Hardware
---
 * toc
 {: toc}

# FRDM K64F
 * [Board's page in the mbed site](https://developer.mbed.org/platforms/FRDM-K64F/)
 * [NXP page with links to technical docs](http://www.nxp.com/products/software-and-tools/hardware-development-tools/freedom-development-boards/freedom-development-platform-for-kinetis-k64-k63-and-k24-mcus:FRDM-K64F)

# Mbed Applications Shield
 * [Mbed examples](https://os.mbed.com/components/mbed-Application-Shield/)

# Storage
For storage of the board I use a "Really Useful Box, 0.2litre" box.
They are quite common, some (online options are)
 * [staples](http://www.staples.co.uk/0-2-litre-box-clear/cbs/297704891.html)
 * [maplin](https://www.maplin.co.uk/p/really-useful-02l-box-5-pack-n65fl)
 * [hobycraft](http://www.hobbycraft.co.uk/really-useful-clear-box-02-litres/571333-1000)
 * [amazon](https://www.amazon.co.uk/Really-Useful-Boxes-Rectangle-Box/dp/B001F67NJ4)

Or just find a shop and buy one.

# Windows 10 Fix
Windows 10 seems to mess with the board reset.  The problem lies in that Windows is trying to write drive house-keeping data to the virtual usb drive that appears as "MBED" (folders like _System Volume Information_).

Looking through various forums, this looks like a common complaint.
Most of the recommended solutions to turn off this feature involve setting a registry-key **DisableAutomaticRemovableDriveIndexing** to 1.

I didn't have any success with that, but the following comment I found in one discussion fixed the issue.  I now have my version of Windows 10 playing nicely with the board. (http://disq.us/p/15vrugs)
> In recent versions of Windows 10, as well as the above, you need to stop the Storage Service too (type Services into the start menu to find the management applet)

# If you do something silly
> Like press the reset button while running a debugger.

And end up with the red and green lights stuck on (need to detail the process)

* [Firmware FRDM K64F](https://developer.mbed.org/handbook/Firmware-FRDM-K64F)
* [Recovering FRDM-K64F mbed Board](https://mcuoneclipse.com/2014/04/19/recovering-frdm-k64f-mbed-board/)
* [How to Recover the OpenSDA V2.x Bootloader](https://mcuoneclipse.com/2016/06/26/how-to-recover-the-opensda-v2-x-bootloader/)
* [Firmware FRDM K64F](https://developer.mbed.org/handbook/Firmware-FRDM-K64F)
* [Download – OpenSDA Bootloader and Application](http://www.nxp.com/products/software-and-tools/run-time-software/kinetis-software-and-tools/ides-for-kinetis-mcus/opensda-serial-and-debug-adapter:OPENSDA?tid=vanOpenSDA#FRDM-K64F)
* [OPENSDA: OpenSDA Serial and Debug Adapter](http://www.nxp.com/products/software-and-tools/run-time-software/kinetis-software-and-tools/ides-for-kinetis-mcus/opensda-serial-and-debug-adapter:OPENSDA?tid=vanOpenSDA)


# Documentation
I've collected all the technical documentation and datasheets I can find.
(I'll have to go back and find the urls)

## ARM Cortex M4
* [Cortex M4 Generic User Guide]({{site.baseurl}}{% link docs/DUI0553A_cortex_m4_dgug.pdf%})
* [Cortex M4 Technical Reference Manual]({{site.baseurl}}{% link docs/DDI0439B_cortex_m4_r0p0_trm.pdf%})

## FRDM K64F
* [FRDM K64F User Guide]({{site.baseurl}}{% link docs/FRDMK64FUG.pdf%})
* [K64F processor Reference Manual]({{site.baseurl}}{% link docs/K64P144M120SF5RM.pdf%})
* [Accelerometer and Magnetometer]({{site.baseurl}}{% link docs/FXOS8700CQ.pdf%})
* [RGB led datasheet]({{site.baseurl}}{% link docs/CLV1AFKB(874).pdf%})
* [Board Schematic]({{site.baseurl}}{% link docs/FRDM-K64F-SCH-E4.pdf%})
* [Headder pins]({{site.baseurl}}{% link docs/FRDM-K64F_PKG_pins.pdf%})

## Application Shield
* [Board Schematic]({{site.baseurl}}{% link docs/ApplicationShield V_1_0_0 SCH.pdf%})
* [Board PCB layout]({{site.baseurl}}{% link docs/ApplicationShield V_1_0_0 BRD.pdf%})
* [LCD Datasheet]({{site.baseurl}}{% link docs/NHD-C12832A1Z-FSW-FBW-3V3.pdf%})
* [LCD Driver (ST7565R) Datasheet]({{site.baseurl}}{% link docs/st7565r.pdf%})
* [5-way switch]({{site.baseurl}}{% link docs/SKRH Series - Basic information.pdf%})
* [RGB led datasheet]({{site.baseurl}}{% link docs/CLV1AFKB(874).pdf%})
* [Accelerometer]({{site.baseurl}}{% link docs/MMA7660FC.pdf%})
* [Temperature sensor]({{site.baseurl}}{% link docs/LM75B.pdf%})
