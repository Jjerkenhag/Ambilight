# Ambilight
Ambient light software for Arduino and neopixel LED

The program takes the median of the color in the top-area of the screen and sends it to the corresponding LED through the Arduino.
The program is written in C# for simple testing and the code for the Arduino is made in their official IDE.

In my opinion everything above 30 updates per second is close to non-noticeable in delay.
However, a jump from 25 -> 33 pixels per LED give almost double the update time but most commonly no apparent change in color.

My preffered configuration:
- 20x20 pixel gathering
- 1/3 of screen
- non-linear
- no extant
- 100 brightness
- This gives ~60 updates per second with ~40 ms delay and a CPU usage of ~5%.

TODO:
- Implement audio mode
- Implement ambient mode (soft color change etc.)
- Add extant to video
