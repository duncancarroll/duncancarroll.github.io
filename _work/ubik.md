---
title: "Ubik"
excerpt: "An ongoing study to determine if consciousness can exert a weak electrical influence in the OBE state"
date: 2023-10-11
hidden: false
header:
  teaser: /assets/images/ubik-teaser.jpg
---
Are you ready to go out on a limb?

In the 1969 Philip K. Dick novel [Ubik](https://en.wikipedia.org/wiki/Ubik), scientists use consciousness amplifiers to communicate with those in the [Bardo](https://en.wikipedia.org/wiki/Bardo_Thodol), a state also known as the "astral" in which consciousness is thought to be able to exist independently of the body.

When I started meditating, I spontaneously [astral projected](https://www.supermeditate.me/the-astral-express), seeming to leave my body and emerge in another world.  I can't properly explain how strange this was, and the "realness" of it left me wanting to find a way to ascertain whether my consciousness was actually leaving my body or not.

Of course, if we wanted to stop at Occam's Razor, we could call it a day and say that these are dream-like or hallucinatory experiences---but where's the fun in that?  As Michael Faraday wrote, "Nothing is too wonderful to be true" so in that spirit we will not make any assumptions and instead rely on what we can test.

Ok, but how do we test something like this?

# Astral Clues
If consciousness and the brain are separate, there'd have to be an interface by which the two communicate--- so what might that interface be?

One clue is that astral projection is always preceded by a strong sense of internal vibration.  Like, _really_ strong. Like, "Holy f\*ck I'm being electrocuted" strong.  It turns out that this is a universal precondition--- one cannot AP unless in the so-called "vibrational state". Interestingly, one can remain in this state _without_ projecting, in other words it seems to facilitate the process rather than being a side-effect of it. This led me to the idea that consciousness and the brain might interface by phase synchronization.

Phase synchronization is a phenomenon that occurs whenever parts of a system are coupled, most often in those with wave-like properties, and it can happen mechanically as well as electrically, for example, soldiers marching over a bridge must march out of step or the resonant frequency will cause it to collapse.  In an AC power grid, multiple sources of electricity must first be [synchronized](https://en.wikipedia.org/wiki/Synchronization_(alternating_current)) before they can be joined together.  Might such synchronization be happening in the brain?

We know that brainwaves correlate to states of consciousness, with sleep being at the low end (delta) and alertness being at the high end (gamma), and [thalamo-cortical resonance](https://en.wikipedia.org/wiki/Recurrent_thalamo-cortical_resonance) has been proposed as an explanation for how the brain integrates information into the coherent whole we call "perception".  If we imagine that in the normal waking state consciousness is phase-synchronized to the brain, the vibrational state could simply be the interference pattern produced when the two separate.

An electrical "snap" is also frequently reported by APers upon returning to the body.  While perhaps a minor observation, it's similar to what happens when two electrical signals of different phases are joined.  If the phases are equal enough, no snap is felt, but if not... snap crackle pop.

This is highly speculative territory---but don't worry, we're going to test it.

The model also explains the question of why meditation---the act of sitting still and focusing one's attention---would ever cause something so bizarre as astral projection in the first place: By increasing the strength of attention, we are increasing the strength of the "consciousness signal", ultimately causing it to break out of phase at a time when the brain's signal are reduced (i.e. in sleep or meditation).

Could the linkage between these two systems simply be electrical?  While there's no reason to assume this (maybe it's magnetic?  Chemical?  Or if you're Stuart Hameroff, scale-independent quantum oscillatory), electrical sensors are cheap so we'll start there.

# Testing
While [numerous tests](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3918960/) have been conducted on subjects in an OBE state, they are usually focused on body and brain activity, but we would not expect a major difference there, after all, in our model the "car" is still idling, it's just that the driver has left the vehicle.

Instead, we will take a different approach and measure the electrical potential of a nearby object, a "surrogate brain" (in this case a flask of saltwater), while a subject in an OBE state attempts to manipulate it and pass a message via Morse code.

Why saltwater?  It's conductive and provides an environment remotely similar to the brain.  One thing we don't know is whether or not our "consciousness signal" needs an existing electrical signal to synchronize to or if it's strong enough to just push electrons around by itself, so we will need two solutions:

1. 10 mL saltwater with no current applied.
2. 10 mL saltwater with a sinusoidal current applied.

If a subject can astral project from Point A and successfully wiggle some electrons at Point B, it would demonstrate that the influence of consciousness can extend beyond the brain under certain conditions.

# Parts
The sensor is not complicated.  A voltmeter with 5uV resolution is placed in an RF-isolated enclosure and used to record a time series measurement of voltage within a saltwater solution at ~30 Hz:
1. [Voltmeter](https://www.yoctopuce.com/EN/products/usb-electrical-sensors/yocto-millivolt-rx-bnc) + [enclosure](https://www.yoctopuce.com/EN/products/enclosures/yoctobox-long-thick-black-bnc).
2. Data logging - [Yoctopuce Ethernet board](https://www.yoctopuce.com/EN/products/extensions-and-networking/yoctohub-ethernet)
3. RF enclosure
4. Lab stand & flask

# Process
- A Typescript app is used to connect to the sensor, retreive data, and log it to a CSV (and optionally InfluxDB.)
- 10 mL distilled water is mixed thoroughly with 1/4 tsp lab-grade NaCl.
- The sensor is tested by introducing a sine wave into the solution and verifying the output.
- Normal output shows stable voltage with long-period fluctuations over a 24-hour period of +/-20mV.


# Execution
Now all we need to do is meditate frequently enough that we astral project. Some things to remember:

1. Run the sensor every night.  Even when you're meditating regularly there's really no telling when you're going to AP, so if you forget to turn it on you might miss it.

2. Keep the sensor as close to you as possible, ideally within arm's reach. You don't move like a normal human being in the OBE state (There's no gravity, your arms and legs pass through everything, etc.) so try to position the sensor such that it can be reached with one arm while laying down.

3. After you AP, mark the time immediately or you will have no reference point when looking at the data.

4. Record video with timestamp or no one will believe you (no one will believe you anyway, but still...)

5. The vibrations are of two types:  Minor and major, and you can only separate while in major.  Minor vibrations are mild and feel like you're sitting next to a subwoofer.  Major vibrations feel like you've stuck your finger into an electrical socket and your fight-or-flight instinct will kick in strongly, so it's important to remember to stay cool when you attempt to separate.  Once separated, the vibrations will disappear.

6. Regular meditation is one of the most reliable ways to trigger AP, but there are additional techniques you can add on to improve your odds such as sleep interruption.

# Progress
So far I've had two APs with Ubik in place, but one was aborted due to my alarm clock going off, and the second time I successfully separated but I'd placed the sensor across the room and couldn't get to it in time.

# Perfectly Reasonable Questions
- *If consciousness is separate from the brain, why does anesthetizing the brain eliminate it?*  The only explanation I have is that in the non-OBE state, consciousness is "trapped" or otherwise fully encapsulated by the body, and because the brain's signal is normally the stronger of the two, when it goes down it takes consciousness with it.

- *Both Buddhism and science tell us that every action is the result of a deterministic causal chain, and as a result consciousness is an illusion.*  I don't know if this is true or not, but it doesn't invalidate the model because we're not saying anything about consciousness except that it can separate from the body.  This theory doesn't explain qualia or free will, so the inviolable causal chain could still exist and this would just be another part of it.

- *What are we "seeing" in the OBE state?*  Well, we're definitely not seeing an accurate representation of objective reality.  Instead, it's more like the mind's last representation of the world around us, but because it's not "grounded" by sensory input, things are slightly off.  Doors, windows, or items may not be in the right places.  If you were wearing a watch to sleep, you will find that it is there, but it's not functional or displays nonsensical information.  Generally speaking, it's not as though we are a ghost flying around; it's more like we're a buggy version of Google Street View.

- *ChatGPT seems pretty close to being conscious, how about that?*  My argument here is that the difference is subtle but important:  If LLMs are the brain, then consciousness is the prompt.  If the car is the brain, consciousness is the driver.  Can we have self-driving cars which are indistingiushable from human drivers?  Yes!  Are they conscious?  No, I don't think so.  However, if this model is correct the interplay between AI and consciousness may soon be closely interlinked (more below.)

- *What does this model say about death?*  In this model, death is a separation of consciousness from the body wherein the brain can no longer generate sufficient signal to bind to.  In theory it would be possible to create a replacement interface to which a Bardo-roaming consciousness could bind to & manipulate.  This would open up a fascinating new field of study and engineering, and would be a more practical route to life extension than attempting to keep the body alive indefinitely.  It is also one way to imagine how the Kurzweilian "uploading our consciousness into computers" / "merging with AI" scenario might play out.

# Contact
If you are interested in this study and promise not to be snarky feel free to [drop me a line](mailto:duncan.carroll@gmail.com).
