---
layout: post
title:  "From Gamer to Pro: Building a Custom Ergonomic Keyboard (Part 3) - Case Design"
date:   2024-07-21 11:21:03 +0000
categories: jekyll update
---
Continuing the 'From Gamer to Pro' series, this article details creating a custom ergonomic keyboard case using 3D printing and basic design principles.

The Plate: Foundation for Stability

The plate holds the switches in place and prevents keyboard flex during typing. Since I have a 3D printer, I opted to print the plate using PLA filament with 100% infill for maximum sturdiness.

Designing the Plate in Autodesk Fusion 360:

Import and Outline: I imported the PCB model from Part 2 and used the projection tool to create the plate's basic shape.

Switch Sockets: Using the switch dimensions and PCB layout, I created slightly oversized holes for the switches in a sketch.

Double Extrusion for Strength: The first extrusion created a base of 1.5mm, while the second extrusion with a slightly smaller hole size added another 1.5mm, resulting in a sturdy plate with proper switch fit. This technique allows for a thicker plate without compromising switch compatibility.

Printing Considerations:

Molten plastic shrinks as it cools. Most slicers allow for shrinkage compensation, but the exact value depends on the filament used. Experimentation might be necessary to achieve the perfect fit.

Creating the Case:

Following a similar process as the plate, we can design the case using Fusion 360:

Projecting the Plate: We can project the plate outline onto a new sketch and offset it slightly to create a clean finish for the case.

Extrusions and Cutouts: The case outline is extruded to a desired depth, and then another extrusion creates the base. Cutouts for ports and screw holes are made using the project and offset tools with negative extrusions. Heatset inserts were chosen for a clean, threaded screw connection.

Finishing Touches:

3D-printed objects often have visible layer lines. To achieve a smooth finish for painting, I used automotive primer filler,sanding between coats. Finally, the case was painted with gunmetal grey using an airbrush (a first-time experience that yielded a satisfying result!).

Assembly and Next Steps:

After the paint dried, the keyboard was assembled with added feet to prevent desk-sliding. In the next article, we'll dive into the world of keyboard firmware – the brains behind the keys! Stay tuned!