# Nebulae_v2_Instruments
Alternative instruments for the Qu-Bit Nebulae v2 Eurorack module. Each file can also be used in any Pure Data project.

This software was written by Samuel Burt in Pure Data. It will run in Pd-vanilla on any computer, but is specifically designed to run on the Qu-Bit Nebulae v2. 

# Installation
Simply copy the pd files onto the root level of your Nebulae USB flash drive. When you turn on your Nebulae, the files will automatically load. To load a file, push and hold the "speed" button for two seconds. Rotate the speed button and observe the five buttons on the Nebulae. When the main instrument page is selected (with the Nebulae's original granular instrument) all five buttons should dimly light. The currently loaded instrument's slot will glow more brightly. From the main instrument page, rotate the "speed" encoder to the right. From here you can select the instrument you want to load by pressing its corresponding button and then pressing the "speed" button. Give the Nebulae about fifteen seconds to load the program.

# Options as of 2022_01_03
The four instruments appear in this order:

- 00_supersaws.pd
- 01_chord_maker.pd
- 02_rainstick.pd
- 03_pansshadow.pd

## 00_supersaws.pd
00_supersaws.pd generates four different voices each consisting of seven sawtooth waveforms that spread based on the central Pitch spread knob. Toggle off three voices to have a single monophonic voice. Two voices go out the left outlet and two go out the right.

## 01_chord_maker.pd
01_chord_maker.pd produces up to five tunable waveforms in the form of chords. This program takes care of chord quality and inversion, basing these properties off the key, chord root, and range knob. Notes in a chord automatically wrap (inverting the chord) if they would appear below the lowest note set by the Range knob. The Jazz button will turn all (dominant) V chords into augmented chords. Waveshapes transition from a sine wave to shapes with more harmonics, while Waveform Modulation changes the balance between fundamental and overtones.

## 02_rainstick.pd
02_rainstick.pd creates a live granulated delay line of up to six seconds in length. Grain size, density, and pitch can all be randomized with the Randomization knob.

## 03_pansshadow.pd
[CURRENTLY INOPERABLE] 03_pansshadow.pd tracks the pitch and note durations of its input. These pitch and note durations are reordered and either output as a three voice brass sound or as two volts-per-octave control voltages. Each voice can be assigned to either play back the pitches and notes in sequence, randomly, foreward/reverse, randomly weighted for the most common notes, or randomly weighted for the most recent notes.

# Notes for the future
These instruments are not necessarily in their finished form. They are playable right now! Future iterations might change some of their functionality to provide improvements and more levels of control.

