# Two Transistor Surround Sound Decoder / Vocal Remover Preamplifier
A very simple two transistor surround sound decoder or vocal remover preamplifier based off two Class A audio amplifiers. This method of surround sound decoding simply isolates the out of phase audio in a stereo mix.

![alt text][s]

[s]: https://github.com/DaGooseYT/ss-decoder/blob/main/schematic.png

## Features & Usage

### Features
- Low power consumption: ~10mA @5v
- No frequency band limitations on output.
- Can be used with virtually any audio amplifier at any power output
- Very high linear quality, being based on the Class A audio amplifier
- Small and simple design; makes it easy to integrate into any application
- Can accept any linear input, including but not limited to Bluetooth devices.

### Usage
Refer to the schematic diagram to follow these steps.

1. Connect a linear audio source to resistors `R5` and `R6`. **The audio source must be a stereo mix.**
2. Connect the input of your audio amplifier to the output of the preamplifier on the collector pins of transistors `Q1` and `Q2`.
3. Change the resistance of `R5` or `R6` to change the gain of the preamplifier, if the output sound is too loud or too quiet.

## Licensing & Attribution
- Everything in this repository (including the schematic and BOM) are licensed under the BSD 3-Cause license. Refer to `LICENSE` for more info.
- Apart from the conditions in the `LICENSE` file, if you choose to showcase the contents of this repository (modified or not) in a presentation or video, please provide attribution or disclaimer somewhere (such as the video description) in the following format:
`The Surround Sound Decoder (Vocal Remover) schematic/circuit was initially provided by DaGoose.
Original project source: https://github.com/DaGooseYT/ss-decoder.`
