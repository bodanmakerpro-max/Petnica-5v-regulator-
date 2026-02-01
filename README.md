5V Linear Regulator Using TL431 + NPN Transistor

This project is a simple 5V linear voltage regulator made from common parts.
It uses a TL431 as a precision reference and error amp, and a 2N3904 transistor as the pass element.

The goal of this circuit is to get a stable 5V output without using a 7805 or switching regulator. it’s good for learning and for low power stuff.

What this is

discrete 5V linear regulator

based on TL431 adjustable reference

NPN transistor handles the load current

simple and cheap parts

simulated in LTspice

How it works (short)

The TL431 compares the output voltage using a resistor divider

When output goes above or below 5V, TL431 sinks more or less current

This controls the base of the 2N3904

The transistor adjusts current to keep output around 5V

C1 smooths the output voltage

That’s it. no magic.

Schematic overview

Input voltage: around 7V to 12V recommended

Output voltage: ~5V

Reference: TL431

Pass transistor: 2N3904

Output capacitor: 100uF

Load resistor in sim: 1k

Parts list

TL431 adjustable reference

2N3904 NPN transistor

R1: 300 ohm

R2: 8.7k

R3: 8.7k

R4: 1k (load, for testing)

C1: 100uF electrolytic

Notes and limitations

This is a linear regulator so it wastes power as heat

Not good for high current loads

Output current is limited by the transistor

No thermal protection

No short circuit protection

If you want more current, use a bigger transistor or add a power BJT.

Use cases

small logic circuits

sensors

microcontroller experiments

learning how linear regulators actually work

Simulation

Designed and tested in LTspice.
Transient and DC sweep used to check stability and output voltage.

License

Do whatever you want with it.
Use it, modify it, break it, learn from it.[Read me file.txt](https://github.com/user-attachments/files/24993890/Read.me.file.txt)
