---
layout: post
title:  "Grounding Scheme"
date:   2018-10-23 14:59:06 +0200
categories: Amp
---


# Introduction
The grounding scheme as it is indicated in the build manual is suboptimal. I'm trying to follow the daisy chained multiple star scheme as descripted in 'Designing Tube Preamps for Guitar and Bass': [Grounding](http://www.valvewizard.co.uk/Grounding.pdf).

# Amplifier Parts

## (Fixed Bias) Power Output Stage
Based on p.273. Ground of bias supply (**positive** side) meets the cathodes bias resistors together with the filter caps. These two filter caps are both located in one can cap (32+32uF, 500V) and share a common negative (ground) lug. This lug thus seems to be a logical place to use as the ground star.

## Long Tail Pair Phase Invertor
Based on p.274. Ground from speaker output should use this star ground together with the ground of the LTPPI and the accompagnying filter cap (half of the 16+16uF, 500V can cap; other half is not used). Both anode resistors have a separate connection to the *positive* star. I don't see a good way to achieve this. Where does the tone stack ground belong?

## Pre Amp
Based on p.274. Separate wires to the *positive* star for the anode resistors. Every tube should have its own little _tube star_ and then these should then be connected to the pre amp local star with a separate wire. 1M resistor should also be connected to this _tube star_, so it should not be located at the input jack. Then finally the daisy chain should connect to the chassis. The book is not totally consistent. In one image the input ground is connected to the first tube star, in another it is connected to the local star. This should be the **only** connected to the chassis of the ground. The other input should thus not be connected to the chassis.