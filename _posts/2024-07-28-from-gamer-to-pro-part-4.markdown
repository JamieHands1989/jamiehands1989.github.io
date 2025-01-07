---
layout: post
title:  "From Gamer to Pro: Building the Brains of the Keyboard (Part 4)"
date:   2024-07-28 11:21:03 +0000
categories: jekyll update
---
Hey everyone, welcome back to the final installment of the "From Gamer to Pro" series! We've taken a deep dive into the world of custom ergonomic keyboards, exploring the design process from concept to (almost) completion. Today, we'll tackle the final piece of the puzzle: the firmware, the brains that bring our keyboard to life.

Recap: Building the Foundation

Part 1 addressed the limitations of traditional keyboards designed for typewriters. We explored the need for an ergonomic and customizable solution for modern needs. Parts 2 and 3 delved into the creation of the PCB (printed circuit board) and the case design, forming the physical foundation of our keyboard.

But so far, it's just a fancy paperweight. It needs a mind of its own!

Unlocking Customization: The Power of QMK

This is where QMK (Quantum Mechanical Keyboard Firmware) comes in. It's the code we flash onto each half of the keyboard, acting as the bridge between hardware and software. QMK provides incredible customization, allowing us to define the keyboard layout and functionality exactly how we want.

Why Blank Keycaps?

This customization becomes even more powerful with blank keycaps. Traditional keyboards are fixed layouts, regardless of the application or personal preference. Blank keycaps free us from this limitation, allowing us to remap any key based on specific needs. It's similar to macro keyboards and programmable mice, but on a much deeper level.

Configuring the Matrix: Talking to the Keys

To achieve this level of control, QMK scans the keyboard matrix, reading row by row and column by column to determine which key is pressed. With a single keyboard, this is straightforward. However, our split design requires some additional configuration. QMK reads the left and right halves sequentially, meaning the top row on the physical keyboard might actually be row 6 in the matrix. Using the schematics from Part 2, we tell QMK how to interpret this matrix.

Beyond the Basics: Tap Dance and Layers

QMK offers even more advanced features. "Tap Dance" allows a single key to perform different actions based on the number of taps. We can also create multiple "layers" triggered by a key or a Tap Dance combination, essentially creating multiple keyboard layouts on one physical device.

Enhancing the Experience: Via and Vial

While QMK is powerful, Via and Vial introduce user-friendly graphical interfaces (GUIs) for configuring our custom keyboard. Via is a built-in feature within QMK, while Vial is a more modern branch. Both require minor adjustments in QMK to enable them.

Via is the older option and lacks support for some advanced features like Tap Dance. Vial fills this gap, offering better compatibility with modern functionalities.

Here are the resources for diving deeper:

QMK - https://github.com/qmk/qmk_firmware

Via - https://github.com/the-via

Vial - https://get.vial.today/

The Journey Ends... (For Now)

This concludes the "From Gamer to Pro" series. Hopefully, you've enjoyed the journey and feel inspired to embark on your own custom keyboard project. Remember, the world of mechanical keyboards offers endless possibilities for personalization and optimization. Happy building!