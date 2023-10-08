---
title: "Ubik"
excerpt: "Can consciousness exert a weak electrical influence from the OBE state?"
date: 2022-06-22
hidden: false
header:
  teaser: /assets/images/ubik-teaser.jpg
---
In the Philip K. Dick novel [Ubik](https://en.wikipedia.org/wiki/Ubik), scientists use consciousness amplifiers to communicate with those in the [Bardo](https://en.wikipedia.org/wiki/Bardo_Thodol), an intermediary state in Tibetan Buddhism thought to exist between death and rebirth.

When I started meditating, I experienced a phenomenon known as [astral projection](https://www.supermeditate.me/the-astral-express), in which I seemed to leave my body and emerge in another world.  It's something I will never forget, and it left me with a question:  Did my consciousness actually leave my body, or did it just _seem_ that way?

As Michael Faraday once wrote, "Nothing is too wonderful to be true". Because the nature of consciousness has not yet been established, it is important not to make assumptions and instead rely on tests.  But how do we test such a crazy idea?

# Astral Clues
Astral projection is always preceded by the sense of a strong sense of internal vibration.  The fact that such a state is a necessary precondition may offer a clue as to how consciousness and the brain could interface: phase synchronization.

# Phase Sync
It's established that brainwaves correlate to one's state of consciousness, with sleep being at the low end (delta) and alertness being at the high end (gamma). Thalamo-cortical resonance has been proposed as an explanation for how the brain integrates information into a coherent whole.  If we imagine that in the waking state consciousness and the brain are two separate "signals" bound by phase synchronization, the vibrational state makes sense:  It's the interference pattern naturally produced when the two separate.

There is another interesting clue, which is that in astral projection an electrical "snap" is often (but not always) felt upon returning to the body.  Such a snap would be familiar to anyone who has worked with phase-synchronized systems as it corresponds to the phase difference between the two signals when they are re-joined.

In this model, meditation functions by increasing the strength of the "consciousness signal", such that it can exceed that of the brain and break out of phase when the brain's signal is relatively low (during sleep or deep meditation.)

If consciousness and the brain are coupled electrically, and consciousness can separate out, then we should be able to measure its influence on another object with a subject who is in the OBE state.

# Testing
While many tests have been conducted on subjects in the OBE state, they are typically focused on measuring brain activity, but in our model we would not expect a considerable difference, after all the "car" is still idling while the driver has left the vehicle.  Instead, we will measure the electrical activity of another object which the OBE'd subject will then attempt to manipulate.

If you're still with me I appreciate it, because we're really out on a limb here, but let's keep going.

We don't know if our "consciousness signal" needs to bind to an existing electrical signal first before it can exchange information, or if it can just push electrons around willy-nilly, so in terms of measurement we will need two solutions:
1. A saltwater solution with no electric current applied.
2. A saltwater solution with a brainwave-like sinusoidal current applied.

If an individual can astral project from Point A and successfully wiggle some electrons at Point B---passing a message in Morse code, for example---it would demonstrate that the influence of consciousness extends beyond the brain.

# Parts
A microvolt-sensitive voltmeter in an RF-isolated enclosure is used to record a time series measurement of voltage within a saltwater solution.  It's relatively low-cost ($400 USD) and easy to assemble.  The full BOM is [here](https://docs.google.com/spreadsheets/d/1x1zZBeL7GawCRSwFvTGJBpj9yIvj37LNaCB3L1gBPrs/edit?usp=sharing). It consists of:

1. [Voltmeter](https://www.yoctopuce.com/EN/products/usb-electrical-sensors/yocto-millivolt-rx-bnc) + [enclosure](https://www.yoctopuce.com/EN/products/enclosures/yoctobox-long-thick-black-bnc).
2. Data logging:
  - [Yoctopuce Ethernet board](https://www.yoctopuce.com/EN/products/extensions-and-networking/yoctohub-ethernet) OR
  - Ubik's [Android logging app](https://tbd).  This is a good option for travel, as the phone can provide both power & logging capability.
3. RF enclosure (Amazon list)
4. Lab stand & flask (Amazon list)

# Output





## Voltmeter

The voltage threshold required for a neuron to fire is about 30 millivolts, so assuming the brain does not act as an amplifier, that's the maximum voltage range we need to look for.

While something like an Arduino could work, that device is hampered by several factors including lack of negative voltage, no shielding, and generally not being designed for high-sensitivity use.

I settled on a sensor built by the Swiss hardware company Yoctopuce, designed for high-sensitivity use such as pH measurement.  It is electrically isolated, accommodates very high impedance (weak signals), and includes a BNC (shielded) connector for our electrode.  It can log a small amount of data onboard or it can be connected to USB or Ethernet (the latter via an additional board.)  While the sampling rate is not as high as I would like, it's low cost and ease of use won the day.



Our test case is:
  1. Successfully astral project
  2. Navigate to Ubik
  3. Attempt to influence the signal by introducing something non-random such as Morse code.

