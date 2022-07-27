---
title: "Ubik"
excerpt: "A voltmeter + enclosure designed to detect whether consciousness can exert a weak electrical influence from within an OBE state."
date: 2022-06-22
hidden: false
header:
  teaser: /assets/images/ubik-teaser.jpg
---
In the Philip K. Dick novel [Ubik](https://en.wikipedia.org/wiki/Ubik), a specialized amplifier is used to communicate with those in the [Bardo](https://en.wikipedia.org/wiki/Bardo_Thodol), an intermediary state in Tibetan Buddhism thought to exist between death and rebirth.

When I started meditating, I stumbled onto the Bardo [accidentally](https://www.supermeditate.me/the-astral-express) by way of a phenomenon known as astral projection.  The experience heightened my curiosity---was my consciousness actually separating from my body, or did it only seem to?

Details common to AP / OBE experiences suggest a new and intriguing way to test this empirically, and Ubik is my first stab at such a test.

# The Theory
Assuming for a moment consciousness can in fact separate from the brain, there would have to be an interface allowing communication between the two, and that interface is likely to be electrical.

If an individual can astral-project at Point A and successfully wiggle electrons at Point B---passing a simple message in Morse code, for example---it would demonstrate that the influence of consciousness can extend beyond the brain, opening a new and exciting avenue for further study.

# Parts
Ubik is a highly-sensitive voltmeter in an RF-isolated enclosure designed to detect microvolt-level currents in a saltwater solution of similar ionic composition as the brain.  It's relatively low-cost ($400 USD) and easy to assemble.  The full BOM is [here](https://docs.google.com/spreadsheets/d/1x1zZBeL7GawCRSwFvTGJBpj9yIvj37LNaCB3L1gBPrs/edit?usp=sharing). It consists of:

1. [Voltmeter](https://www.yoctopuce.com/EN/products/usb-electrical-sensors/yocto-millivolt-rx-bnc) + [enclosure](https://www.yoctopuce.com/EN/products/enclosures/yoctobox-long-thick-black-bnc).
2. Data logging:
  - [Yoctopuce Ethernet board](https://www.yoctopuce.com/EN/products/extensions-and-networking/yoctohub-ethernet) OR
  - Ubik's [Android logging app](https://tbd).  This is a good option for travel, as the phone can provide both power & logging capability.
3. RF enclosure (Amazon list)
4. Lab stand & flask (Amazon list)
5. Common parts & equipment (You may already own some of these)

# Steps to Assembling

Fully assembled, Ubik looks like this:

(image)

### 1. Assemble the enclosure

### 2. Assemble the stand

### 3. Crimp the electrode

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

