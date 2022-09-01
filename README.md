# Max-Devices
This repository contains various audio devices that I built for Max/Msp / Max For Live. 

## Tinntinabuler
__*Max patcher (.maxpat)- Generative music machine inspired by Arvo Part*__\
*Also available for Mac for Live! (.amxd)*

![Tinntinabuler](https://i.imgur.com/KRnjUSR.png)

Tinntinabuler is a patch that creates generative music based on *tinntinabuli*, a voice leading method invented by composer Arvo Part. It creates very rich harmonies and a lush textutre.

## Tite Fold
__*Max for Live audio effect (.amxd) - fold distortion / saturation effect*__

![Tite Fold](https://i.imgur.com/Z3QXfgi.png)

This is a simple (yet versatile) fold distortion / saturation effect.

Controls:

- __*Drive*__ - the amount of input gain.
- __*Soft / med / hard*__ - Multiplies the Drive parameter by 1, 2.5 and 5, respectively.
- __*Out*__ - Controls the output level of the distortion.
- __*Dry / wet*__ - A mix control between the dry and distorted signal.

## Noiz Osc

![Noiz Osc](https://i.imgur.com/Siup4wR.png)

__*Max for Live instrument (.amxd) - monophonic string modeling synthesizer*__

This is a monophonic synth which creates notes using white noise fed into comb filters, which results in a sound that is similar to a string.\
It is featured on a track that I released recently ([you can listen to it here](https://itaiarad.bandcamp.com/track/pardes-yavesh)), and was built especially to be used in it.

Controls:

- __*MIDI module*__ - Controls MIDI input behaviour.
- __*Partials*__ - This controls that number of filter chains in the system (they are used in parallel).
- *__Pitch modulation__ (rate + depth)* - This modulates the pitch of the filters randomly, which can be used to create unison and other special effects.
- __*Envolope*__ - This is a standard ADSR envelope for the synth.
- __*Feedback*__ - Controls the comb filers' feedback - higher values have a more defined pitch, while lower values become more noisy.
- __*Q*__ - Noiz Osc uses a lowpass filter for each partial at the end of the chain - This controls their resonance. The cutoff frequencies are random and cannot be changed.
- __*Rate*__ - The rate of pitch and amplitude modulation.
- __*Density*__ - The 'density' of the modulation - higher values will result the modulation to statistically give higher values, and vice versa.
- __*Attack / Decay / Sustain / Release*__ - Standard ADSR envelope for the output signal.
- __*Out*__ - Output level control.

## Justin

![Justin](https://i.imgur.com/qDTQIAP.png)

__*Max for Live instrument (.amxd) - Oscillator for die-hard just intonation folks*__

This extremely simple device is just an oscillator which is tuned manually, and can accept highly accurate decimal values.\
I was asked to build this by a friend who worked a lot with just-intonation for his compositions and needed an oscillator that can be tuned very percisely.

Controls:
- __*Waveform*__ - Toggles between sine, saw, square and triangle for the waveform.
- __*Pitch*__ - The oscillator's frequency in Hertz.
- __*Multiply*__ - Multiplies the frequency. Possible values go from 0.5, doubling at each step up to 32, allowing you to shift octaves easily.
- *__VCA__ (value + response)* - You can have flexible control over the VCA by mapping another Max For Live device (such as an envelope or a LFO) to the *value* slider. *Response* changes the VCA's behavior from exponential to linear.
- __*Output*__ - Output level control.
