---
layout: post
title:  "From Gamer to Pro: Building a Custom Ergonomic Keyboard (Part 2) - PCB Design"
date:   2024-07-10 11:21:03 +0000
categories: jekyll update
---
Welcome to part 2 of the From Gamer to Pro series! In part 1, we explored the journey from gamer to developer and why a traditional keyboard wouldn't cut it anymore. We also looked at the exciting world of ergonomic keyboards and how this project aims to build a custom split keyboard with a staggered column layout.

Now, let's delve into the nitty-gritty: building the PCB! There are various ways to wire a mechanical keyboard. This series will focus on the PCB matrix approach, leaving hand-wiring and direct-pin wiring for a potential future series if there's enough interest.

What is KiCad? KiCad is a free, open-source software for electronics design that allows us to create schematics and design PCBs (Printed Circuit Boards).

Decisions for PCB Design

When creating a mechanical keyboard PCB, we have several decisions to make:

Hand-wiring vs. PCB:  For this project, we'll use a PCB to benefit from the additional support it provides for hot-swappable switches.

Direct-pin vs. Matrix Wiring:  Due to the number of switches (52 across both halves), we'll use matrix wiring, which requires adding diodes to prevent keystroke ghosting.

Communication between Keyboard halves:  We'll use I2C communication (requiring 4 pins) for its speed compared to the slower serial option (using 3 pins).

Understanding Schematic Symbols

Before diving into schematic creation, let's explore the basic symbols used for our custom keyboard:

Switch (Symbol: ⿲ ): The foundation of your keyboard, responsible for registering key presses. These lines often represent the internal mechanism of the switch.

Diode (Symbol: ▶ ): Tiny one-way electrical valves that prevent unwanted current flow, crucial for avoiding keystroke ghosting. The line segment typically points in the direction the current can flow.

Microcontroller (Optional, Symbol: Varies): The brains of your keyboard, allowing for programmability and advanced features. It might be represented by a square with internal markings. (You might choose a simpler design without a microcontroller for this project).

Resistor (Optional, Symbol: □ ): Used for various purposes depending on the complexity of your design. The color code on the rectangle helps identify its resistance value. We'll explore these visuals in more detail later.

Connectors (Symbol: Varies):  These establish connections between the PCB and other components like the USB cable. They can have various shapes depending on the connector function.

Creating the Schematic and PCB Layout

Once you have a finalized schematic with all the components and their connections mapped out, it's time to translate that information into the actual PCB layout using KiCad.  Each symbol in the schematic corresponds to a footprint in the PCB layout, which defines the physical size and shape of the component on the board.

For this project, footprints were obtained from external resources and modified to create a reversible PCB design (usable on both sides).

Manufacturing the PCB

Since we don't have the equipment for PCB manufacturing, we'll use a service like JLCPCB (https://jlcpcb.com/). To order PCBs, we need to export Gerber files from KiCad.  These files contain the schematics and designs for our PCBs.

Resources

Joe Scotto's YouTube channel (https://www.youtube.com/@joe_scotto) offers excellent tutorials on KiCad usage and custom mechanical keyboard creation.

Conclusion

This concludes part 2 of the From Gamer to Pro series! We've explored the PCB design process using KiCad. In the next article, we'll take our schematics and physical PCBs and use them as a foundation to build the plates and cases for the keyboard. Stay tuned for Part 3: Building the Keyboard Housing!