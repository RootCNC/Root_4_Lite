---
title: Root 4 Lite Assembly Guide
description: Root 4 Lite Assembly Guide for Newbies
published: true
date: 2022-06-28T21:37:30.411Z
tags: root 4 lite, r4 lite, guide
editor: markdown
dateCreated: 2022-05-24T19:30:47.756Z
---

# Root 4 Lite Assembly Guide for Newbies
> Please note: This Assembly guide was community made by #RobF - please send your love his way!
>
> If you would like to support the project in any shape or form, please get in touch with Pete!
{.is-success}

## Introduction
So, you’ve watched all [Pete’s YouTube videos](https://www.youtube.com/c/sailorpete12/videos), admired the elegant simplicity of the Root 4 Lite (R4L) design.  You’ve compared the costs of buying a Chinese 3018 engraver or other DIY CNCs and can see a strength, performance, simplicity benefit in the Root CNCs.  You’ve got access to a 3D printer and may have even started printing Root CNC parts.  The only problem is you’ve never built a CNC or operated one before.  Fear not, others have been this way and succeeded with some planning and patience.  

This guide aims to provide a bit more detail on how to plan, print, build, and check basic operation of our R4L CNC.  

## Resources
Root 4 Lite Github: [Link Here](https://github.com/RootCNC/Root_4_Lite)
### Useful Links
- Bill of Materials (BOM): [Link here](https://github.com/RootCNC/Root_4_Lite/tree/main/BOM)
- Source STL and DXF Files: [Link here](https://github.com/RootCNC/Root_4_Lite/tree/main/Source)
- Working Area spreadsheet calculator: [Working%20Area.xlsx](https://github.com/RootCNC/Root_4_Lite/blob/main/Working%20Area.xlsx)


### Useful Videos
YouTube – make sure you’re familiar with the 4 R4L assembly videos:
- [Another 3D Printed CNC Machine? PT1](https://www.youtube.com/watch?v=DjvXqU2bEzY)
- [Building a small High performance 3D printed CNC machine – Root 4 Lite PT2](https://www.youtube.com/watch?v=-5PmiW85Cyw&t=618s)
- [3D Printed CNC Machine – Root 4 Lite PT3](https://www.youtube.com/watch?v=_y3V89cwmr8)
- [Root 4 Lite PT4 – the final stage assembly for the DIY 3D printed CNC machine](https://www.youtube.com/watch?v=ivuQiyucW90&t=402s)

### Social links
- [Root 4 Lite CNC Webpage](https://rootcnc.com/root-4-lite/)
- [Facebook Group](https://www.facebook.com/groups/rootcnc/)
- [Discourse](https://rootcnc.discourse.group/)
- [Root CNC Discord Channel](https://discord.gg/93Ue5SwthW) Great for quick answer to questions
- [Thingiverse](https://www.thingiverse.com/sailorpete/designs)
- [Youtube](https://www.youtube.com/c/sailorpete12/)

## Planning and Preparation
### Practicalities
Where is your machine going to live, and can your significant other or neighbours cope with the noise and dust?  How much space do you realistically have available.  What materials do you expect to be cutting?  The Root 4 Lite is a great compromise between relatively easy to understand parts, few special tools, strong design, and flexible sizing options.

The majority of 3D parts are not overly complex, show thoughtful design to avoid weak points, and will fit on the baseplate of a modest 3D printer (200x200mm).  

### 3D printed parts
These need to be dimensionally precise – check your printer is calibrated and capable of reproducing parts to correct sizing.  Consider printing a 20mm [calibration cube](https://www.thingiverse.com/thing:1278865).  Aim to print with more walls than usual (e.g. 3-6), higher % infill.  Layer sizes of 0.3 – 0.4 mm printed in PLA, PLA+, or ABS should all be fine.  Where supports are required be prepared to remove as much of this as possible later.  Most parts contain cavities or indentations for receiving bolts and nuts – check these spots are particularly clean before assembly begins.

### Sizing
Use the excellent [sizing spreadsheet](https://github.com/RootCNC/Root_4_Lite/blob/main/Working%20Area.xlsx) from the Github site.  Bigger is not always better – for ballscrew sizes approaching 750-1000mm, consider building a full [Root 4 CNC](https://rootcnc.com/root-4/) for a stronger, more capable (and more expensive) machine.  The spreadsheet assumes you will be using 12mm thick side panels.  Warning:  If you use thicker or thinner material, the size of your X axis ballscrews and Box Section Lengths may need adjustment.  

The R4L side panels contain main important mounting holes for the Y axis carriages and X axis assemblies.  It is highly recommended you consider purchasing these from the Root CNC website shop, or have them made up locally (from the BOM DXF files section).  If possible avoid attempting to cut them manually – it will make your building significantly easier.

The [Github](https://github.com/RootCNC/Root_4_Lite) site also includes a DXF file for preparing a suitable 18mm baseboard with holes positions for mounting Y Axis supports and threaded inserts.


### Choice of Spindle/Router
Pete has designed the R4L specifically for a cooled 240V spindle driven by a VFD.  This should result in optimal control over spindle speed, cutting power, noise and longevity.  It is also possible to fit a 240V/110V router (e.g. Makita RTO700C).

For more information on spindles, please check out the Bill of Materials (BOM) [Link Here](https://github.com/RootCNC/Root_4_Lite/tree/main/BOM)


### Choice of Control Hardware/Firmware
Any solution that will drive at least 4 axes is theoretically suitable.  A robust and future-proof solution would be Pete’s own “Root Controller”, offering full opto-isolation and a multitude of driver and control options, Wifi operation and other benefits of ESP32 GRBL [FluidNC](https://github.com/bdring/Grbl_Esp32).  Beginners or those on a budget might consider an Arduino Uno or Mega solution with suitable shield (e.g. [RAMPS](https://reprap.org/wiki/RAMPS_1.4)).

### Choice of Box Section Rails
Aluminum box section is strong and light and won’t corrode.  Steel box section may need a little more cleaning, and if possible check the sizing with calipers before purchase.  Steel sections may be helpful for section lengths above 750mm.  Aluminum is fine otherwise.

### Hardware
If you’re not going to buy all the required parts straight away, consider at least ordering these parts first to allow assembly of the Y rails and X assembly:
- M5x60 pan head bolts (for the 8 carriages and 625 bearings)
	- M5 loc nuts
	- M5 washers
- M3x14mm cap head bolts
	- M3 nuts
	- M3 standard and penny washer
- Side panels
- Baseboard
- Box sections (aluminum or steel)
- Consider buying a set of bolts, washers and screws off Aliexpress or eBay initially
	-E.g. “1080pcs M2/M3/M4/M5 stainless steel bolts nuts screws heax head assorted”
	- (then buy specific items as needed afterwards)

### Tools
A set of extra-long Allen Keys with “ball ends” is recommended for R4L assembly.  Although not essential, these make some assembly steps (e.g. mounting steppers to motor mounts) much easier.

## Assembly

>General Notes:  The assembly guide below is a suggestion on how to proceed.   Steps may not necessarily have to be executed in the order shown, but others have found this a safe way to put the R4L together.
{.is-info}

### Baseboard Preparation
MDF or marine plywood are both suitable material.  It’s not essential to seal and paint the CNC sideboards or baseplate, but it may help avoid long term swelling from moisture, particularly if you will be using MDF.  

> MDF is particularly prone to absorption of both sealers and paint.  Consider applying at least 2 sealing coats before painting.
{.is-warning}

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/insert.png" width="600">

It is easier to decide on any mounting hardware options before assembly, along with drilling holes and mounting inserts.

If you want to build a different size machine, there is a handly calculator to work out the size of the machine vs build area vs length of box sections: [LINK Working Area Spreadsheet](https://github.com/RootCNC/Root_4_Lite/blob/main/Working%20Area.xlsx)

There is also a handy tool to generate the a matrix of mounting holes within the baseboard, to aid in the mounting of work peices. This tool can be brought and downloaded from the store [Drill Location spreadsheet tool](https://rootcnc.com/product/drill-location-spreadsheet/)

#### Baseboard Video reference
- [R3L detailed build](https://youtu.be/z-iaeO7dcOc?t=655)  - 10:55 onwards
- [R4L Part one](https://youtu.be/DjvXqU2bEzY?t=469) 7:49 onwards)


### Carriages

Ensure any leftover support plastic inside the printed carriages is cleaned away.  A small allen key just large enough to clear the slot cut outs can help.  You may have more or less cleaning to do depending on how precise your 3D printer is creating the many internal cavities.  Gently run an M3 drill bit through the side holes to ensure the full depth is clear.
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/singlecarraige.png"  width="600">
Insert the M5x20 HEX head bolts (4 for each carriage plate), then locate an M5 washer, 625 bearing, 2nd M5 washer, and finally an M5 Loc nut.  Tighten nuts until just firm.

> Don’t assemble the carriage plates on the 20mm square box sections just yet.
{.is-info}

#### Carriages Video reference
- [R4L Part one](https://youtu.be/DjvXqU2bEzY?t=489) 8:09 onwards

### Y Axis Sections
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/yaxis_sections.png" width="600">

> Note If you intend to mount endstop switches at the front of the Y rails, or include wiring for future accessories, remember to run your shielded cable through the box section rails and Y axis boxmounts BEFORE assembly.
{.is-info}

Check the 4 box section lengths against the sizing spreadsheet for your planned build.  Make sure each end is filed slightly to take the off the edges and corners that will be inserted into the 3D printed Y Axis boxmount.  The Y axis rails will fit approx. 20mm inside each Y boxmount – do a pre-assembly check that the each rail with the 2 boxmounts attached will locate correctly on the baseboard holes.  Lightly mark each rail 20mm in from the end to ensure proper seating.  Using a mallet or wood block and hammer, knock the rail into each Y axis boxmount.  

Don’t mount the Y rails just yet – its best to assemble a carriage onto each rail before you mount rails to the baseboard.  
Video reference:  R4L Part two [Link](https://www.youtube.com/watch?v=-5PmiW85Cyw&t=618s) 8:47 onwards


### Y Rails and Carriages
Now assemble a pair of carriage plates on each Y rail.  Insert 4 M5x60mm Pan head bolts through the top carriage plate, an M5 washer and M5 nut on the other side, then the bottom carriage plate (on other side of the Y rail box section), then another M5 washer, and finally an M5 loc nut.  When all 4 M5x60 bolts are in place, gently but firmly tighten the loc nuts.  These need to be firm enough that the carriages sit firmly on the box sections with any rocking movement.  Slide the assembled carriage back and forth and check each of the 4x625 bearings is moving smoothly – if one or more aren’t rolling properly, then consider tightening the respective bolt a little more.  
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/carriages.png" width="600">

For the inward facing side of the carriages, it is worth seating M3 nuts in the various slots/cavities ready for later bolting to side panels and Z axis assembly.  To do this, pop an M3 nut into the top or bottom carriage slots.  Using an M3x30mm bolt, locate the nut onto the bolt, then tighten the bolt so the nut is pulled down into the hex-shaped cavity within the carriage.  It is particular helpful to do this for panel-facing sides of the carriages.  If any of the nuts don’t seat firmly, it might be helpful to put some masking tape over the nut slots to stop these escaping.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/baseboardfeet.png" width="600">
In a similar fashion, locate 4xM3 nuts in the front and rear slots near the base of each Y axis boxmount.  Locate the Y Axis boxmounts over the baseboard mounting holes.  Insert M3x30mm bolts from the bottom, located through a Y axis “foot”, up through the baseboard and up into the boxmount.  Gently tighten each M3 bolt with an allen key – consider inserting a small set of pliers into the boxmount slots to stop the M3 nuts popping out of their locating holes as the M3 bolts are tightened.  

Only loosely tighten each M3 bolt.  When both rail assemblies are mounted, check they are square on the baseboard and separated by the same distance at front and rear.  When positioned correctly, firmly tighten each M3 bolt from under the baseboard.   


#### Y Rails and Carriages Video Reference
R4L Part three [Link](https://www.youtube.com/watch?v=_y3V89cwmr8) 7:22 onwards


### X Gantry Assembly
As per the Y rails, make sure there are no sharp corners or edges on each end of the X rails (box sections).  Using a mallet, gently knock each X rail into a single X-axis boxmount, making sure the completely flat outside surface of the boxmount is facing out from the box section rails.  Sit this out flat face on a block of wood when bumping in each X box section rail to ensure the end of the box section sits flush with the outside surface of the boxmount.  
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/X_GantryMallet.png" width="600">

#### X Gantry Rails Video Reference
X Gantry Rails  R4L Part one [LINK](https://youtu.be/DjvXqU2bEzY?t=572) (9:30)

> Note that one end of the X-axis boxmount has a hollowed out space where the X axis endstops will eventually be mounted (circled in red).  This end will be pointing vertically UP.  
{.is-warning}

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/Sidehighlight.png" width="600">

Now go ahead and mount the remaining 2 carriages on the X rails.  Just as you did for the Y rails, use M5x60mm Pan head bolts (bolt pointing downwards), M5 nuts, washers and loc nuts.  It’s worth using loc nuts on the bottom to ensure the correct mounting pressure on the rails - and also protect against spindle vibrations shaking these loose which will minimize the need for constant maintenance.  

Now is also a good time to drill and clean out the M3 holes on the gantry side facing the front of the machine and seat some M3 nuts in the carriage slots (again, same as previously done for the Y rails)

### Z Axis Linear Rail Mount Preparation
Drill/clean out the M3 holes for the linear rails and rear mounting holes on to the X gantry carriages.  Check the orientation of your linear rails before bolting them to the Z carriage – if at all possible you want to very top of the linear rail to be flush with the top of the Mount assembly (so that when we later mount an FK10 bearing block on the top of the linear rail mount it will be able to sit flat).  


<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/top_bearing.png" width="600">

> The top of the linear rails should be flush with the very top of the linear rail mount assembly, or just below.
{.is-info}

Go ahead and mount the linear rails with M3x10 (or 8mm) bolts.  Slide the cars on to the linear rails.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/Z_Axis_Mounting.png" width="600">

#### Linear bearings Video Reference
Linear bearings being mounted R4L Part one [LINK](https://youtu.be/DjvXqU2bEzY?t=626) (10:26)

> Use 2 long bolts temporarily for the bottom most holes on the linear rails – to stop the cars sliding off the rails during later stages, until we eventually mount the Z axis carriage to these.
{.is-info}

### Mount the Z axis linear rail mount
Mount the Z axis linear rail mount to the X axis carriages.  Make sure you have the rail mount orientated right way up (Large FK10 bearing mount facing upwards).  Don’t be in a hurry to tighten down until all 16 bolts are seated loosely in their respective M3 nut, and the nut has retracted and seated into the carriage assembly so that it is held firmly and not rotating.  Once all bolts and nuts are seated and firm, then proceed to tighten everything up. Slide a 608 bearing into the bottom bearing mount of the linear rail mount – you shouldn’t have to squeeze too hard to get this in – consider running some sandpaper around the inside of the bearing mount to remove any rough plastic if the bearing doesn’t slide into please easily.

#### Attaching linear rail mount Video Reference
Attaching linear rail mount to X axis carriages R4L Part one [LINK](https://youtu.be/DjvXqU2bEzY?t=711) (11:51)

### Mounting the X Axis gantry to the Y rails
Attach each panel to the carriages on the Y rails using M3 bolts and washers – you should have previously installed and seated the M3 nuts inside the carriages, but if you didn’t do so now.  Only loosely tighten each bolt, enough to ensure the corresponding M3 nut has retracted back into the carriage and not spinning.  You may need to use a small screwdriver or allen key on some of these to stop them spinning until they tighten down properly into the recess inside the carriage.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/GantryMounting.png" width="600">

#### Attaching X gantry to Y rails Video Reference
Attaching X gantry to Y rails - R4L Part three [LINK](https://youtu.be/_y3V89cwmr8?t=331) (5:31)

Once all 16 bolts are in place, check the gantry is as close to vertical as possible, relative to the baseboard, using a large setsquare.  Take your time doing this, as it will result in properly square machine later on.  Check the X and Y rails are moving freely.  Tighten down the M3 bolts attaching the side panels to the Y rail carriages.   

If you left one Y rail only loosely tightened down on to the baseboard, now is the time to check again the Y rails are square and properly space to all the X gantry to slide smoothly fully forward and back.  Once satisfied, tighten down the M3 bolts to firmly lock into position this Y rail.  Don’t be too concerned if the machine isn’t perfectly square when the X gantry if fully forward or back – GRBL can autosquare out minor differences in the location of the Y rails and X gantry assemblies.   Check again the bolts on the X gantry and those attaching the sides panels are all firmly tightened.  

> Congratulations – you’ve now got something that’s starting to look like a CNC!  :)
{.is-info}

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Assembly-Guide/Root4_Dry.png" width="600">

#### Basic Motion Video Reference
End of R4L Part three [LINK](https://youtu.be/_y3V89cwmr8?t=331) (note Pete has already installed the X axis ballscrew in the pic)
