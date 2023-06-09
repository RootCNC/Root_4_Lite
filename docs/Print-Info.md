---
title: Root 4 Lite Print Orientation
description: How to print the parts for the Root 4 Lite
published: true
date: 2022-06-28T22:24:57.245Z
tags: root 4 lite, how to print
editor: markdown
dateCreated: 2022-06-28T22:17:17.168Z
---

# How to Print
Print settings for any of the Root CNC machine is key for a long lasting - high performance CNC machine. Below are the setting I used:

Resolution: 0.25-0.35mm
Infill: 50-60%
## Notes:
- Strength is key! use the hardest settings possible
- Print with 3-4 perimeters
- Print with ABS, PETG PLA will be fine though your mileage may vary (I am worried about the low glass transistion point of PLA being too low for the motors)

# DustShoe_Bottom.STL

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/dustshoe_bottom.png" width="600">

# DustShoe_Rail_Right.STL

> For the left side - Please mirror in your slicer
{.is-info}

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/dustshoe_rail_right.png" width="600">

# X_Aixs_DragChainMount.STL.
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/x_aixs_dragchainmount.png" width="600">

# X_Axis_BearingIdler.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/x_axis_bearingidler.png" width="600">

# X_Axis_BoxMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/x_axis_boxmount.png" width="600">

# X_Axis_MotorMount.STL

> Needs supports, print with hex nut end down

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/x_axis_motormount.png" width="600">

# X_Y_Axis_Carriage.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/x_y_axis_carriage.png" width="600">

# Y_Aixs_DragChainMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_aixs_dragchainmount.png" width="600">

# Y_Axis_BoxMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_boxmount.png" width="600">

This piece needs some support, you can paint it like this (you need it only for the leg, everything else prints just fine without support):

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_boxmount-painted_support.png" width="600">

Here's how the support will look like. It will be easy to remove and it's on internal faces, so it will not be visible once mounted.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_boxmount-rendered_support.png" width="600">

# Y_Axis_Foot.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_foot.png" width="600">

# Y_Axis_Idler.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_idler.png" width="600">

This piece needs a little support, you can paint it like this:

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_idler-painted_support.png" width="600">

Here's how the support will look like. It will be easy to remove and it's on a down facing spot, so it will not be visible once mounted.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_idler-rendered_support.png" width="600">

# Y_Axis_Motor_FK10_BearingMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_motor_fk10_bearingmount.png" width="600">

This part needs some support for both the long bridges and the hex bolt point. I (Valerioa) forgot to add support on the hex bolt overhang and got a big blob (the part will be probably usable, but a bit support should result in a better print)

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_motor_fk10_bearingmount-painted_support.png" width="600">

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/y_axis_motor_fk10_bearingmount-rendered_support.png" width="600">

# Z_Axis_Carriage_65mm.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_axis_carriage_65mm.png" width="600">

This is probably one of the biggest, heaviest and longest prints for this project, so you definitely want to get it right on the first print.
You'll need support for the entire bottom face of the ballscrew bolt mount. To preserve your sanity, add the support only on the bottom face, without going into the bolt's holes. Going into the bolt's holes is not necessary and the support will be a pain to remove, with the risk of damaging the hole's shape.
Here's quoted a post from RobF from the discord channel talking about this piece:
"The bottom face and holes on my primitive printer were a bit "grotty", but it doesn't matter as you only need to be able to get your hex nuts into those 6 holes and the bolts above will pull them up into the recess and crush any little bits of support you missed.  Its all facing down and hidden at the back of the carriage so no-one will see it. I was initially a bit concerned how structurally sound it would all come out, but the Z axis assembly and strong bolts ensures its all rock solid in the end."

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_axis_carriage_65mm-painted_support.png" width="600">

Here's how it will look like. Small supports can be added to support the bridging on the sides. They should print fine without supports if your printer is well tuned for bridging, but on a 10+ hours print it's marginal in terms of both print time and wasted material, so better safe than sorry.

<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_axis_carriage_65mm-rendered_support.png" width="600">

# Z_Axis_LinearRailMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_axis_linearrailmount.png" width="600">

# Z_Axis_MotorMount.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_axis_motormount.png" width="600">

# Z_Y_Axis_BallscrewSpacer.STL
<img src="https://raw.githubusercontent.com/RootCNC/Root_4_Lite/main/Media/docs/Print-Info/z_y_axis_ballscrewspacer.png" width="600">
