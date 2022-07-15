---
title: "Ubik"
excerpt: "A simple device to test whether consciousness can exert an electrical interface while in an OBE state."
date: 2022-06-22
hidden: false
header:
  teaser: /assets/images/ubik-teaser.jpg
---
In the 1967 Philip K. Dick novel [Ubik](https://en.wikipedia.org/wiki/Ubik), a specialized amplifier is used to communicate with those in the [Bardo](https://en.wikipedia.org/wiki/Bardo_Thodol), the intermediary state of Tibetan Buddhism thought to exist between death and rebirth.

I stumbled onto the Bardo by way of a phenomenon known as astral projection, which [occurred spontaneously](https://www.supermeditate.me/the-astral-express) through meditation.  These experiences heightened my curiosity as to whether my consciousness was actually separating from my body.

Certain details common to AP / OBE experiences suggest that this may be possible to test empirically, and Ubik is my first stab at such an effort.

# Poking The Bardo

If consciousness and the brain are in fact separate, the most obvious interface between the two would be electrical.  If this is the case, it should be possible for an astrally-projected individual at Point A to wiggle some electrons at Point B:

Ubik tests this idea by acting as a "surrogate brain" which an astrally-projected consciousness could (in theory) influence.  Ubik can detect very weak electrical signals (tens of microvolts) at very high impedance, meaning that if consciousness is electrical, and can separate out, Ubik should be able to detect it.


# Parts
Ubik is relatively low-cost ($400 USD) and easy to assemble.  The full BOM is [here](https://docs.google.com/spreadsheets/d/1x1zZBeL7GawCRSwFvTGJBpj9yIvj37LNaCB3L1gBPrs/edit?usp=sharing). It consists of:

1. [Voltmeter](https://www.yoctopuce.com/EN/products/usb-electrical-sensors/yocto-millivolt-rx-bnc) + [enclosure](https://www.yoctopuce.com/EN/products/enclosures/yoctobox-long-thick-black-bnc).
2. Data logging via:
  - [Yoctopuce Ethernet board](https://www.yoctopuce.com/EN/products/extensions-and-networking/yoctohub-ethernet) OR
  - Ubik's [Android logging app](https://tbd).  This is a good option for travel, as the phone can provide both power & logging capability.
3. RF enclosure (Amazon list)
4. Lab stand & flask (Amazon list)
5. Common parts & equipment (Amazon list)

Note that item 5 contains very common equipment such as a wire stripper, ground cable, etc. so please omit any items you don't need.

# Assembly

Fully assembled, Ubik looks like this:

(image)

### 1. Build the enclosure

### 2. Assemble the stand

### 3. Assemble the electrode

### 4. Wire the circuit

### 5. Prepare the flask

### 6. Set up data logging

### 7. Run a validation test





# Output





## Voltmeter

The voltage threshold required for a neuron to fire is about 30 millivolts, so assuming the brain does not act as an amplifier, that's the maximum voltage range we need to look for.

While something like an Arduino could work, that device is hampered by several factors including lack of negative voltage, no shielding, and generally not being designed for high-sensitivity use.

I settled on a sensor built by the Swiss hardware company Yoctopuce, designed for high-sensitivity use such as pH measurement.  It is electrically isolated, accommodates very high impedance (weak signals), and includes a BNC (shielded) connector for our electrode.  It can log a small amount of data onboard or it can be connected to USB or Ethernet (the latter via an additional board.)  While the sampling rate is not as high as I would like, it's low cost and ease of use won the day.



Our test case is:
  1. Successfully astral project
  2. Navigate to Ubik
  3. Attempt to influence the signal by introducing something non-random such as Morse code.

