# Two Transistor Surround Sound Decoder / Vocal Remover Preamplifier
A very simple two transistor surround sound decoder or vocal remover preamplifier based off two Class A audio amplifiers. This method of surround sound decoding simply isolates the out of phase audio in a stereo mix.

Watch the video on how to build: https://youtu.be/4wfMt4YOYYA

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
3. Change the resistance of `R5` or `R6` to change the gain of the preamplifier; if the output volume is too loud or too quiet.

## Troubleshooting
- **Mid-high range frequency constant click/popping sound:** This is caused by wireless interference. The circuit is not protected from EMF interference. Please remove any wireless devices (such as a cellphone) 10 feet away from the circuit or turn them on airplane mode while in use.
- **Some vocals/mono audio sound is still leaking into the Out of Phase audio:** Assuming that the audio you are playing doesn't natively have any vocals in the Out of Phase audio, If you haven't done so already, it is important that you use ±1% tolerance resistors or less to limit this from happening. Regardless, Vocals can still leak through as a result of the diodes in the NPN transistors having reverse current leakage.

## Licensing & Attribution
- This repo is licensed under the BSD 3-Cause license. Any images are licensed under CC BY-SA 3.0. Refer to `LICENSE` for more info.
